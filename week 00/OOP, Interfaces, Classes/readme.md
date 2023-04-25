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
