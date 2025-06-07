* There is a direct correlation between the input and the output.  If we double the amount that we input, we will double the amount of time it takes to run it *

==A complexity Class tells us how well it scales, no how long it takes== 


```python

def find_min(items):
	smallest = None

	for i in items:
		if smallest is None or i < smallest:
			smallest = i

	return smallest

```

What are we doing here? 
3 or more operations for each item in our input list: 
	1. Look at the number
	2. Compare it to Smallest or None
	3. reassign if necessary

	Why not 3o(n)? O(n) == O(2n) == O(3n) 



```Python
def str_equals(str_a, str_b):
	if len(str_a) != len(str_b):
		return False
	for i in range(len(str_a)):
		if str_a[i] != str_b[i]:
			return False
	return True

```

Complexity: O(n + 2) BUT we don't need the +2 because we drop the constant = O(n)

Best case: it will return false almost immediately when the strings are not the same length O(1)
Worst case: When we have a complete match because we have to iterate over every character that we have O(n)



![[Screenshot 2025-06-07 at 5.26.40 PM.png 

A straight line would indicate a linear complexity.  A faster algortihm would have  a shallower gradient, a slower one would have a steeper gradiant 