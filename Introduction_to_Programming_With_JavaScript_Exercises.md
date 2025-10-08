# Introduction to Programming With JavaScript Exercises
Exercises for each section of Launch Schools Intro to Programming with JavaScript Book

## The Basics

1. Concatenate two or more strings, one with your first name and one with your last, to create a string with your full name as its value. For example, if your name is John Doe, think about how you can put `'John'` and `'Doe'` together to get `'John Doe'`.

    ```javascript
    'Thaddeus' + ' ' + 'Pearson'
    ```
    &nbsp;

1. Using arithmetic operators, get the individual digits of a 4-digit number like `4936`

    ```javascript
    let num = 4936

    for (i = 0; i < 4; i++) {
        let digit = num % 10
        num = (num - digit) / 10
        console.log(digit)
    }
    ```
    &nbsp;

1. Identify the data type for each of the following values:

    ```javascript
             'true' // String
             false  // Boolean
               1.5  // Number
                 2  // Number
         undefined  // Undefined
    { foo: 'bar' }  // Object
    ```
    &nbsp;

1. Explain why this code logs '510' instead of 15

    ```javascript
    console.log('5' + 10);
    ```

    The javascript interpreter is using implicit coercion to change the type of `10` to a string. If either operand is a string, the `+` operator will always result in concatenation.
    &nbsp;

1. Refactor the code from the previous exercise to use explicit coercion, so it logs 15 instead

    ```javascript
    console.log(Number('5') + 10)
    ```
    &nbsp;

1. Use the template literal syntax along with the expression `Number('5') + 10` to log the following sentence to the console: `The value of 5 + 10 is 15.`

    ```javascript
    console.log(`The value of 5 + 10 is ${Number('5') + 10}.`)
    ```
    &nbsp;

1. Will an error occur if you try to access an array element with an index that is greater than or equal to the length of the array? For example:
    
    ```javascript
    let foo = ['a', 'b', 'c'];
    console.log(foo.length);  // => 3
    console.log(foo[3]); 
    ```
    
    The above code will not cause an error, however `undefined` will be printed as there is no 3rd index in `foo` as currently defined.
    
    &nbsp;

1. Create an array named `names` that contains a list of pet names.

    ```javascript
    let names = [
        'asta',
        'butterscotch',
        'pudding',
        'neptune',
        'darwin'
    ]
    console.log(names)
    ```
    &nbsp;

1. Create an object named `pets` that contains a list of pet names and the type of animal.

    ```javascript
        let pets = {
            asta : 'dog',
            butterscotch : 'cat',
            pudding : 'cat',
            neptune : 'fish',
            darwin : 'lizard',
        };
    ```
    &nbsp;

1. What value does the following expression evaluate to?

    ```javascript
    console.log('foo' === 'Foo');
    ```

    This will evaluate to False and print `false` to the console.

    &nbsp;

1. What value does the following expression evaluate to?

    ```javascript
    console.log(parseInt('3.1415'));
    ```

    This will print 3 to the console.

    &nbsp;

1. What value does the following expression evaluate to?

    ```javascript
    console.log('12' < '9');
    ```

    This will print `true` to the console.

    &nbsp;

## Variables

1. Write a program named `greeter.js` that greets `'Victor'` three times. Your program should use a variable and not hard code the string value `'Victor` in each greeting.

    ```javascript
    let name = 'Victor';
    console.log(`Good Morning, ${name}.`);
    console.log(`Good Afternoon, ${name}.`);
    console.log(`Good Evening, ${name}.`);
    ```
    &nbsp;

1. Write a program named age.js that includes someone's age and then calculates and reports the future age in 10, 20, 30 and 40 years.

    ```javascript
    let age = 20;

    for (year = 10; year < 50; year += 10) {
        console.log(`In ${year} years, you will be ${age + year} years old.`)
    }
    ```
    &nbsp;

1. What happens when you run the following program? Why do we get that result?

    ```javascript
    {
    let foo = 'bar';
    }
    console.log(foo);
    ```

    `Reference error`, as foo is only defined within the scope of the brackets.
    
    &nbsp;

1. What happens when you run the following code? Why?
    
    ```javascript
    const NAME = 'Victor';
    console.log('Good Morning, ' + NAME);
    console.log('Good Afternoon, ' + NAME);
    console.log('Good Evening, ' + NAME);

    NAME = 'Joe';
    console.log('Good Morning, ' + NAME);
    console.log('Good Afternoon, ' + NAME);
    console.log('Good Evening, ' + NAME);
    ```

    The first 3 statements get logged to the terminal and then a TypeError
    occurs, as NAME is a constant variable and cannot be reassigned.

    &nbsp;

## Input/Output

## Functions

## Flow Control

## Loops& Iterating

## Arrays

## Objects

## More Stuff