
The algorithm takes the same amount of time irrelevant of the size of the input 


```python

def number_of_edges(nodes):
	result = 0
	for i in range(nodes):
		for j in range(i + 1, nodes):
			result +=1
	return result

```

This is O(n^2) -- nested loop

Change it to linear: 


```python

def number_of_edges(nodes):
	result = 0
	for i in range(nodes):
		nodes - (i + 1)

	return result

```
