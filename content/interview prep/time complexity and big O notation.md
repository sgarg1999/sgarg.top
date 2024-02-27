```table-of-contents
```
# Sources
- [CS DOJO | Introduction to Big O Notation and Time Complexity )](https://www.youtube.com/watch?v=D6xkbGLQesk)


# What is time complexity?
Imagine a function:
```
def coolFunction(array):
	"""
	Extremely tedious way to calculate sum of an array
	"""
	total = 0
	
	for i in array:
		total += i
		
	return total
```

We want to answer the question: **how much time it will take to run this function?**

However, this can depend on a lot of factors, meaning we would have non-standard measurements 

e.g.:
- hardware capabilities
- how many tabs ya got open bud
- which programming language are you using?

So, instead, we ask: **how does the runtime of this function grow?**

enter: ===time complexity===

For our `coolFunction`, we would say that the time complexity is **linear**.


This is because the runtime of the function increases linearly a the size of the input increase.

Other examples of complexity include:
- constant time: runtime does not change as size of input changes
	- e.g.: 
```
def constantTime(lst):
	return lst[0]		
```
- quadratic time: runtime changes in quadratic fashion as size of input changes
	- e.g.:
```
def quadraticTime(lst):
    total = 0
    for i in lst:
        for j in lst:
            total += i * j
    return total

```

But who really wants to sound like a Math major right? 

Why use the words constant, linear, quadratic, when you can sound even more pretentious and wise?

now enter: ===big O notation===

# What is big O notation?
Simply a way of denoting the complexity of an algorithm
```
{
	constant_time_complexity:      O(n),
	linear_time_complexity:        O(1),
	quadratic_time_complexity:     O(n^2)
}
```

Steps to find time complexity:
1. find the fastest growing term
2. take out the coefficient

e.g. *Given*

$$
T = an+b
$$
the fastest growing term would be:
$$
a \cdot n
$$
where the coefficient is simply $a$, which after removing, we are left with:
$$
n
$$
and therefore, we are in **linear** time // $O(n)$.

side note: this looks like a simple cheat for calculus, I'm sure theres some calc here though

