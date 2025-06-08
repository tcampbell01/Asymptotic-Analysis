Chess/ rice game fable 2^62


```python

{7,2,3} , target value = 9

def subset_sum(s, target) {
	#s is set

	n = len(s)

	for i in range(2 ** n): #2 ^ n
		sum = 0
		for j in range(n):
			if i & (2 ** j):
				sum += s[j]
				print(s[j]), " ", end=''
		if sum == target:
			return True
	return False
}

```

outer loop iterates (worst case) at 2^n
O(2^n * n)