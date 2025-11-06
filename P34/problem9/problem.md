## Title

Matrix Median

## Slug

matrix-median

## Difficulty

Medium

## Description

Given an integer n (which is odd), consider an n x n multiplication table. However, instead of the standard multiplication table, each cell (i, j) (with i and j from 1 to n) contains the value (i * j) % n, where % is the modulo operation. But note: this table is different from the usual multiplication table. Now, if we list all n*n numbers in this table in non-decreasing order, what is the value at the middle position? (Since n is odd, n*n is odd and the median is well-defined.)

For example, for n=3, the table is:
Row1: (1*1)%3=1, (1*2)%3=2, (1*3)%3=0 → [1,2,0]
Row2: (2*1)%3=2, (2*2)%3=1, (2*3)%3=0 → [2,1,0]
Row3: (3*1)%3=0, (3*2)%3=0, (3*3)%3=0 → [0,0,0]

Sorting all values: [0,0,0,0,0,0,0,0,1,2,2] → the median is 0.

But actually, we need a different pattern. Actually, we will use the standard multiplication table but with modulo? Wait, no. Actually, let me redefine.

Actually, let's redefine the problem clearly. We consider an n x n matrix where the element at (i,j) is (i*j) mod n. Then we list all n*n numbers in non-decreasing order. The median is the value at the (n*n+1)/2-th position (1-indexed). For n=3, total elements 9, median is 5th element. The sorted list is: [0,0,0,0,0,0,0,1,2] wait no, actually let's compute properly.

Wait, but actually the problem is to find the median of the matrix where each cell is (i*j) mod n. But note: this is different from the base problem. So to avoid confusion, let's choose a different approach.

Actually, let's change the problem to avoid overlap with the base.

Alternatively, let's consider: Given n, consider an n x n matrix where the element at (i,j) is (i * j) mod (n+1) or something? But to make it distinct.

Alternatively, let's define the matrix as having elements a(i,j) = (i * j) mod (n+1) but then for n=3, modulus 4, then:
Row1: (1*1)%4=1, (1*2)%4=2, (1*3)%4=3 → [1,2,3]
Row2: (2*1)%4=2, (2*2)%4=0, (2*3)%4=2 → [2,0,2]
Row3: (3*1)%4=3, (3*2)%4=2, (3*3)%4=1 → [3,2,1]

Sort: [0,1,1,2,2,2,3,3,3] → median is 2.

But for n=3, the median is 2. So for n=3, output 2.

But to make the problem different, let's use a different function. Instead of (i*j) mod (n+1), let's use (i*j) mod (n*2) or something? Alternatively, let's use (i^2 + j^2) mod n? But that might be too different.

Wait, the base problem is about the multiplication table median. So to create a new problem that is similar but different, we can change the matrix definition.

Let's define the matrix such that the element at (i,j) is (i * j) mod (n*2) or something? But then the values are between 0 and n*2-1, which is large.

Alternatively, let's define the matrix as having entries: a(i,j) = (i^2 + j^2) mod (n*2) but that might not be similar.

Alternatively, let's use a different function: f(i,j) = (i * j) mod (n*2) but then for n=3, modulus 6:
Row1: (1*1)%6=1, (1*2)%6=2, (1*3)%6=3 → [1,2,3]
Row2: (2*1)%6=2, (2*2)%6=4, (2*3)%6=0 → [2,4,0]
Row3: (3*1)%6=3, (3*2)%6=0, (3*3)%6=3 → [3,0,3]
Sorted: [0,0,1,2,3,3,3,4] wait 9 elements: [0,0,1,2,3,3,3,4,?] Actually, the values are: 0,2,3,1,2,0,3,0,3? Let's list all: 
1: 1,2,3
2: 2,4,0
3: 3,0,3
So all values: 1,2,3,2,4,0,3,0,3 → which is: 0,0,1,2,2,3,3,3,4
Sorted: 0,0,1,2,2,3,3,3,4 → median (5th) is 2.

So for n=3, median is 2.

But the base problem for n=3 gave 3. So this is different.

But to make the problem meaningful, we need to find the median of the matrix where each cell is (i*j) mod m for some m. In the base problem, m is n, but here let's choose m = 2*n.

So define: For given n, consider the n x n matrix M where M(i,j) = (i*j) mod (2*n). Then sort all n*n values and find the median.

For n=3, as above, median=2.

For n=5, let's compute quickly? But to write the problem, we don't need to compute by hand, we can define the problem.

So the problem becomes: Given n, find the median of the set { (i*j) mod (2*n) | i=1..n, j=1..n }.

But note: the values are in range [0, 2*n-1]. And the median is the value at the (n*n+1)/2-th position.

But to compute this without generating all n*n values? Because n can be up to 1e6.

So we need an efficient method.

Actually, similar to the base problem, we can use binary search on the value to count the number of values <= x.

So let's define the problem as:

Given n, consider the n x n matrix where the (i,j)-th element is (i * j) mod (2*n). Then sort all n*n values. Find the value at the (n*n+1)/2-th position.

But wait, is this what we want? The base problem was about the multiplication table without modulus. Here we add modulus. But then the values are modulo 2n, so they are 0,1,...,2n-1. But in the multiplication table, the values are products which can be large.

But in our case, we are taking modulo 2n, so the values are in [0,2n-1]. So for large n, the matrix has many repeated values.

In fact, for each residue r, the number of pairs (i,j) such that (i*j) mod (2*n) = r is something we can compute.

But to find the median, we need to know the distribution.

Alternatively, we can use binary search on the value x, and count the number of entries <= x.

So define a function count(x) = number of pairs (i,j) such that (i*j) mod (2*n) <= x.

But note: the values are integers from 0 to 2n-1.

So for a given x, count the number of pairs (i,j) with (i*j) mod (2*n) <= x.

But note: (i*j) mod (2*n) is the remainder when i*j is divided by 2n. This is not directly comparable to x because x is an integer between 0 and 2n-1? Actually, the values are in 0..2n-1, so if we consider x as an integer, we can count.

But actually, the condition (i*j) mod (2*n) <= x is not straightforward because the modulus operation makes the value cyclic.

Actually, the value (i*j) mod (2*n) is the remainder, which is between 0 and 2n-1. So if x is in [0,2n-1], then we can count.

But note: for