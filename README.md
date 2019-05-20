presentation-Q3-2019
Hi! My name is Alesia Zharnasek
Today I will talk about TypeScript
---------Slide – TypeScript
-Superset of JavaScript
-Compiles to EcmaScript
-don’t need special runtime

In short: it is Lightweight productivity booster
-------Slide – Begin
Based on the Stack Overflow Developer survey in 2019, TypeScript is more "loved" as a programming language than JavaScript. The reason TypeScript is so loved amongst JavaScript developers is because adding types to JavaScript allows you to spot errors before running your code. The errors provided by the TypeScript compiler will give a good indication of how an error can be fixed. Adding types to JavaScript also allows code editors to provide some more advanced features, such as code completion, project-wide refactoring, and automatic module importing.
---------Slide -What is TypeScript
Helps in large scale JavaScript application development.
Adds additional features like Static Type (optional), Class, Module etc (that are not present in JavaScript) to JavaScript.
Starts with JavaScript, ends with JavaScript. We can say that TypeScipt is JavaScript. Any valid .js file can be renamed .ts and compiled with other TypeScript files.
TypeScript purposefully borrows ideas from EcmaScript 6 (ES6 Harmony) spec – class, module.
The compiler is an open source project and Runs on Any browser, Any host, Any OS.

-------Slide –How it worked
Installing Typescript
Writing code in Text Editors
Compiling to JavaScript

------Slide – Lets started
Let’s get started by building a simple web application with TypeScript.
INSTALLING TYPESCRIPT
There are two main ways to get the TypeScript tools:

- Via npm (the Node.js package manager) / yarn add typescript
- or By installing TypeScript’s Visual Studio plugins.
  The easiest way to setup TypeScript is via npm. Using the command below we can install the TypeScript package globally, making the TS compiler available in all of our projects :
   yarn add typescript or npm install -g typescript //For the latest stable version
  Text Editors With TypeScript
  Nowadays, there are a lot more text editors and IDEs that either natively or through plugins offer support for the TypeScript syntax, auto-complete suggestions, error catching, and even built-in compilers.  Visual Studio Code ,Official Free Plugin for Sublime Text, The latest version of WebStorm and More including Vim, Atom, Emacs and others.

----Slide - Building your first TypeScript file
In your editor, type the following JavaScript code in greeter.ts:

-------Slide -Compiling your code
We used a .ts extension, but this code is just JavaScript. You could have copy/pasted this straight out of an existing JavaScript app.
At the command line, run the TypeScript compiler:
tsc greeter.ts
The result will be a file greeter.js which contains the same JavaScript that you fed in. We’re up and running using TypeScript in our JavaScript app!
We can also use the --watch option to automatically compile a TypeScript file when changes are made: # Initializes a watcher process that will keep main.js up to date. tsc main.ts --watch
More advanced TypeScript users can also create a tsconfig.json file, consisting of various build settings. A configuration file is very handy when working on large projects with lots of .ts files since it somewhat automates the process.
-------Slide –Add TypeScript
Now we can start taking advantage of some of the new tools TypeScript offers. Add a : string type annotation to the ‘person’ function argument as shown here:

-------Slide -Type annotations
Type annotations in TypeScript are lightweight ways to record the intended contract of the function or variable. In this case, we intend the greeter function to be called with a single string parameter. We can try changing the call greeter to pass an array instead:
Re-compiling, you’ll now see an error:
error TS2345: Argument of type 'number[]' is not assignable to parameter of type 'string'.
Similarly, try removing all the arguments to the greeter call. TypeScript will let you know that you have called this function with an unexpected number of parameters. In both cases, TypeScript can offer static analysis based on both the structure of your code, and the type annotations you provide.
Notice that although there were errors, the greeter.js file is still created. You can use TypeScript even if there are errors in your code. But in this case, TypeScript is warning that your code will likely not run as expected.
-------Slide -Interfaces
Let’s develop our sample further. Here we use an interface that describes objects that have a firstName and lastName field. In TypeScript, two types are compatible if their internal structure is compatible. This allows us to implement an interface just by having the shape the interface requires, without an explicit implements clause.
-------Slide -Classes
Finally, let’s extend the example one last time with classes. TypeScript supports new features in JavaScript, like support for class-based object-oriented programming.
Here we’re going to create a Student class with a constructor and a few public fields. Notice that classes and interfaces play well together, letting the programmer decide on the right level of abstraction.
Also of note, the use of public on arguments to the constructor is a shorthand that allows us to automatically create properties with that name.
Re-run tsc greeter.ts and you’ll see the generated JavaScript is the same as the earlier code. Classes in TypeScript are just a shorthand for the same prototype-based OO that is frequently used in JavaScript.
---------Slide -TypeScript Facts -Thanks
 Large and scale application development
 Language, not a framework
 Cross-compiles to JavaScript
 Produces idiomatic JavaScript
 Doesn‘t try to replace JavaScript
 Offers missing language features (Anticipates ES6, …)
 Is a superset of JavaScript (Promises easy migration of JS code)
 JS libs can be used easily
 (Optional) static typing
