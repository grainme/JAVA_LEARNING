<h1> What does OOP means?</h1>
<p>OOP refers to languages that use ojects in programming. The aim of <strong>OOP</strong>
  is to to bind together the data and the functions that operate on them so that no other part of   the code can access this data except that function</p>
<h2>Access Modifier</h2>
<p>There are 4 types of access specifiers in JAVA</p>
<ol>
  <li>Public : Accessible in all classes in your application</li>
  <li>Protected : Accessible within the same package or subclasses in different packages. </li>
  <li>Private : Accessible only within the class in which it is defined. </li>
  <li>default : I don't care about this one!</li>
</ol>

<h2>Abstraction</h2>
<p>Data abstraction is basically hiding the non essential data from the user.<br>
Ex : A car is viewed as a car rather than its individual components.<br>
In <strong>JAVA</strong>, Abstraction is achieved using Interfaces and abstract classes. The abstract method contains only method declaration but not implementation.</p>

```java
abstract class Hello{
  //abstract methods declaration
  abstract void hi();
  abstract void hello();
  abstract void welcome();
}
```

<h2>Encapsulation</h2>
<p>It is similar to data-hiding, it's like a shield that prevents data being accessed by non owners!<br>
Encapsulation can be achieved by declaring all the variables in a class as private and then writing public methods in the class to set and get the values of the variables.</p>

```java
class Person {
    private String name;
    private int age;
 
    public String getName() { return name; }
 
    public void setName(String name) { this.name = name; }
 
    public int getAge() { return age; }
 
    public void setAge(int age) { this.age = age; }
}
 
public class Main {
    public static void main(String[] args)
    {
        Person person = new Person();
        person.setName("John");
        person.setAge(30);
 
        System.out.println("Name: " + person.getName());
        System.out.println("Age: " + person.getAge());
    }
}
```

<h2>Inheritance</h2>
<p>It is the mechanism in Java by which one class can inherit the features of another class, and this is pretty useful when it come to avoiding redundancy.<br>
  <li>Superclass : The class whose features are inherited.</li>
  <li>Subclass : The class that inherits the other class, it can have its own methods in addition to the superclass methods and variables..</li>
  <li>Reusability : Inheritance supports the concept of “reusability”, i.e. when we want to create a new class and there is already a class that includes some of the code that we want, we can derive our new class from the existing class.</li>
</p>

```java
//base class or parent class or super class
class A{
  //parent class methods
  void method1(){}
  void method2(){}
}
  
//derived class or child class or base class
class B extends A{  //Inherits parent class methods
  //child class methods
  void method3(){}
  void method4(){}
}
```

<h2>Polymorphisme</h2>
<p>It is the ability of OOP languages to differentiate between entities with the same name efficiently. This is done by JAVA with the help of the signature and declaration of these entities. The ability to appear in different form called polymorphism.<br>
There are two kinds of Polymorphism (mainly in java) : <br>
<li>Overloading : when using for example the same name for different methods but with different parametres.</li>
<li>Overriding : when we redefine already defined methods (like toString) and change their behavior (implement a new body).</li>
</p>

```java
    public int sum(int x, int y)
    {
        return (x + y);
    }
    public int sum(int x, int y, int z)
    {
        return (x + y + z);
    }
```




















