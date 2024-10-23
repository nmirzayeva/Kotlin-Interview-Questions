<div style="text-align: center;">
  <img src="https://github.com/user-attachments/assets/fc6c90c8-e7b2-4266-85f3-5d0fc7199122" alt="Kotlin" style="width: 80%; max-width: 600px;"/>
     </div>

## 1. **Difference Between `val` and `const val`**
`const val` assigns a value at compile-time, whereas `val` assigns a value at runtime. `const val` is advantageous when defining a constant value because it resolves the assignment during the compile phase, thus avoiding the need for runtime assignment.

## 2. **When to Use `!!` and `?.` Operators**
We use `!!` when we are certain that a nullable variable is not null. In cases where we are not sure if a variable is null or when it being null is not critical, we use `?.`.

## 3. **Variable Declaration Without Type and Null Value**
In Kotlin, if a variable is declared without a type and is initially assigned a null value, the variable’s type automatically becomes `Nothing?`.

## 4. **Meaning and Usage of the `Nothing` Type**
The `Nothing` type in Kotlin represents a type that has no value. `Nothing?` is the nullable version of this type, meaning the variable can be either `Nothing` or `null`.

## 5. **Usage of the Elvis Operator**
The Elvis operator `?:` is used for null safety. The expression on the left side of `?:` is executed if it is not null; otherwise, the expression on the right side (the default scenario) is executed. For example: 
```kotlin
val result = nullableValue ?: defaultValue
```
## 6. **Difference Between `Double` and `Float`**
`Double` is used for larger floating-point numbers, while `Float` is used for smaller floating-point numbers. The memory consumption varies accordingly:
- `Float` is **32-bit** (4 bytes) and has approximately **7 decimal digits** of precision.
- `Double` is **64-bit** (8 bytes) and has approximately **15-16 decimal digits** of precision.

We use `Float` when the number size is suitable, and we want to save memory.

## 7. **What are boxed and unboxed variables**
Boxing refers to storing a variable as an object, while unboxing refers to storing it as a primitive type. In Kotlin, even if it seems like we are creating an `Int` object, it is automatically cast to a primitive `int` type in the Java bytecode.

## 8. **Are smaller numeric types subclasses of larger numeric types in Kotlin? For instance, is `Byte` a subclass of `Short`, and Short a subclass of `In`t**

In Kotlin, smaller numeric types are not subclasses of larger numeric types. Instead, all numeric types (`Byte`, `Short`, `Int`, `Long`, `Float`, `Double`) are subclasses of the Number class. Therefore, the answer is no; all numeric types share the common superclass Number.

## 9. **What happens if I add a `Long` number to an `Int` number**

The sum of a `Long` and an `Int` will be of type `Long`. The larger type (`Long`) determines the type of the result.

## 10. **What happens if you compare the numbers 2 and 2.5 using `==`**
```kotlin
fun main() {

    val a :Number= 2
    val b : Number = 2.5f

    println(a==b)
}
```
Comparing the numbers 2 and 2.5 using `==` will return false because 2 and 2.5 are not equal.



