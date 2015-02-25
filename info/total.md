Mortar teams should find the biggest squad on the map as fast as possible and take them out.

While searching out targets, they see five different kinds of cells on a map grid, each marked by a number.

The container is represented as a square matrix.
The numbers 1 through 5 are used to label the different kinds of cells -- the elements of the matrix.
Zero is an empty cell.
Find the largest group of identical numbers neighbotring each other and
figure out both the quantity of the cells within the group and the number the cells contain.

![gird](radiation-search.png)

**Input:** A square matrix as a list of lists. Each list contains integers. 

**Output:** The size and marking of the largest group as a list/tuple of two integers.

**Example:**

```python
find_union([
    [1, 2, 3, 4, 5],
    [1, 1, 1, 2, 3],
    [1, 1, 1, 2, 2],
    [1, 2, 2, 2, 1],
    [1, 1, 1, 1, 1]]) == [14, 1] # or (14, 1)

find_union([
    [2, 1, 2, 2, 2, 4],
    [2, 5, 2, 2, 2, 2],
    [2, 5, 4, 2, 2, 2],
    [2, 5, 2, 2, 4, 2],
    [2, 4, 2, 2, 2, 2],
    [2, 2, 4, 4, 2, 2]]) == [19, 2]
```
**How it is used:**

In this task, you can learn about Union-finding algorithms and Disjoint-set data structures.
It can be used in image recognition, geographic analysis and even model the partitioning of a set.

**Precondition:**
```python
3 <= len(matrix) <= 10
all(all(0 <= x <= 5 for x in row) for row in matrix
any(any(x for x in row) for row in matrix
```

The tests have only one unique solutions.

