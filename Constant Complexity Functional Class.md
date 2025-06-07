
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

This is O(n)

Change it to constant? 


```python

def number_of_edges(nodes):
	return nodes * (nodes - 1) / 2

```

This is O(1) because it doesn't change based on the size of the input 

