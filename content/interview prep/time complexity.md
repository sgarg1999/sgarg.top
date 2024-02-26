>[!SUMMARY] Table of Contents

>- [[time complexity#SOURCES:|SOURCES:]]
>- [[time complexity#What is time complexity?|What is time complexity?]]
# Sources:
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

enter: [[BIG O NOTATION]] and [[TIME COMPLEXITY]]

For our `coolFunction`, we would say that the time complexity is **linear**.
This is because the runtime of the function increases 