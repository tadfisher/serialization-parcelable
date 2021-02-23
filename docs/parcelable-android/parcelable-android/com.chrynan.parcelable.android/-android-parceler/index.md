//[parcelable-android](../../index.md)/[com.chrynan.parcelable.android](../index.md)/[AndroidParceler](index.md)



# AndroidParceler  
 [androidJvm] class [AndroidParceler](index.md)(**parcelable**: Parcelable)

A class bridging the serialization logic between the Parcelable interface in this library and the Android [android.os.Parcel](https://developer.android.com/reference/kotlin/android/os/Parcel.html) and [android.os.Parcelable](https://developer.android.com/reference/kotlin/android/os/Parcelable.html) interfaces.

   


## Constructors  
  
|  Name|  Summary| 
|---|---|
| <a name="com.chrynan.parcelable.android/AndroidParceler/AndroidParceler/#com.chrynan.parcelable.core.Parcelable/PointingToDeclaration/"></a>[AndroidParceler](-android-parceler.md)| <a name="com.chrynan.parcelable.android/AndroidParceler/AndroidParceler/#com.chrynan.parcelable.core.Parcelable/PointingToDeclaration/"></a> [androidJvm] fun [AndroidParceler](-android-parceler.md)(parcelable: Parcelable)   <br>


## Functions  
  
|  Name|  Summary| 
|---|---|
| <a name="com.chrynan.parcelable.android/AndroidParceler/createFromParcel/#android.os.Parcel#kotlin.reflect.KClass[TypeParam(bounds=[kotlin.Any])]/PointingToDeclaration/"></a>[createFromParcel](create-from-parcel.md)| <a name="com.chrynan.parcelable.android/AndroidParceler/createFromParcel/#android.os.Parcel#kotlin.reflect.KClass[TypeParam(bounds=[kotlin.Any])]/PointingToDeclaration/"></a>[androidJvm]  <br>Content  <br>fun <[T](create-from-parcel.md) : [Any](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)> [createFromParcel](create-from-parcel.md)(source: [Parcel](https://developer.android.com/reference/kotlin/android/os/Parcel.html), kClass: [KClass](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.reflect/-k-class/index.html)<[T](create-from-parcel.md)>): [T](create-from-parcel.md)  <br>More info  <br>Retrieves the value of [T](create-from-parcel.md) represented by the provided kClass from the underlying [android.os.Parcel](https://developer.android.com/reference/kotlin/android/os/Parcel.html) using the parcelable instance.  <br><br><br>
| <a name="com.chrynan.parcelable.android/AndroidParceler/describeContents/#TypeParam(bounds=[kotlin.Any?])/PointingToDeclaration/"></a>[describeContents](describe-contents.md)| <a name="com.chrynan.parcelable.android/AndroidParceler/describeContents/#TypeParam(bounds=[kotlin.Any?])/PointingToDeclaration/"></a>[androidJvm]  <br>Content  <br>fun <[T](describe-contents.md)> [describeContents](describe-contents.md)(value: [T](describe-contents.md)): [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)  <br>More info  <br>Retrieves the hashCode for the provided value used to describe it's contents in the underlying [android.os.Parcel](https://developer.android.com/reference/kotlin/android/os/Parcel.html).  <br><br><br>
| <a name="kotlin/Any/equals/#kotlin.Any?/PointingToDeclaration/"></a>[equals](index.md#%5Bkotlin%2FAny%2Fequals%2F%23kotlin.Any%3F%2FPointingToDeclaration%2F%5D%2FFunctions%2F784558222)| <a name="kotlin/Any/equals/#kotlin.Any?/PointingToDeclaration/"></a>[androidJvm]  <br>Content  <br>open operator fun [equals](index.md#%5Bkotlin%2FAny%2Fequals%2F%23kotlin.Any%3F%2FPointingToDeclaration%2F%5D%2FFunctions%2F784558222)(other: [Any](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)?): [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)  <br><br><br>
| <a name="kotlin/Any/hashCode/#/PointingToDeclaration/"></a>[hashCode](index.md#%5Bkotlin%2FAny%2FhashCode%2F%23%2FPointingToDeclaration%2F%5D%2FFunctions%2F784558222)| <a name="kotlin/Any/hashCode/#/PointingToDeclaration/"></a>[androidJvm]  <br>Content  <br>open fun [hashCode](index.md#%5Bkotlin%2FAny%2FhashCode%2F%23%2FPointingToDeclaration%2F%5D%2FFunctions%2F784558222)(): [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)  <br><br><br>
| <a name="com.chrynan.parcelable.android/AndroidParceler/newArray/#kotlin.Int/PointingToDeclaration/"></a>[newArray](new-array.md)| <a name="com.chrynan.parcelable.android/AndroidParceler/newArray/#kotlin.Int/PointingToDeclaration/"></a>[androidJvm]  <br>Content  <br>fun <[T](new-array.md) : [Any](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)> [newArray](new-array.md)(size: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)): [Array](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-array/index.html)<[T](new-array.md)?>  <br>More info  <br>Retrieves a new empty array for type [T](new-array.md).  <br><br><br>
| <a name="kotlin/Any/toString/#/PointingToDeclaration/"></a>[toString](index.md#%5Bkotlin%2FAny%2FtoString%2F%23%2FPointingToDeclaration%2F%5D%2FFunctions%2F784558222)| <a name="kotlin/Any/toString/#/PointingToDeclaration/"></a>[androidJvm]  <br>Content  <br>open fun [toString](index.md#%5Bkotlin%2FAny%2FtoString%2F%23%2FPointingToDeclaration%2F%5D%2FFunctions%2F784558222)(): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)  <br><br><br>
| <a name="com.chrynan.parcelable.android/AndroidParceler/writeToParcel/#TypeParam(bounds=[kotlin.Any])#android.os.Parcel#kotlin.reflect.KClass[TypeParam(bounds=[kotlin.Any])]/PointingToDeclaration/"></a>[writeToParcel](write-to-parcel.md)| <a name="com.chrynan.parcelable.android/AndroidParceler/writeToParcel/#TypeParam(bounds=[kotlin.Any])#android.os.Parcel#kotlin.reflect.KClass[TypeParam(bounds=[kotlin.Any])]/PointingToDeclaration/"></a>[androidJvm]  <br>Content  <br>fun <[T](write-to-parcel.md) : [Any](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)> [writeToParcel](write-to-parcel.md)(value: [T](write-to-parcel.md), dest: [Parcel](https://developer.android.com/reference/kotlin/android/os/Parcel.html), kClass: [KClass](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.reflect/-k-class/index.html)<[T](write-to-parcel.md)>): Parcel  <br>More info  <br>Writes the provided value, represented by the provided kClass, to the [dest](https://developer.android.com/reference/kotlin/android/os/Parcel.html) using the parcelable instance.  <br><br><br>


## Extensions  
  
|  Name|  Summary| 
|---|---|
| <a name="com.chrynan.parcelable.android//createFromParcel/com.chrynan.parcelable.android.AndroidParceler#android.os.Parcel/PointingToDeclaration/"></a>[createFromParcel](../create-from-parcel.md)| <a name="com.chrynan.parcelable.android//createFromParcel/com.chrynan.parcelable.android.AndroidParceler#android.os.Parcel/PointingToDeclaration/"></a>[androidJvm]  <br>Content  <br>inline fun <[T](../create-from-parcel.md) : [Any](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)> [AndroidParceler](index.md).[createFromParcel](../create-from-parcel.md)(source: [Parcel](https://developer.android.com/reference/kotlin/android/os/Parcel.html)): [T](../create-from-parcel.md)  <br>More info  <br>A reified convenience function for [AndroidParceler.createFromParcel](create-from-parcel.md).  <br><br><br>
| <a name="com.chrynan.parcelable.android//decodeFromBundle/com.chrynan.parcelable.android.AndroidParceler#android.os.Bundle#kotlin.Int/PointingToDeclaration/"></a>[decodeFromBundle](../decode-from-bundle.md)| <a name="com.chrynan.parcelable.android//decodeFromBundle/com.chrynan.parcelable.android.AndroidParceler#android.os.Bundle#kotlin.Int/PointingToDeclaration/"></a>[androidJvm]  <br>Content  <br>inline fun <[T](../decode-from-bundle.md) : [Any](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)> [AndroidParceler](index.md).[decodeFromBundle](../decode-from-bundle.md)(bundle: [Bundle](https://developer.android.com/reference/kotlin/android/os/Bundle.html), flags: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html) = 0): [T](../decode-from-bundle.md)?  <br><br><br>[androidJvm]  <br>Content  <br>fun <[T](../decode-from-bundle.md) : [Any](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)> [AndroidParceler](index.md).[decodeFromBundle](../decode-from-bundle.md)(bundle: [Bundle](https://developer.android.com/reference/kotlin/android/os/Bundle.html), kClass: [KClass](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.reflect/-k-class/index.html)<[T](../decode-from-bundle.md)>, flags: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html) = 0): [T](../decode-from-bundle.md)?  <br>More info  <br>Retrieves a value of [T](../decode-from-bundle.md) of kClass from the provided bundle and flags, or null if the bundle is empty or  <br><br><br>
| <a name="com.chrynan.parcelable.android//encodeToBundle/com.chrynan.parcelable.android.AndroidParceler#TypeParam(bounds=[kotlin.Any])/PointingToDeclaration/"></a>[encodeToBundle](../encode-to-bundle.md)| <a name="com.chrynan.parcelable.android//encodeToBundle/com.chrynan.parcelable.android.AndroidParceler#TypeParam(bounds=[kotlin.Any])/PointingToDeclaration/"></a>[androidJvm]  <br>Content  <br>inline fun <[T](../encode-to-bundle.md) : [Any](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)> [AndroidParceler](index.md).[encodeToBundle](../encode-to-bundle.md)(value: [T](../encode-to-bundle.md)): [Bundle](https://developer.android.com/reference/kotlin/android/os/Bundle.html)  <br><br><br>[androidJvm]  <br>Content  <br>fun <[T](../encode-to-bundle.md) : [Any](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)> [AndroidParceler](index.md).[encodeToBundle](../encode-to-bundle.md)(value: [T](../encode-to-bundle.md), kClass: [KClass](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.reflect/-k-class/index.html)<[T](../encode-to-bundle.md)>): [Bundle](https://developer.android.com/reference/kotlin/android/os/Bundle.html)  <br>More info  <br>Writes the provide value of kClass into a [Bundle](https://developer.android.com/reference/kotlin/android/os/Bundle.html) and returns it.  <br><br><br>
| <a name="com.chrynan.parcelable.android//newArrayInline/com.chrynan.parcelable.android.AndroidParceler#kotlin.Int/PointingToDeclaration/"></a>[newArrayInline](../new-array-inline.md)| <a name="com.chrynan.parcelable.android//newArrayInline/com.chrynan.parcelable.android.AndroidParceler#kotlin.Int/PointingToDeclaration/"></a>[androidJvm]  <br>Content  <br>inline fun <[T](../new-array-inline.md) : [Any](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)> [AndroidParceler](index.md).[newArrayInline](../new-array-inline.md)(size: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)): [Array](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-array/index.html)<[T](../new-array-inline.md)?>  <br>More info  <br>A reified convenience function for [AndroidParceler.newArray](new-array.md).  <br><br><br>
| <a name="com.chrynan.parcelable.android//writeToParcel/com.chrynan.parcelable.android.AndroidParceler#TypeParam(bounds=[kotlin.Any])#android.os.Parcel/PointingToDeclaration/"></a>[writeToParcel](../write-to-parcel.md)| <a name="com.chrynan.parcelable.android//writeToParcel/com.chrynan.parcelable.android.AndroidParceler#TypeParam(bounds=[kotlin.Any])#android.os.Parcel/PointingToDeclaration/"></a>[androidJvm]  <br>Content  <br>inline fun <[T](../write-to-parcel.md) : [Any](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)> [AndroidParceler](index.md).[writeToParcel](../write-to-parcel.md)(value: [T](../write-to-parcel.md), dest: [Parcel](https://developer.android.com/reference/kotlin/android/os/Parcel.html)): Parcel  <br>More info  <br>A reified convenience function for [AndroidParceler.writeToParcel](write-to-parcel.md).  <br><br><br>
