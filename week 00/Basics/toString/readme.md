 <h1>Explanation of the toString() Method in Java</h1>
    <p>The <code>toString()</code> method is a method that is available to all Java objects. It returns a string representation of the object.</p>
    <p>By default, the <code>toString()</code> method returns a string that contains the name of the object's class and its memory address. This is not very useful in most cases.</p>
    <p>However, you can override the <code>toString()</code> method in your own classes to provide a more useful string representation of the object. For example, you could define a <code>toString()</code> method in a <code>Person</code> class that returns the person's name and age:</p>
    <pre>
      <code>
public class Person {
  private String name;
  private int age;
public Person(String name, int age) {
this.name = name;
this.age = age;
}

@Override
public String toString() {
return "Person{name='" + name + "', age=" + age + "}";
}
}
</code>
</pre>
<p>Now, if you create a <code>Person</code> object and print it to the console, you will see the person's name and age instead of a meaningless string:</p>
<pre>
<code>
Person person = new Person("Alice", 25);
System.out.println(person); // prints "Person{name='Alice', age=25}"
</code>
</pre>
<p>Overriding the <code>toString()</code> method can be useful for debugging purposes, as well as for providing a meaningful string representation of your objects for other developers to use.</p>
