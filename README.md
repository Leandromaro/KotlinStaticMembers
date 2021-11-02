# KotlinStaticMembers
## Kotlin How to create Static Members for class

Kotlin doesn’t have static member for class, it’s mean that you can’t create static method and static variable in Kotlin class.

Fortunately, Kotlin object can handle this. If you declare a companion object inside your class, you'll be able to call its members with the same syntax as calling static methods in Java/C#, using only the class name as a qualifier.
```
class MyClass { 
  companion object {
    val info = "This is info"    
    fun getMoreInfo():String { return "This is more fun" }
  } 
}
MyClass.info             // This is info
MyClass.getMoreInfo()    // This is more fun
```

