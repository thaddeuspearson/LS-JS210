# Introduction to Programming With JavaScript Exercises
Exercises for each section of Launch Schools Intro to Programming with JavaScript Book

## The Basics
1. Concatenate two or more strings, one with your first name and one with your last, to create a string with your full name as its value. For example, if your name is John Doe, think about how you can put `'John'` and `'Doe'` together to get `'John Doe'`.

    ```javascript
    'Thaddeus' + ' ' + 'Pearson'
    ```

1. Using arithmetic operators, get the individual digits of a 4-digit number like `4936`

    ```javascript
    let num = 4936

    for (i = 0; i < 4; i++) {
        let digit = num % 10
        num = (num - digit) / 10
        console.log(digit)
    }
    ```

1. Identify the data type for each of the following values:

    ```javascript
             'true' // String
             false  // Boolean
               1.5  // Number
                 2  // Number
         undefined  // Undefined
    { foo: 'bar' }  // Object
    ```

## Variables

## Input/Output

## Functions

## Flow Control

## Loops& Iterating

## Arrays

## Objects

## More Stuff