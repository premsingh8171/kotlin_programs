# Kotlin Programs

1. What will be the output?
```kotlin
>     class Sample{
>     fun add(a:Int, b:Int,sum:(Int, Int)->Int){
>     var res = sum(a,b)
>     println("Result is $res")
>     }
>     }
>     
>     fun main() {
>     var sample = Sample()
>         sample.add(6,8,{a,b -> a+b})   
>     }
> Output:Result is 14
```


2. What will be the output?
```kotlin
>     fun main() {
>     var nums = listOf<Int>(1,6,8,9,6,8)
>     nums[1] = 5
>     for(x int nums){
>      print(x)   
>     }
>     }

> Unresolved reference. None of the following candidates is applicable because of receiver type mismatch: public inline operator fun kotlin.text.StringBuilder /* = java.lang.StringBuilder */.set(index: Int, value: Char): Unit defined in kotlin.text
No set method providing array access
Expecting 'in'
Expecting ')'
Unexpected tokens (use ';' to separate expressions on the same line)
Unresolved reference: x
  
> **It means  result wil be Compile-Time Error**
```  

3. What will be the output?
```kotlin  
>      fun main() {
>     val words = listOf("kotlin", "cobol", "android", "pascal", "python", "swift", "flutter")
>     val byLenght = words.groupBy{it.length}
>     println(byLenght)
>     }

> Output:Result is  {6=[kotlin, pascal, python], 5=[cobol, swift], 7=[android, flutter]}
``` 
  
 4. Look the below code
```kotlin  
    >     var num1 = 3
>         outer@ while(num1>0){
>         var num2 = 3
>         inner@ while(num2>0){
>         if(num1 ==2)
>         // do one statement
>         //break@outer
>         println("num1 = $num1, num2 = $num2")
>         num2--
>         }
>         num1--
>         }
    
Which of the folowing options should be placed in Line 7 to get the below output?
 output: 
 num1 =3, num2=3
 num1 =3, num2=2
 num1 =3, num2=1
    
 Options:
 1. break
 2. break@outer
 3. break@inner
 4. Compiler-Time Error
```


5. What will be the output? when the below code is executed?

```kotlin
>     fun main() {
>     var greed: String = "Hello All"
>     greed = null
>     println(greed)
>     }

Null can not be a value of a non-null type String
> So the result will be Compile-Time Error
```

6. Which of the below Line number will cause a compile time error, when this code is executed?

```kotlin
> fun main() {
> val y: MyClass<Any> MyClass<String>("Harshini") //line 1 here
> val z: MyClass<String> MyClass<Any>(10.00)     //line 2
> } 
> class MyClass<out T>(val value: T)

After run this code we will get below error

Unexpected tokens (use ';' to separate expressions on the same line)
Unexpected tokens (use ';' to separate expressions on the same line)

```
7. What is the error of below code?

```kotlin
>     class Test: EmpData{}
>     object EmpData{}
>     fun main(args: Array<String>){
>     var sampleText = Test()
>     }

Result wil be get Cannot inherit from a singleton
```

8. What is the output of below code?
```kotlin
>     fun main(args: Array<String>){
>     var value = greater(16,81)
>     println(value)
>     }
>     
>     fun greater(a:Int, b:Int):Int = if(a>b){
>     println("$a is greater")
>     a
>     679
>     }else{
>     println("$b is greater")
>     b
>     123
>     }

Output: 
81 is greater
123

```
 
 9. What will be the output?
```kotlin
>     class Test : Exception()
>     fun main(args: Array<String>){
>     try{
>     throw Test()
>     }
>     catch(e: Exception){
>     println("Got the Test Exception")
>     }
>     finally{
>     println("Inside finally block")
>     }
>     }
    
Output:
Got the Test Exception
Inside finally block
```

10. What will be the output?

```kotlin
>     fun main(args: Array<String>){
>     var emp1 = Employee(12221, "Ramesh")
>     println("*****************************")
>     var emp2 = Employee(12343, "Arjun", "Chennai")
>     }
>     
>     class Employee(id:Long,name:String){
>     var eid:Long = 0
>     lateinit var ename:String
>     init{
>     println("Inside Init")
>     eid = 1223
>     ename = "Vimal"
>     println("Id is $eid and Name is $ename")
>     }
>     constructor(id:Long, name:String, dc:String):this(id, name){
>     println("Id is $id and Name is $name and DC is $dc")
>     }
>     }



Output:
Inside Init
Id is 1223 and Name is Vimal
*****************************
Inside Init
Id is 1223 and Name is Vimal
Id is 12343 and Name is Arjun and DC is Chennai
```

    
    
