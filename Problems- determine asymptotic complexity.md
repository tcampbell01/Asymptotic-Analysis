
Problem 1: 

==LINEAR -==- this algorithm executes 1 time for each i, so it runs n times.  
```cpp

for (int i = 0; i < n; i++) {
    cout << "Hello" << endl;
}


```

Problem 2:  ==Logarithmic==

We are doubling i, so we're counting how many times we can multiple by 2 before reaching n.  Time complexity = Θ(log n)
```cpp

for (int i = 1; i < n; i *= 2) {
    cout << i << endl;
}


```

Problem 3:

==Quadratic== - This is a nested loop.  Θ(n²)
```cpp

for (int i = 0; i < n; i++) {
    for (int j = 0; j < n; j++) {
        cout << i + j << endl;
    }
}


```

Problem 4: ==Linearithmic==

Outer loop runs n times.  Inner loop multiplies by two... Θ(n log n)
```cpp

for (int i = 0; i < n; i++) {
    for (int j = 1; j < n; j *= 2) {
        cout << i + j << endl;
    }
}


```

Problem 5:  ==quadratic==

Outer loop runs n times.  Inner loop runs i times(which increases with each outer loop step) Θ(n²)
```cpp

for (int i = 0; i < n; i++) {
    for (int j = 1; j < n; j *= 2) {
        cout << i + j << endl;
    }
}


```
### 🔁 Visual Analogy

Think of **O(n²)** as saying:

> "I’ll get to the destination in _at most_ 2 hours."

And **Θ(n²)** as saying:

> "I’ll get to the destination in _exactly_ 2 hours every time."