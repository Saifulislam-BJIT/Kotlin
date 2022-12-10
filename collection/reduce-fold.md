# Reduce and Fold

```kotlin
fun main() {
    val itemList = listOf(1, 2, 3, 4, 5)
    println(itemList.sum())
    println(itemList.sumOf{it*3})
    print("reduce ")
    println(itemList.reduce{ sum, item -> sum + item})
    print("fold ")
    println(itemList.fold(10) { sum, item -> sum + item})
    print("fold right: ")
    println(itemList.foldRight(10) { sum, item -> sum + item})
}
```
