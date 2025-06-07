Run time complexity of O(n^2)

(grows a lot faster than linear and don't scale well comparitively)


```python

from quadratic.Ppoint2D import Point2D
from math import dist

def find_closest_pair(points):
	minimum_dist = math.inf
	closest_pair = (None, None)
	
	for i in range(len(points)):
		for j in range(i, len(points)):
			distance = dist(points[i], points[j])
				if distance < minimum_dist and i != j:
					minimum_dist = distance
					closest_pair = (points[i], points[j])
		return closest_pair
	

```

outer loop - n times
inner loop - n times 
	= O(n^2) 
	
==(if there are nested loops, it's a good indication that this is quadratic)==

Looking at the graph, this would have a curved line on the graph 

==THE COMPLEXITY DOES NOT TELL US HOW FAST, IT ONLY TELLS US HOW WELL IT SCALES== 


```python

def find_closest_pair(points):
	minimum_dist = math.inf
	closest_pair = (None, None)
	for i in range(len(points)):
		for j in range(i + 1, len(points)):
			distance = dist(points[i], points[j])
			if distance < minimum_dist:
				minimum_dist = distance
				closest_pair = (points[i], points[j])
		return closest_pair

```

