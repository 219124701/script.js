# script.js
# week1 to 5 
Introduction to Java Script

We have 8 concepts that we will be focusing on : 
1. We have variables and Data Types : variables in JavaScript you declare variables using 'var','let', or 'const'. 'var' has function scope , while 'let' and 'const' have block scope. While 'let' and 'const' have block scope.
2. DATA TYPES : javaScript suports various data types including numbers , strings, booleans , arrays, objects,functions and more.
3. FUNCTIONS: Are blocks of reusable code that perform a specific task. They can be declared using the 'FUNCTION' keyword as a arrow functions ('()=>{}').
4. Functions can take parameters and return values . They can also be assigned to variables and passed as arguments to other functions (higher order functions).

5. HOW TO ADD A COMMENT ON JAVA SCRIPT: you can add comments to your code to provide explainations, documentation, or to temporarily disabled code. There are two main ways to add comments: Single-line comments : use '//' to add comments that span single line. below its how to add comment:
  // This is a single-line comment
let x = 5; // This comment explains the purpose of the variable x

MMULTI-LINE COMMENTS : Enclose comments within '/* */' to create multi-line comments. 
/* This is a multi-line comment
   that spans multiple lines */
let y = 10;

Here are some best practices for using comments in JavaScript:

Be descriptive: Write comments that explain the purpose of the code, especially if it's not immediately obvious from the code itself.
Avoid unnecessary comments: Comments should add value to the code by providing insights or explanations that are not self-evident.

Update comments: Remember to update comments when you modify the code to keep them accurate and relevant.
Use comments sparingly: Write code that is self-explanatory and easy to understand without relying too heavily on comments.

# day 4 
JAVA SCRIPT VARIABLES :JAVASCRIPT WORK WITH THREE PRIMITIVE DATA TYPES : 
NUMBERS: E.G 123,120.50 , etc.
STRINGS of text e.g "This text string" etc 
BOOLEAN E.G. TRUE OR FALSE 
JAVASRCIPT also defines two trivial data types, NULL and undefined , each of which defines only a single value. in addition to those primitive data types, also JAVASCRIPT does not does not make a distinction between intern=ger values and floating point values . All numbers in javascript are represented as floating point values.

JAVASCRIPT has variables , Variables can be thought of as named containers . You can place data into these containers and then refer to the data simple by naming the container. JS vaviables needs to be declared with the var keyword as follows: 
<script type = "text/javascript"> 
  <!--
    var money ;
    var name;
  //-->
</script>

you can also declare multiple variables with the same var keyword as follows- 
<script type= "text/javascript>
  <!--
  var money,name;
  </script>

  THIS IS HOW YOU CREATE A VARIABLE NAMED MONEY AND ASSIGN THE VALUE 2000.50 TO IT , YOU CAN ASSIGN A VALUE AT THE TIME OF INITIALIZATION AS FOLLOWS: 
  <script type ="text/javascript">
    <!--
      var nam ="Okuhle"
    var money;
    money=2000.50,

      Java is an untyped language it means that javascript variable can hold a value of any data type , you dont have to tell have to javascript during a variable declaration what type of value the variable will hold.

  # WEEK2 
    # DAY2
    WEB DESIGN

    CALLIG ONE FUNCTION FROM ANOTHER FUNCTION
Function Definition: You define multiple functions, each with a specific task to perform.

Function Calls: Within one function, you can call another function to execute its task. This can be done using the function name followed by parentheses, optionally passing any required arguments.

Chaining Functions: By nesting function calls within each other, you can create a sequence of actions. The output of one function can serve as input for another function, allowing you to build more complex processes

    // Define three functions, each returning a string
function function1() {
    return "Hello";
}

function function2() {
    return "world!";
}

function function3() {
    return " How are you?";
}

// Define a main function that calls the three functions and concatenates their results
function mainFunction() {
    var result1 = function1();
    var result2 = function2();
    var result3 = function3();
    var finalResult = result1 + " " + result2 + result3;
    return finalResult;
}

// Call the main function and print the result
console.log(mainFunction()); // Output: Hello world! How are you?

  CREATING OBJECTS WITH USER-DEFINED FUNCTIONS:

    To create objects with user-defined functions in JavaScript, you can use constructor functions or ES6 class syntax. Constructor functions are traditional and widely used, while ES6 classes provide syntactic sugar over constructor functions. Here's how you can create objects using both approaches:

    
// Define a constructor function
function Person(name, age) {
    this.name = name;
    this.age = age;
}

// Add methods to the prototype of the constructor function
Person.prototype.greet = function() {
    return "Hello, my name is " + this.name + " and I am " + this.age + " years old.";
}

// Create instances of the Person object using the 'new' keyword
var person1 = new Person("John", 30);
var person2 = new Person("Alice", 25);

// Call methods on the objects
console.log(person1.greet()); // Output: Hello, my name is John and I am 30 years old.
console.log(person2.greet()); // Output: Hello, my name is Alice and I am 25 years old.

 OPERATORS 
1. Assignment operators
2. Comparison operator
3. Arithmetic operator
4. Bitwise operator
5. logical opereators
6. String
7. Conditional operator


    # WEEK 2
    #DAY 3

      JAVASCRIPT METHODS AND THIS KEYWORD:
In JavaScript, the this keyword refers to the object that is currently executing the code. It provides a way to access properties and methods of the current object within a function or method. Understanding how this works is essential for object-oriented programming and for working with JavaScript methods.In JavaScript, methods are functions that are associated with objects. They are defined within the context of an object and are accessed using dot notation.

Example:

const person = {
  firstName: 'John',
  lastName: 'Doe',
  fullName: function() {
    return this.firstName + ' ' + this.lastName;
  }
};

console.log(person.fullName()); // Outputs: John Doe

      
    JAVA EMAIL VALIDATION CODE EXPLAINED:
    
Email validation is a crucial part of form validation, as it ensures that the email address provided by the user conforms to a certain format. While it's impossible to fully validate an email address using only JavaScript (the only sure way is to send a verification email), you can perform basic checks to ensure that the email address has a reasonable format.

   function validateEmail(email) {
  var re = /\S+@\S+\.\S+/; // Regular expression pattern for basic email format
  
  return re.test(email); // Returns true if the email matches the pattern, false otherwise
}
    

    
    

    
    
    
    

      



