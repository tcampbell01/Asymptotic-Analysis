Logarithms is the inverse of exponential


```python

def binary_search(items, x):

	start = 0
	end = len(items) - 1

	while start <= end:
		mid = (start + end) // 2
		if x > items[mid]:
			start = mid + 1
		elif x < items[mid]:
			end = mid - 1
		else:
			return mid
	return -1

```
recursive version:


```python

def binary_search(items, x, start, end):

	mid = (start + end) // 2
	if start > end: 
		return -1
	elif x > items[mid]:
		return binary_search(items, x, mid + 1, end)
	elif x < items[mid]:
		return binary_search[items, x, start, mid - 1]
	else:
		return mid

```
in this version it is obvious that the input is reducing itself. -- dividing itself in 2

O(log (base 2) n)

==Logarithmic functions are very very scalable!==



