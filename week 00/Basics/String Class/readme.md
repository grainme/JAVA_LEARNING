<h1>String Class && its Methods</h1>

<h3>Length</h3>
<p>To know the size of a string simply call the .length method over the string object</p>

<h3>Concatenate Two Strings</h3>
<p>Because the String objects are immutable we need to store ther return of .concat() in a variable!<br><code>String name = str1.concat(str2);</code></p>

<h3>Equals not ==</h3>
<p>To check whether two strings are equal or not, we can also use equalsIgnoreCase!<br><code>str1.equals(str2);</code></p>

<h3>indexOf</h3>
<p>To get the index of a character/string in a string
  <pre lang="java">
  <code>
  // Implementation
  str1 = "Marouane";
  str1.indexOf("rou"); // this should output ans = 2
  </code>
  </pre>
</p>
