
## DEBUGGING & ERROR

* When you are writing JavaScript, do not expect to write it perfectly the first time , Programming is like problem solving: you are given a puzzle and not only do you have to solve it , but you also need to create the instructions that allow the computer to solve it , too .

---

### Each time a script enters a new execution context , there are two phases of activity : 
1. PREPARE
 * The new scope is created
 * Variables , functions , and arguments are created
 * The value of the this keyword is determined
2. EXECUTE
 * Now it can assign values to variables
 * Reference functions and run their code
 * Execute statements


> In the interpreter , each execution context has its own variables object , It holds the variables , functions , and parameters available within it , Each execution context can also access its parent's variables object .


![JS debugging](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/08/JavaScript-Debugging-and-Testing.png)

## HOW TO DEAL WITH ERRORS ?
1. debug the scrpit to fix errors .
 > If you come across an error while writing a script (or when someone reports a bug) , you will need to debug the code, track down the source of the error , and fix it .

2. handle errors gracefully
 > You can handle errors gracefully using try , catch , throw , and finally statements .

 ---

 > The JavaScript console will tell you when there is a problem with a script , where to look for the problem , and what kind of issue it seems to be .

### [For more detail : JS Book](https://www.goodreads.com/book/show/16219704-javascript-and-jquery)

---

## how to look at errors in chrome ?
> The console will show you when there is an error in your JavaScript , It also displays the line where it became a problem for the interpreter .

![error chrome](https://wordpress.org/support/files/2020/07/chrome-devtools.png)

---
### [Take Quiz](https://mhmadwrekat.github.io/reading-notes/quizclass10)

---
##### [Back To Home Page](https://mhmadwrekat.github.io/reading-notes)


---
<b>
<p align="center">
© Mohammad alwrekat
</p>