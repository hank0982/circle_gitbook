# Variables

There are three different ways to declare variables: `var, let and const`

## var vs let

* The scope of a variable defined with `var` is function scope or declared outside any function, global.
* The scope of a variable defined with `let` is block scope.



```javascript
function varvslet() {
  console.log(i); // (Optional) i is undefined due to hoisting
  // console.log(j); // ReferenceError: j is not defined

  for( var i = 0; i < 3; i++ ) {
    console.log(i); // 0, 1, 2
  };

  console.log(i); // 3
  // console.log(j); // ReferenceError: j is not defined

  for( let j = 0; j < 3; j++ ) {
    console.log(j);
  };

  console.log(i); // 3
  // console.log(j); // ReferenceError: j is not defined
}
```

 \(Optional\)  
You might not understand the difference between function scope and block scope. Please check the following example and [link](https://edgecoders.com/function-scopes-and-block-scopes-in-javascript-25bbd7f293d7) for more details.

```javascript
function(){
    // function scope is defined in every function called
    var a = 1;
    let c = 3;
    console.log(a);
    > 1
    console.log(c);
    > 3
    {
        /*
         block scope is wrapped by two brackets but not created by function
         e.g. 
             for(){block} 
             if(){block}
        */
        console.log(a);
        > 1
        let b = 2;
        console.log(b);
        > 2
    }
    console.log(b); // ReferenceError: b is not defined
    console.log(c);
    > 3
}
console.log(a); // ReferenceError: a is not defined
console.log(c);
```





## const

Variables defined with **const** behave like **let** variables, except they cannot be reassigned

```javascript
const apple = {juicy: true}
apple = {juicy: false} //ERROR
```

However, it acts slightly different from constant variables you learned from other languages. For further details, please check [link](https://www.w3schools.com/js/js_const.asp)

