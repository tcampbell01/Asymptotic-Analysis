
Merge Sort 

#divide and conquer algorithm
```python

def merge(items,left, right):
	l,r = 0,0

	for i in range(len(items)):
		value_l = left[l] if l < len(left) else math_inf
		value_r = right[r] if r < len(right) else math_inf
	items[i] = min(vlue_1, value_r)
if value_1 < value_r:
	l += 1
else: 
	r += 1
return items

def merge_sort(items):
	mid = len(items) // 2
	left = merge_sort(items[:mid])
	right = merge_sort(items[mid:])
	return merge(items, left, right)
	
```

Merge part of the algorithm has O(n ---> linear)

Merge_sort splits the input as it goes along... so n/2 ... log(base 2)n 