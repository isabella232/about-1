# function

## Function

A **function** is a block of code that _**1. takes input**_, _**2. processes that input**_, and then _**3. produces output**_.

Here is an example:

```javascript
function example (x) {
  y = x * 2
  return y
}
```

_Name_ of function: **example**

_Input_ \(_argument_\): **x**

_processes_: **x\*2**

_output_ \(_return value_\): **y**

We can _**call**_ that function like this :

```javascript
example(5)
```

The **result** is :

```javascript
10
```

The above example assumes that the `example` function will take a number as an argument –– as input –– and will return that number multiplied by 2.

## The challenge:

Create a file named `functions.js`.

In that file, define a function named `eat` that takes an argument named `food` that is expected to be a string.

Inside the function return the `food` argument like this:

```javascript
return food + ' tasted really good.'
```

Inside of the parentheses of `console.log()`, call the `eat()` function with the string `bananas` as the argument.

Check to see if your program is correct by running this command:

```bash
javascripting verify functions.js
```

