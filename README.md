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
