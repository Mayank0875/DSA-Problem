## Title

Matrix Median

## Slug

matrix-median

## Description

Given an integer n, consider the n x n multiplication table. However, instead of the standard multiplication table, we define each cell (i, j) (with i and j from 1 to n) to have the value i * j * (i + j) (instead of i * j). Find the median element when all the n² numbers in this table are sorted in increasing order. It is guaranteed that n is odd.

For example, for n = 3, the table is:
Row 1: 1*1*(1+1)=2, 1*2*(1+2)=6, 1*3*(1+3)=12 → [2,6,12]
Row 2: 2*1*(2+1)=6, 2*2*(2+2)=16, 2*3*(2+3)=30 → [6,16,30]
Row 3: 3*1*(3+1)=12, 3*2*(3+2)=30, 3*3*(3+3)=54 → [12,30,54]

The sorted list is [2,6,6,12,16,30,30,54] (8 elements). The median is the average of the 4th and 5th elements: (12 + 16)/2 = 14, but since we need a single value and n is odd, we take the middle one directly? Actually, wait: there are 9 elements? Let's recalc.

Wait, the problem says n=3 gives 9 elements? But in our example, we have 3 rows and 3 columns, so 9 elements. But in the description, we have 8? That was a mistake. Actually, for n=3, there are 9 elements. But the problem says "n is odd", so n=3 gives 9 elements? But the median of 9 elements is the 5th element. So we need the 5th smallest.

But in the example above, the sorted list of 9 numbers would be? Actually, the table above: 
Row1: 2,6,12
Row2: 6,16,30
Row3:12,30,54

So the sorted list is [2,6,6,12,12,16,30,30,54] (9 numbers). The 5th is 12.

But note: the problem asks for the median, which for an odd number of elements is the middle one. So for n=3, the median is the 5th smallest, which is 12.

But wait: the example in the base problem was for a standard multiplication table. Here we have a different function: i*j*(i+j). So the problem is similar but with a twist.

Now, for n=5, we need to compute the median.

## Examples

### 1

#### Input

3

#### Output

12

#### Explanation

The sorted list for n=3 is [2,6,6,12,12,16,30,30,54]. The 5th element is 12.

### 2

#### Input

5

#### Output

192

#### Explanation

For n=5, the median is 192.

## Input Format

- The only input line has an integer n.

## Output Format

- Return one integer: the answer to the task.

## Constraints

- 1 ≤ n ≤ 1e6

## Time Limit

2 seconds

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory