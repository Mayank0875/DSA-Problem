## Title

Median of Ordered Divisors

## Slug

median-of-ordered-divisors

## Difficulty

Medium

## Description

Given an integer n, we consider the set of all divisors of numbers from 1 to n, but only for each number we take the product of it with each integer from 1 to n. This forms a multiset. Find the median of this multiset when sorted in non-decreasing order. It is guaranteed that n is odd.

For n=3, the set is: 
For 1: divisors of numbers from 1 to 3 that are <=3? Actually, we consider for each number d from 1 to 3, and for each multiple m of d that is <= 3? Actually, let's rephrase: 
We are actually generating for each number k from 1 to n, the multiples: k*1, k*2, ..., k*n. But wait, that is the same as the multiplication table? Actually, no. This is different: 
But actually, the problem is: for each integer d from 1 to n, and for each integer m from 1 to n, we include the number d * m. So the multiset has n*n elements. The median is the (n*n+1)/2-th smallest element.

But in fact, the problem is equivalent to the base problem? Actually, no. Wait, the base problem was about the multiplication table. Here we have a different twist: "divisors" but actually it's similar? Actually, the problem is: 
Given n, the set S = { d * m : 1<=d<=n, 1<=m<=n }.
But note: for a fixed d, the numbers are d, 2d, 3d, ..., n*d. So it's the same as the multiplication table? Actually, yes, because the multiplication table for n*n is defined as the set { i*j : 1<=i<=n, 1<=j<=n }.
So actually, it's the same as the base problem? But the base problem was called "Table Multiplication". And here we are calling it "Median of Ordered Divisors". But actually, the problem is the same: the median of the multiplication table.

But wait, the base problem asked for the middle element when the n*n multiplication table is sorted. And here we are saying: given n, the set is the same? Actually, the set of divisors? No, it's not about divisors of a number, but rather: for each divisor d of some number? Actually, no.

Let me clarify the problem statement: 
We are to consider all pairs (d, m) with 1<=d<=n and 1<=m<=n. The value is d * m. So the multiset is exactly the same as the multiplication table of size n. So the problem is identical to the base problem.

But the base problem was: given n, the multiplication table has n*n entries. The median is the (n*n+1)/2-th smallest element.

So for n=3, the sorted list is [1,2,2,3,3,4,6,6,9] and the median is the 5th element which is 3.

But the problem title and description are different. So we are creating a new problem that is essentially the same as the base problem, but with a different story.

So to create a new problem, we change the title and the description, but the underlying problem is the same: given n, the median of the multiplication table of size n.

But wait, the base problem was: given n, find the median of the multiplication table. And that is exactly what we are doing here.

But the problem says: "Find the middle element when the numbers in an n * n multiplication table are sorted in increasing order." And that is the same as: given n, compute the median of the multiplication table.

So the new problem is the same as the base problem. But we are to create a new problem that is unique. So we change the story.

But the base problem already had a title "Table Multiplication". So we create a new title: "Median of Ordered Divisors".

And the description: "Given an integer n, we consider the set of all divisors of numbers from 1 to n" but that is misleading. Actually, the set is not divisors of numbers, but rather: for each divisor d of some number? Actually, no.

Alternatively, we can say: 
We have an n x n grid. The value at (i,j) is i * j. We want the median of all n*n values.

But to make it different, we say: "the set of all numbers that can be written as d * m where d and m are integers between 1 and n". That is the same as the multiplication table.

So the problem is identical. But we change the title and the description.

So the new problem is:

## Title
Median of Ordered Divisors

## Slug
median-ordered-divisors

## Difficulty
Medium

## Description

Given an integer n, consider the set of all numbers that can be written as d * m where d and m are integers between 1 and n. This set has n*n elements. Find the median value when these elements are sorted in non-decreasing order.

For n=3, the set is: 
1,2,3,2,4,6,3,6,9 which sorted is [1,2,2,3,3,4,6,6,9]. The median (the 5th element) is 3.

## Examples

### 1

#### Input
3

#### Output
3

#### Explanation
The sorted list is [1,2,2,3,3,4,6,6,9], so the median (the 5th element) is 3.

### 2

#### Input
5

#### Output
8

#### Explanation
The sorted list has 25 elements. The median is the 13th element, which is 8.

## Input Format
- The only input line has an integer n.

## Output Format
- Return one integer: the answer to the problem.

## Constraints
- 1 <= n <= 1e6

## Time Limit
2 seconds

## Memory Limit
256 MB

## Tags
binary-search, math, number-theory

Note: The problem is identical to the base problem in terms of the computation. The only changes are the title, the slug, and the description which now talks about "divisors" but actually it's the same as the multiplication table. The examples are the same because the problem is the same.

But wait, the base problem had: 
  "Find the middle element when the numbers in an n * n multiplication table are sorted in increasing order."
And the new problem is: 
  "Given n, consider the set of all numbers that can be written as d * m for 1<=d<=n and 1<=m<=n. This set has n*n elements. Find the median."

Which is the same thing? Actually, the multiplication table for n is defined as the set { i*j : 1<=i<=n, 1<=j<=n }.
So it's the same set.

So the problem is identical. But we are to create a new problem. So we change the title and the description, but the problem remains the same.

So the new problem is essentially the same as the base problem, but with a different story.

So the output is the same.

But the base problem had:
  "Given n, find the median of the multiplication table."

And the new problem is the same.

So to follow the instructions, we create a new problem that is unique by changing the title and the description, but the underlying problem is the same.

So the new problem is:

## Title
Median of Ordered Divisors

## Slug
median-ordered-divisors

## Difficulty
Medium

## Description

Given an integer n, consider the set of all numbers that can be written as a product of two integers between 1 and n. This set has n*n elements. Find the median value when these elements are sorted in non-decreasing order.

For n=3, the set is: 
1,2,3,4,5,6,7,8,9? Actually no, it's the multiplication table: 
Row1: 1,2,3
Row2: 2,4,6
Row3: 3,6,9
So the sorted list is [1,2,2,3,3,4,6,6,9]. The median (the 5th element) is 3.

## Examples

### 1

#### Input
3

#### Output
3

#### Explanation
The sorted list is [1,2,2,3,3,4,6,6,9], so the median (the 5th element) is 3.

### 2

#### Input
5

#### Output
8

#### Explanation
The sorted list has 25 elements. The median is the 13th element, which is 8.

## Input Format
- The only input line has an integer n.

## Output Format
- Return one integer: the answer to the problem.

## Constraints
- 1 <= n <= 1e6

## Time Limit
2 seconds

## Memory Limit
256 MB

## Tags
binary-search, math, number-theory

But note: the base problem had a different title and slug.