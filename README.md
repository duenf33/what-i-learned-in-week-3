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
Searching for (and fixing) errors in programming code is called code debugging.<br>
We are going to take a closer look on how to debug in VSCode. It is simple to do, however it could be a little confusing at first.<br>
Here below I will have some screenshots explaining the steps to follow ⇲<br>

![vscode-debugging](./week3/vscode-debugging-hd.gif)
