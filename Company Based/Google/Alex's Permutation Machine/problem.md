## Title

Alex's Permutation Machine

## Slug

alexs-permutation-machine

## Difficulty

Medium

## Description

Alex has discovered an ancient machine that processes sequences of numbers. The machine works with a specific type of sequence called a **zero-based permutation** of length $n$. This means the sequence contains distinct integers from $0$ to $n-1$.

The machine has a "Double Step" feature. When activated, it transforms the input array `nums` into a new array `ans`. The rule for the transformation is strictly defined: for every index $i$ (where $0 \le i < n$), the new value `ans[i]` must be equal to `nums[nums[i]]`.

Alex needs your help to simulate this machine's operation efficiently. Given the permutation `nums`, can you build the resulting array `ans`?

## Examples

### 1

#### Input

3
0 2 1

#### Output

0 1 2

#### Explanation

In the first example, nums = [0, 2, 1].
ans[0] = nums[nums[0]] = nums[0] = 0
ans[1] = nums[nums[1]] = nums[2] = 1
ans[2] = nums[nums[2]] = nums[1] = 2 Result: [0, 1, 2].
    
### 2

#### Input

4
3 2 1 0

#### Output

0 1 2 3

#### Explanation

In the second example, nums = [3, 2, 1, 0].
ans[0] = nums[nums[0]] = nums[3] = 0
ans[1] = nums[nums[1]] = nums[2] = 1
ans[2] = nums[nums[2]] = nums[1] = 2
ans[3] = nums[nums[3]] = nums[0] = 3 Result: [0, 1, 2, 3].
  

## Input Format  

- The first line contains a single integer $n$ ($1 \le n \le 1000$) — the length of the permutation.
- The second line contains $n$ distinct integers `nums[0], nums[1], ..., nums[n-1]` ($0 \le nums[i] < n$).

## Output Format  

- Return the transformed array `ans` on a single line, with elements separated by spaces.
  

## Constraints  

- 1 ≤ n ≤ 1000
- 0 ≤ nums[i] < n


## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array, two-pointers, hash-table