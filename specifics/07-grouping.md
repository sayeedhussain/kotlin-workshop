## Grouping

The Kotlin standard library provides extension functions for grouping collection elements. The basic function groupBy() takes a lambda function and returns a Map.

```kotlin
val numbers = listOf(1, 2, 3, 4, 5, 6)
println(numbers.groupingBy { if (it % 2 == 0) "odd" else "even" }.fold(0) {acc, element -> acc + element})
```
