## Divide and Conquer and Greedy Problem Set

**Note**: These are just to give a head start. If you want to practice more, search online. Also, for detailed explanations of each problem, you will find helpful resources online.

### Divide and Conquer Problems

#### Problem 1: Binary Search
**Problem Description**: Implement a binary search algorithm to locate a target value in a sorted array. Return the index of the target value if it exists, or `-1` if it does not.

**Input Format**:
- A single integer `n` (1 \<= n \<= 10^5), the size of the array.
- A sorted array of `n` integers `a[1...n]` (-10^9 \<= a[i] \<= 10^9).
- A single integer `x`, the target value to search for.

**Output Format**:
- A single integer representing the 0-based index of `x`, or `-1` if not found.

**Sample Input**:
```
5
1 3 4 7 9
4
```
**Sample Output**:
```
2
```

---

#### Problem 2: Merge and Quick Sort
**Problem Description**: Implement the merge sort and quick sort algorithms to sort an array of integers in ascending order.

**Input Format**:
- A single integer `n` (1 \<= n \<= 10^5), the size of the array.
- An array of `n` integers `a[1...n]` (-10^9 \<= a[i] \<= 10^9).

**Output Format**:
- A single line containing the sorted array.

**Sample Input**:
```
6
5 2 9 1 5 6
```
**Sample Output**:
```
1 2 5 5 6 9
```

---

#### Problem 3: Power Calculation
**Problem Description**: Compute \(a^b\) efficiently using the divide and conquer technique.
**Try BigMod Problem too.**

**Input Format**:
- Two integers `a` and `b` (1 \<= a, b \<= 10^9).

**Output Format**:
- A single integer, the value of \(a^b\).

**Sample Input**:
```
2 10
```
**Sample Output**:
```
1024
```

---

#### Problem 4: kth Minimum and Maximum of an Array
**Problem Description**: Find the `k-th` smallest and largest elements in an unsorted array using DnC approach.

**Input Format**:
- A single integer `n` (1 \<= n \<= 10^5), the size of the array.
- An array of `n` integers `a[1...n]` (-10^9 \<= a[i] \<= 10^9).
- An integer `k` (1 \<= k \<= n).

**Output Format**:
- Two integers representing the `k-th` smallest and largest elements.

**Sample Input**:
```
6
7 10 4 3 20 15
3
```
**Sample Output**:
```
7 10
```

---

#### Problem 5: Finding Pair of Points with Minimum Distance
**Problem Description**: Given `n` points in a 2D plane, find the pair of points with the smallest Euclidean distance using a divide and conquer approach.

**Input Format**:
- A single integer `n` (2 \<= n \<= 10^5), the number of points.
- `n` pairs of integers representing the coordinates of the points.

**Output Format**:
- A single floating-point number representing the minimum distance.

**Sample Input**:
```
4
0 0
1 1
2 2
3 3
```
**Sample Output**:
```
1.414
```

---

#### Problem 6: Maximum Subarray Problem with Indices
**Problem Description**: Find the maximum sum of any contiguous subarray and return the indices of the subarray using the divide and conquer approach.

**Input Format**:
- A single integer `n` (1 \<= n \<= 10^5), the size of the array.
- An array of `n` integers `a[1...n]` (-10^4 \<= a[i] \<= 10^4).

**Output Format**:
- Two integers representing the start and end indices (0-based) of the subarray.
- The maximum sum.

**Sample Input**:
```
5
-2 1 -3 4 -1
```
**Sample Output**:
```
3 3
4
```

---

#### Problem 7: Skyline Problem
**Problem Description**: Given a list of buildings represented as triples `(Li, Ri, Hi)`, where `Li` is the left x-coordinate, `Ri` is the right x-coordinate, and `Hi` is the height, find the skyline formed by these buildings.


**Input Format**:
- A single integer `n` (1 \<= n \<= 10^5), the number of buildings.
- `n` triples `(Li, Ri, Hi)`.

**Output Format**:
- A list of critical points forming the skyline.

**Sample Input**:
```
2
2 9 10
3 7 15
```
**Sample Output**:
```
[2, 10], [3, 15], [7, 10], [9, 0]
```

---

### Greedy Problems

#### Problem 1: Fractional Knapsack (With Item List)
**Problem Description**: Find the maximum value that can be obtained from a fractional knapsack and the list of items taken.

**Input Format**:
- Two integers `n` and `W` (1 \<= n \<= 10^5, 1 \<= W \<= 10^9), the number of items and the knapsack capacity.
- Two arrays `value[1...n]` and `weight[1...n]` where `value[i]` and `weight[i]` are the value and weight of the `i-th` item.

**Output Format**:
- A floating-point number, the maximum value, and a list of fractions of items taken.

**Sample Input**:
```
3 50
60 100 120
10 20 30
```
**Sample Output**:
```
240.0 [(1, 1.0), (2, 1.0), (3, 0.6667)]
```

---

#### Problem 2: Job Sequencing
**Problem Description**: Schedule jobs to maximize profit, ensuring each job is completed within its deadline.

**Input Format**:
- A single integer `n` (1 \<= n \<= 10^5), the number of jobs.
- Two arrays `deadline[1...n]` and `profit[1...n]`.

**Output Format**:
- An integer, the maximum profit.

**Sample Input**:
```
4
4 1 1 1
20 10 40 30
```
**Sample Output**:
```
60
```

---

#### Problem 3: Activity Selection
**Problem Description**: Select the maximum number of activities that do not overlap.

**Input Format**:
- A single integer `n`.
- Two arrays `start[1...n]` and `end[1...n]`.

**Output Format**:
- An integer, the maximum number of activities.

**Sample Input**:
```
4
1 3 2 5
2 4 3 6
```
**Sample Output**:
```
2
```

---

#### Problem 4: Egyptian Fraction
**Problem Description**: Represent a fraction as a sum of unique unit fractions using the greedy algorithm.

**Input Format**:
- Two integers `numerator` and `denominator`.

**Output Format**:
- A list of unit fractions.

**Sample Input**:
```
6 14
```
**Sample Output**:
```
1/3 + 1/11 + 1/231
```

---

#### Problem 5: Minimum Product Subset of an Array
**Problem Description**: Find the minimum product subset of an array using a greedy approach.

**Input Format**:
- A single integer `n`.
- An array of `n` integers.

**Output Format**:
- An integer, the minimum product.

**Sample Input**:
```
4
-1 -1 -2 4 3
```
**Sample Output**:
```
-24
```

---
