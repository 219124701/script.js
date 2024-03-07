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



