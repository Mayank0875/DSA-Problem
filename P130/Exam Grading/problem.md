## Title
Exam Grading

## Slug
exam-grading

## Difficulty
Medium

## Description
Questions 1 to n are graded. The student knows their 'partial score' if questions 1 to k are all graded.

There is a sequence of $n$ questions indexed from $1$ to $n$. Initially, all questions are **ungraded**.

You grade the questions one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you grade the question at the position `sequence[i-1]`.

A state is called **scored** if, after performing $k$ steps, exactly the first $k$ questions (indices $1$ to $k$) are graded and all other questions are ungraded.

Your task is to calculate how many times the system becomes **scored** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "??A??" (Not scored)
- Step 2 (index 2): "?AA??" (Not scored)
- Step 3 (index 4): "?AAA?" (Not scored)
- Step 4 (index 1): "AAAA?" (scored: first 4 are graded)
- Step 5 (index 5): "AAAAA" (scored: first 5 are graded)
Total scored states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "???A" (Not scored)
- Step 2 (index 1): "A??A" (Not scored)
- Step 3 (index 2): "AA?A" (Not scored)
- Step 4 (index 3): "AAAA" (scored)
Total scored states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was scored.

## Constraints
- 1 ≤ n ≤ 10^4
- `sequence` is a permutation of numbers from $1$ to $n$.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy

## Company
google
