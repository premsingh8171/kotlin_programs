# kotlin_programs]

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
  
 4. look the below code
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


5. ff
```kotlin
>     fun main() {
>     var greed: String = "Hello All"
>     greed = null
>     println(greed)
>     }

Null can not be a value of a non-null type String
> So the result will be Compile-Time Error
```
    
    
