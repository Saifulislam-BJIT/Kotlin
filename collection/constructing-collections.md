# Initial function for list

```kotlin
val doubled = List(3, { it * 2 })  // or MutableList if you want to change its content later
println(doubled)
```

# Copy list

```kotlin
val alice = Person("Alice")
val sourceList = mutableListOf(alice, Person("Bob"))
val copyList = sourceList.toList()
sourceList.add(Person("Charles"))
alice.name = "Alicia"
println("First item's name is: ${sourceList[0].name} in source and ${copyList[0].name} in copy")
println("List size is: ${sourceList.size} in source and ${copyList.size} in copy")
```
