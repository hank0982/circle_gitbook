# Function

There are different ways to declare a function. Following are some common ways to declare a getApple function.

```javascript
function getApple(){}

var getApple = function(){}

var getApple = () => {}
```

Generally speaking, a function is a "subprogram" that can be _called_ by code external \(or internal in the case of recursion\) to the function. Like the program itself, a function is composed of a sequence of statements called the _function body_. Values can be _passed_ to a function, and the function will _return_ a value. Please see the following examples to further understand Function

```javascript
function getApple(isJuicy){ // isJuicy is an argument pass to function "getApple"
    const apple = {
        isJuicy
    } 
    /*
    this is the syntactic sugar which is equivalent to 
    const apple = {isJuicy: isJuicy}
    */
    return apple;
}
const newApple = getApple(true)
console.log(newApple.isJuicy);
> true

```

## Pass by reference ? Pass by Value ? Pass by Sharing !! Check this [link](https://www.youtube.com/watch?v=1YFss_4B_o4) for further details \(Optional Optional and Optional\)

## Function as Object \(Optional\)

Function is the Function Object. You can pass function as Object to another function as callback.

```javascript
function getApple(){console.log('APPLE')}
console.log(getApple.__proto__)
> [Function]
// pass the function to function
function getStuff(fn){fn()}
getStuff(getApple)
> 'APPLE'
```

* callback: In computer programming, a callback, also known as a "call-after" function, is any executable code that is passed as an **argument** to other code, which is expected to call back \(execute\) the argument at a given time. This execution may be immediate as in a synchronous callback, or it might happen at a later time as in an asynchronous callback

