# Prototype-based Language \(Optional\)

Javascript is a prototype-based language. So what is a prototype-based language ?

{% code-tabs %}
{% code-tabs-item title="Program1" %}
```javascript

var foo = {one: 1, two: 2};

// bar.[[prototype]] = foo
var bar = Object.create(foo);

bar.three = 3;

bar.one; // 1
bar.two; // 2
bar.three; // 3
```
{% endcode-tabs-item %}
{% endcode-tabs %}

In above example, after line 6, bar will have one 'three' attribute and one '\_\_proto\_\_' attribute like following:

```text
bar = {
    three: 3,
    __proto__: {
        one: 1,
        two: 2
    }
}
```

When the `program1` executes to the line 8, it cannot directly get the 'one' attribute. It will further search \_\_proto\_\_  to find out whether there is 'one' attribute inside. The structure of this is called prototype chain.

Everything in javascript is Object. It means everything in Javascript has the same prototype as Object.

For example,

```javascript
var a = function(){}
console.log(a.__proto__)
> [Function]
console.log(a.__proto__.__proto__)
> {}
var apple = {juicy: true}
console.log(apple.__proto__)
> {}
console.log(apple.__proto__ == a.__proto__.__proto__)
> true
console.log(apple.__proto__.__proto__)
> null
```

In the above example, you will see the variable "a" points to a Function and the variable "apple" points to an Object. However, they both share the same \_\_proto\_\_ object \(see line 5, 8 and 9\).

