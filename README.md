# parcelable

Android Parceling support for the [Kotlinx Serialization library](https://github.com/Kotlin/kotlinx.serialization)
. <br />
<img alt="GitHub tag (latest by date)" src="https://img.shields.io/github/v/tag/chRyNaN/serialization-parcelable">

<a href="https://androidweekly.net/issues/issue-450"><img alt="Badge" src="https://androidweekly.net/issues/issue-450/badge" height="20px"></img></a>

```kotlin
intent.putExtra("key", value, serializer)
val value = intent.getParcelableExtra("key", deserializer)

// Compose
rememberSavable(serializer) { value }
```

Now all the serialization can be handled from a single library, no need to create both custom Parcelers and Serializers.
Have a custom class that requires specific serialization? Use
the [Kotlinx Serialization library](https://github.com/Kotlin/kotlinx.serialization), and it will automatically work
with Android's `Parcel`, `Bundle`, and `Intent`.

## Building

The library is provided through [Repsy.io](https://repsy.io). Checkout
the [releases page](https://github.com/chRyNaN/parcelable/releases) to get the latest version. <br />
<img alt="GitHub tag (latest by date)" src="https://img.shields.io/github/v/tag/chRyNaN/serialization-parcelable">

### Repository

```groovy
repositories {
    maven { url = "https://repo.repsy.io/mvn/chrynan/public" }
}
```

### Dependency

#### Core

```groovy
implementation("com.chrynan.parcelable:parcelable-core:$VERSION")
```

#### Compose

```kotlin
implementation("com.chrynan.parcelable:parcelable-compose:$VERSION")
```

## Usage

* Setup the `Parcelable` object:

```kotlin
val parcelable = Parcelable {
    serializersModule = mySerializersModule
}
```

* Use [Kotlinx Serialization](https://github.com/Kotlin/kotlinx.serialization) to serialize your model class:

```kotlin
@Serializable
data class MyModel(
    val intField: Int,
    val stringField: String,
    val nullableStringField: String? = null
)
```

* Pass your model through `Intents` and `Bundles`:

```kotlin
// Put
intent.putExtra(key, myModel, parcelable)
bundle.putParcelable(key, myModel, parcelable)

// Get
val myModel = intent.getParcelableExtra(key, parcelable)
val myModel = bundle.getParcelable(key, parcelable)
```

* Or serialize to and from `Parcels` and `Bundles`:

```kotlin
// To
parcelable.encodeToParcel(parcel, myModel)
val bundle = parcelable.encodeToBundle(myModel)

// From
val myModel = parcelable.decodeFromParcel(parcel)
val myModel = parcelable.decodeFromBundle(bundle)
```

* Or serialize to a `Saver` with Jetpack Compose

```kotlin
val model = rememberSavable(parcelable = parcelable, serializer = MyModel.serializer) { myModel }
```

## Documentation

More detailed documentation is available in the [docs](docs) folder. The entry point to the documentation can be
found [here](docs/index.md).

## Sample

The `sample-android` module contains an Android App showcasing the use of this library and providing a means to test
parceling different models.

Simply update the `ExpectedModel.model` value to be any Serializable class and run the application to test if the
parceling worked.

### Sample Screenshots

![Main Screen](assets/sample_main_screenshot.png)
![Results Screen](assets/sample_result_screenshot.png)

## License

```
Copyright 2021 chRyNaN

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
