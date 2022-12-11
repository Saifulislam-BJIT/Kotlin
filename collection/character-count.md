# Character Count

```kotlin
val msg = "hello hello hello world"
println(msg.split("").filter{it!="" && it!=" "}.groupingBy { it }.eachCount())
```
