# Space Complexity

Space Complexity is the rate of a function's memory usage as input increases. As the input of functions and algorithms gets very large, the amount of memory required also will increase. It can increase in different rates and Space Complexity allows us to express those rates .

Space Complexity revolves much more on _data types_ rather than executing the code.

_Integers_, _floats_, _Strings_ are **data types** that always take a constant amount of memory.

**Data Types** like arrays do not take a constant amount of memory. The elements inside an array are malleable so the amount of memory an array takes fluctuates.

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

Lets examine this block of code, line by line.

The values of the variables`Average` and `Count` will always take a constant amount of space. Those values are _c~1~_ and _c~2~_.

We have another datatype, `class_grade`, which takes up _c~3~_ amount of memory for every _n_ element. The amount of memory this takes is _n_  __c~3~\* .

The term that has the fastest growing memory usage determines the rate of how much memory is being used by the function. In this case, it would be _n_  __c~3~\* which means the function's memory usage growth is linear.

