# WHAT-I-LEARNED-IN-WEEK-3

## 🎢 Hoisting :
Hoisting is JavaScript's default behavior of moving all declarations to the top of the current scope (to the top of the current script or the current function).<br>
For example:<br>

* This wont work ⇲<br>
```javascript
console.log(a + b); //ReferenceError: a is not defined
                    // ReferenceError: Cannot access 'a' before initialization
let a = 2;

let b = 2;
```
As you can see in the example above we are `console.log`-ing before we declare the variables and that will not work.<br>


* This will work ⇲<br>
```javascript
function example(a, b) {

    return a + b;
}

example(2, 2); // result: 4
```
As you can see on this example above we called the `function example` before the function and we were still able to run what was inside the function.<br>

---

## 🕸 `Code` De`bug`ging 🕸<br>
Programming code might contain syntax errors, or logical errors.<br>
Many of these errors are difficult to diagnose.<br>
Often, when programming code contains errors, nothing will happen. There are no error messages, and you will get no indications where to search for errors.<br>
Searching for and fixing errors in programming code is called `code debugging`.<br>
We are going to take a closer look on how to debug in VSCode. It is simple to do, however it could be a little confusing at first.<br>
Here below is a `gif` file showing in a few steps how to debug a simple function ⇲<br>

![vscode-debugging](./week3/vscode-debugging-hd.gif)

[Click here to find more information about `VS-Code debugging`](https://code.visualstudio.com/docs/editor/debugging)

---

## ♺ Node.js `process.argv` property ♺<br>
The process.argv property is an inbuilt application programming interface of the process module which is used to get the arguments passed to the node.js process when run in the command line.<br>

This property returns an array containing the arguments passed to the process when run it in the command line. The first element is the process execution path and the second element is the path for the js file.<br>

![process.argv](week3/process-argv.png)

As you can see in the left hand side of the screenshot above. There is a terminal displaying a couple of commands invoking `node main.js red blue`.<br>
Pretty much this command is inputting the colors to the code in the right hand side. You can see those two constants `color1` and `color2` both with `process.argv[]`property with an argument location value of the previous mentioned colors `red` and `blue`. Here Below I will show how this terminal command is looked at as an array ⇲<br>

|   0   |   1   |   2   |   3   |
| :---: | :---: | :---: | :---: |
| node  |main.js|  red  |  blue |
