ie-console-table
================

This is a way to provide polyfiling for IE browsers to use the console.table functionality that is given in modern web browsers such as [Firefox](https://developer.mozilla.org/en-US/docs/Web/API/Console.table) and [Chrome](https://developer.chrome.com/devtools/docs/tips-and-tricks#console-table). 

This allows us to view data in a table layout, takes . There is also an optional 'columns' parameter which takes the form of an array of strings similar to the Chrome console.table.

From the example given by Google Chrome:
<pre><code>function Person(firstName, lastName, age) {
  this.firstName = firstName;
  this.lastName = lastName;
  this.age = age;
}

var family = {};
family.mother = new Person("Susan", "Doyle", 32);
family.father = new Person("John", "Doyle", 33);
family.daughter = new Person("Lily", "Doyle", 5);
family.son = new Person("Mike", "Doyle", 8);

console.ietable(family, ["firstName", "lastName", "age"]);</code></pre>

We get:
<pre><code>index | firstName | lastName | age
mother | Susan | Doyle | 32
father | John | Doyle | 33
daughter | Lily | Doyle | 5
son | Mike | Doyle | 8 </code></pre>

Similar to:

[![google.PNG](https://d23f6h5jpj26xu.cloudfront.net/3jescrrmn6dt6a_small.png)](http://img.svbtle.com/3jescrrmn6dt6a.png)
