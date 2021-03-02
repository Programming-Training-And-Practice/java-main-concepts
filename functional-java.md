# Functional Java.





## Contents at a Glance.
* [About.](#about)
* [Documentation.](#documentation)
* [Stream](#stream)
* [Stream intermediate operations.](#stream-intermediate-operations)
* [Stream terminal operations.](#stream-terminal-operations)
* [When can you return Stream.](#when-can-you-return-stream)
* [Common mistakes made in Stream.](#common-mistakes-made-in-stream)
* [Lambda](#lambda)
* [Common mistakes made in Lambda.](#common-mistakes-made-in-lambda)
* [Help.](#help)





## About.





## Documentation.
* A stream can be defined as a sequence of data.





## Functional Expression.
* Java have two types of "functional expression":
  * Lambda.
  * Method reference.  





# Functional Interface.
* "Functional Interface" contains only one abstract method, the name of this method "single abstract method" or "sam"
* "Functional Interface" will inherit all methods from the "Object".
* "Functional Interface" can inherit other "Functional Interface".





# Some Functional Interface.
* Function<T,R>
* UnaryOperator<T>  
* Comparator<T>
  * pay attention to the contract of the "equals" method





# Stream.
* The stream cannot be used twice. You should not reuse Stream.
* The stream is lazy.
* The stream is not mutable.
* Order in operations is important.
* Look closely at the order of operations - prevent incorrect answers.
* Only use infinite streams when absolutely necessary. 
* When using orElse(x), make sure "x" doesn't contain any side effects.
* Only use orElse() to assign default value.
* Use orElseGet() to run alternative flow.




## Stream intermediate operations.
* filter()
* map()
* flatMap()
* distinct()
* sorted()
* peek()
* limit()
* skip()





## Stream terminal operations.
* toArray()
* collect()
* count()
* reduce()
* forEach()
* forEachOrdered()
* min()
* max()
* anyMatch()
* allMatch()
* noneMatch()
* findAny()
* findFirst()





## When can you return Stream.
* Private intermediate function.
* When new stream is created every time.
* When result is very large or might be infinite.
* By default return a collection.





## Common mistakes made in Stream.
* Be careful with returning Stream. And do not consume twice.
* A Stream is not a data structure.
* Overusing forEach.





## Lambda.
* Void-compatible (void SAM)
* Value-compatible (non-void SAM)
* capture value (closure)





## Method Reference.





## Common mistakes made in Lambda.
* Doing too much in single lambda.





## Links.
* [Лекция 7. Элементы функционального программирования на Java](https://www.youtube.com/watch?v=U10maNKqnXg&list=PLlb7e2G7aSpQith1Z6xRpU8jFPgkh_Gvz&index=7&ab_channel=ComputerScienceCenter)
* [Лекция 8. Stream API](https://www.youtube.com/watch?v=Pk7atYm8bX0&list=PLlb7e2G7aSpQith1Z6xRpU8jFPgkh_Gvz&index=8&ab_channel=ComputerScienceCenter)
* []()





## Help.
