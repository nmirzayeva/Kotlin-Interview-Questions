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


