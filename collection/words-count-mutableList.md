# Word count mutable List 

```kotlin
fun main() {
    val itemList = "Hello heLlo world"
    itemList.toLowerCase().split(" ")
		.groupingBy { it }
		.eachCount()
		.toList()
		.sortedByDescending {(key, value) -> value}
		.toMap()
		.map {
			println("${it.key}: ${it.value}")
		}
}
```
