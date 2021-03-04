# My personal OCP 1z0819 notes preparation notes

## Exam Preparation Resources

### Books

- [OCP Oracle Certified Professional Java SE 11 Programmer I Study Guide: Exam 1Z0-815 1st Edition by Jeanne Boyarsky
  ](https://amzn.to/38L87ez)

- [OCP Oracle Certified Professional Java SE 11 Programmer II Study Guide: Exam 1Z0-816 and Exam 1Z0-817 1st Edition
  ](https://amzn.to/3bHa6Cr)

### Additionals

- #### Video Materials
  - [Java SE 11 Developer 1Z0-819 OCP Course - Part 1 by Tim Buchalka](https://www.udemy.com/course/java-se-11-developer-1z0-819-ocp-course-part-1/)

### Notes

- **var** declaration is allowed only inside method body and for loop declarations. It is not allowed to declareclass/instance fields, method parameters, or method return types.
- **Function<T,R>** is a functional interface whose functional method is **_apply(Object)_**. If you have a method that expects this function, for example: void myMethod(Function< Integer, String> f){   ... } it can be invoked like this: myMethod( i -> "create some string here" );
- Class Initialization order:
  1. All static constants, variables, and blocks.
  2. All non static constants, variables, and blocks.
  3. Constructor.
- Static method cannot be overridden by a non-static method and vice versa.
- If there is no package statement in the source file, the class is assumed to be created in an unnamed package that has no name. In this case, all the types created in this package will be available to this class without any import statement.
- Since Integer is a subtype of Number, List< Integer > is a subtype of List<? extends Integer> and List<? extends Integer> is a subtype of List<? extends Number>. Thus, if an overridden method returns List<? extends Integer>, the overriding method can return List < Integer > but not List< Number > or List<? extends Number>.
- Primitives are always passed by value.
- Java 11 has a new feature called the "Single-File Source-Code program".  This feature allows executing your Java source code directly using the java interpreter. The source code is compiled in memory and then executed by the interpreter. The limitation is that all the classes have to be defined in the same file. The class to be executed is the first top-level class found in the source file. It must contain a declaration of the standard main method.
- A superclass object can never be assigned to a base class reference.

  ```java
  Plant p = new Sunflower(); //Valid

  Sunflower s = new Plant(); // Doesnt compile
  ```

-
