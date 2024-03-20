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

# WEEK 3
# DAY1

 STRINGS OPERATIONS
     Strings can created as primitives from string literals or as objects,using the strings() consructor e.g 
    const string1 = "A string primitive";
    const string2 = "Also a string primitive";
    const string3 = "Yet another string primitive";
    const string4 = new String ("A string object";

    THE ONCLICK EVENT
    
    The Onclick Event is the most frequently used event types which occur when a user clicks the left button of his mouse.

The onclick event in JavaScript is a type of event that occurs when a user clicks on an HTML element, such as a button, link, or image. It is one of the most commonly used event handlers in web development for adding interactivity to web pagOverall, the onclick event provides a simple yet powerful mechanism for adding interactive behavior to web pages. It allows developers to respond to user actions, such as clicks, taps, or touches, and create engaging and dynamic user experiences.

  THE ONSUBMIT EVENT :
    
The onsubmit event in JavaScript is an event that occurs when a form is submitted by the user. It is commonly used to handle form submission in web applications and allows developers to perform actions such as form validation, data processing, or sending form data to a server.

Here's a clear explanation of how the onsubmit event works:

Form Submission: When a user submits a form by clicking on the submit button or by pressing the Enter key while focused on a form input field, the browser generates a submit event for the form.

Event Handling: If an event handler function is registered for the onsubmit event of the form element, this function is executed when the form is submitted. The event handler function contains the code or instructions that should be performed before or after the form is submitted.

Function Execution: Inside the event handler function, you can write JavaScript code to perform various tasks or actions related to form submission. Common tasks include form validation (checking if the entered data is valid), data processing (formatting or manipulating form data), and submitting the form data to a server (via AJAX or by redirecting to a new page).

Preventing Default Behavior: In some cases, you may want to prevent the default behavior of the form submission, such as preventing the page from reloading or navigating to a new page. You can achieve this by calling the preventDefault() method on the event object passed to the event handler function.

Form Validation: Form validation is a common use case for the onsubmit event. You can validate form fields to ensure that the user has entered valid data before allowing the form to be submitted. If validation fails, you can display error messages to the user and prevent the form from being submitted until the data is corrected.

Overall, the onsubmit event provides a powerful mechanism for handling form submission in web applications. It allows developers to customize the behavior of form submission and perform additional actions as needed, making web forms more interactive and user-friendly.

  EVENT HANDLERS
    
Event handlers in programming are functions that are executed in response to specific events occurring within an application or environment. These events could be triggered by user actions, such as clicking a button, hovering over an element, typing on a keyboard, or by system events like the completion of a file download.

Definition: An event handler is a function that is designed to respond to a particular event. It "listens" for the event to occur and then executes its associated code when the event is triggered.

  Overall, event handlers play a crucial role in creating interactive and dynamic user interfaces in web development and other software applications. They allow developers to respond to user interactions and system events, enabling rich and engaging user experiences.
  
MULTI-PARAMETER FUNCTION CODING

Multi-parameter coding involves writing functions or methods in programming languages that can accept multiple parameters. Parameters are variables passed into a function, providing input data for the function to operate on. This practice allows for flexible and reusable code, as functions can handle different types and quantities of data. It's a fundamental aspect of programming, enabling developers to create modular and efficient solutions for various tasks.
  
  THIS IS AN EXAMPLE OF A MULTTI-PARAMETER CODING:

  // Function to calculate the area of a rectangle
function calculateRectangleArea(width, height) {
    return width * height;
}

// Calling the function with two arguments (width and height)
var area = calculateRectangleArea(5, 3);
console.log("Area of the rectangle:", area); // Output: Area of the rectangle: 15

# DAY 2 
    DYNAMIC JAVASCRIPT TECHNIQUES:
    DYNAMIC AND STARTIC 

   - STARTIC - rendering happens in Browser higher reactivity but data needs to be fetch after initial rendering.
 - Security can be more complex   

  DYNAMIC- Rendering happens on Server Finished page is served but needs to be generated first.
  - Security needs to be easier. 

    DATA OBJECT:
The Date object in JavaScript is used to work with dates and times. It provides methods for creating, manipulating, and formatting dates and times. The Date object is a built-in object in JavaScript that stores the date and time. It provides a number of built-in methods for formatting and managing that data. 

 THIS IS HOW TO CREATE DATE OBJECT:
  // Current date and time
var currentDate = new Date();

// Specifying date and time components
var specificDate = new Date(2022, 0, 1, 12, 0, 0); // January 1, 2022, 12:00:00 PM

 INTRODUCTION TO DAY 3  

    KEYBOARD EVENTS: There are three keyboard events the keydown event, which is triggered when the key is pressed down on a keyboard. then keyup event that, is triggered when the key is released on the keyboard. last but not least we have the keypress event occurs when the key is pressed down on a keyboard that has the character associated with it.

  FORM EVENTS:

    Form events in JavaScript are events that occur when a user interacts with HTML form elements. These events allow you to perform actions such as validating user input, submitting form data, and updating the UI based on user actions. Here's a brief explanation of commonly used form events:
      
submit: Occurs when a form is submitted, either by clicking the submit button or pressing Enter while focused on a form field. Useful for form validation and data submission.

reset: Occurs when a form is reset, either by clicking the reset button or programmatically calling the reset() method. Useful for clearing form fields or resetting form state.

focus: Occurs when an element receives focus, typically when a user clicks on or tabs into an input field. Useful for providing visual cues or displaying help text.

blur: Occurs when an element loses focus, typically when a user clicks outside of an input field or tabs to another element. Useful for validating user input or triggering actions based on focus change.

change: Occurs when the value of an input field changes, such as typing in a text field or selecting an option from a dropdown menu. Useful for real-time validation or updating the UI based on user input.

input: Similar to the change event, but triggered immediately as the value changes, often with each keystroke. Useful for real-time validation or providing feedback as the user types.

keydown, keyup: Occur when a key is pressed or released while focused on an input field. Useful for implementing keyboard shortcuts or navigating through form fields.

keypress: Occurs when a key that produces a character is pressed while focused on an input field. Useful for handling text input.

These events enable you to create interactive and responsive forms in web applications, enhancing the user experience and providing feedback to users as they interact with form elements.

  DOCUMENT/WINDOW EVENTS:

 The load Event (onload)
    
  The load event occurs when a web page has finished loading in the web browser. You can handle the load event with the onload event handler. The following example will show you an alert message as soon as the page finishes loading.
    
    ![image](https://github.com/219124701/script.js/assets/158051727/c23071ab-21b1-404f-bd16-6f025dabac87)


THE UNLOAD EVENT (onunload)

    The unload event occurs when a user leaves the current web page. You can handle the unload event with the onunload event handler.
      
      ![image](https://github.com/219124701/script.js/assets/158051727/45aba35c-97fd-43b4-a359-4d38586a9be1)

 THE RESIZE EVENT (onresize):

    The resize event occurs when a user resizes the browser window. The resize event also occurs in situations when the browser window is minimized or maximized. You can handle the resize event with the onresize event handler.

    ![image](https://github.com/219124701/script.js/assets/158051727/a8b3667c-b0f7-4ab0-9ecf-107a3ce5e67c)

    
    
    

    
    

    
    

    

    




    
    
      

      
    
    
    

    
    

    
    

    
    
    
    

      



