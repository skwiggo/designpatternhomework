I have chosen to look at the Singleton design pattern.

The Singleton design pattern means that the developer can only use one instantiation of an object within a class. For other classes to use the Singleton variable they have to 'get' a copy of the class from the class itself and they can only use that copy once. This means that they cannot call the class multiple times. 

There are some great benefits to this pattern. If you have a class that you do not want to make copies of - for instance registry data, sensitive information or a configuration that shouldn't be run more than once.

However the Singleton design pattern can create some large problems of its own. For example you cannot use subclasses with the Singleton method to extend its functionality - that is because the Singleton class is private. You could change it to public but then the program would not be technically 'Singleton' anymore.

It also could be argued that the Singleton design pattern violates the Single Responsibility precept of the SOLID methodology. By having only one instantiation of the Singleton class, the Singleton must hold responsibility over large sections of the program rather than just having one single responsibility. 

In conclusion - Singletons do have some valid uses and when used well can be a very useful design pattern for select situations. However it is no "one size fits all" pattern and if used lazily it can cause a myriad of issues within your programs. Therefore it should be used with care.



