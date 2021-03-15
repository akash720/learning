1. JDK generates the byte code for a given file with .java extension.

2. J2EE edition of java is used for developing web application.

3. For compiling a java code we have same compiler for every os.

4. We can call static method without using class name.

5.  A method with the same signature as a private final method in class X can be implemented in a subclass of X because private methods are not inherited.

6. If we declare a static block in java class, it is executed when class loads(even without creating an object) and it only executes once.

7. For primitive data types there's a default value whereas for reference datatype it is null.

8. "this" cannot be referenced from a static context.

9. There's no keyword "default"

10. All three parts of "for" loop are optional

11. In static methods, we can only access static members. But we can access non-static members by creating an object.

12.The wrapper class of all 8 primitive data types except "int" and "char" have same name as the data type with first letter capital.

13. Prior to java 5, there was no concept of AutoBoxing and Unboxing

14. Data is unwraped using the method XXXvalue() where XXX is the datatype.

15. The scanner methods other than nextLine() do not consume the "/n"(i.e., new line character). So we should place an extra nextLine() to consume the character otherwise if we scan for anything next, the "\n" character would also get scanned.

16. If a class has parametrized constructor alone, then compiler will not automatically create a default constructor.

17. It's not mandatory to write a default constructor along with paramterized constructor but if we try to create an object without any parameters then we would get compile error. Also, if we inherit this class then compiler will give error while making object of derived class because the compiler implicitly adds the super() in child class constructor.

18. Arrays for reference data types hold the address of the array elements.

19. If the array is an array of object, it sorts them in ascending order according to their natural ordering.

20. String Pool makes Java more memory efficient by not creating new object if a similar object exists.

21. "==" only works in case of strings created by String Pool.

22. super() and this() cannot be used together. 

23. Java 5.0 onwards it is possible to have different return type(here, class) for a overriding method in child class, but child’s return type should be sub-type of parent’s return type.

24. When a parent class reference holds a child class object, using that reference we can invoke the methods in the parent and also the overridden methods in child. To invoke child specific method downcasting needs to be done.  

```
// implicit upcasting
Parent p = new Child();
// explicit downcasting
Child c = (Child) p;
// explicit upcasting;
Parent p1 = (Parent) c;
```

25. Checked exception like IOException are not propogated automatically so we have to use throws keyword. In Java, exceptions under Error and RuntimeException classes are unchecked exceptions, everything else under throwable is checked.

26. Examples of checked exception are: FileNotFoundException, IOException, SQLException, ClassNotFoundException, etc.
Examples of unchecked exception are: NullPointerExc. , ArrayIndexOutOfBoundsExc., IllegalArgumentExc., Runtime exceptions, NumberFormatExc., ArithmeticExc., ClassCastExc., etc.

27. If we don't use break statement in switch case then all the cases after the matched case gets executed.

28. We can only downcast an object when that object is a superclass reference object containing a subclass object. Or we can say that we cannot downcast parent class object. Check this: https://ide.geeksforgeeks.org/CM2HFEG3Yl

29. https://www.decodejava.com/static-initialization-block-vs-instance-initialization-block.htm
