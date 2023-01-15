# kotlin_programs]

1. What will be the output?
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


2. What will be the output?
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
  

3. What will be the output?
  
> >     fun main() {
>     val words = listOf("kotlin", "cobol", "android", "pascal", "python", "swift", "flutter")
>     val byLenght = words.groupBy{it.length}
>     println(byLenght)
>     }

> Output:Result is  {6=[kotlin, pascal, python], 5=[cobol, swift], 7=[android, flutter]}
