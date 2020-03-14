# Time Complexity

Time Complexity, boils down to the rate the runtime of a function increases as the input gets very large.

Functions and algorithms can increase in a variety of different "times" and its important to know what each time represents.

To determine the time function grows in, we look at each individual line and approximate how the increase in runtime as input increases.

## Looking at a function

```python
class_grade = [80, 73, 20, 45, 100]
def GradeAverage(class_grade):

    average = 0
    count = 0
    for i in class_grade:
        average = average + i
        count = count + 1
    average = average / count

    return average
```

To calculate the time, break the code by lines.

```python
average = 0     
count = 0
```

Both these lines will take a constant amount of time: _c~1~_ and _c~2~_ respectively.

```python
average = average + i
count = count + 1
```

These lines also take a constant amount of time: _c~3~_ and _c~4~_ respectively. However, they repeat _n_ amount of times so the runtime of these lines would be _n_  __c~3~ _and_ n __ _c~4~_.

```python
average = average / count 
return average
```

These lines take a constant amount of time _c~5~_ and _c~6~_.

When looking for time complexity, the fastest growing term determines the time the function grows in. For our function `AverageGrade` , it would run in linear time because the runtime of a function increases as n increases.

### Big - O Notation

We use Big-O notation to express the time a function grows in.

* A function that grows in a _constant time_ doesn't grow at all. A graph of it's runtime would be a straight line. 
* Growing in _Linear Time_ means that the function increases at a steady rate. 
* Growing in _Quadratic Time_ would mean that the graph of the function's time would like the graph of a quadratic function. 

| Time | Big-O Notation |
| :--- | :--- |
| Constant Time | O\(1\) |
| Linear Time | O\(n\) |
| Quadratic Time | O\(n^2^\)\) |
| Factorial Time | O\(n!\) |
| Logarithmic Time | O\(log n\) |

Time Complexity is very important when it comes to functions because it allows us to measure how fast a function will grow.

**Time Complexity does not tell us the runtime of a function!! Calculating the runtime of a function is much harder because we have to consider hardware, IDE, etc**.

