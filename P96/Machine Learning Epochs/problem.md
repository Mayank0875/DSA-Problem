## Title
Machine Learning Epochs

## Slug
machine-learning-epochs

## Difficulty
Medium

## Description
A model groups training samples into batches. Each sample has a loss value.

The Researcher is working with a sequence of $n$ samples, where the $i$-th sample has a value of $a_i$.

The Researcher needs to create a **training schedule**. A training schedule involves dividing the sequence of $n$ samples into one or more contiguous batches such that every sample belongs to exactly one batch.

For a specific training schedule, the **loss gradient** is calculated as follows:
1. Calculate the sum of values for each batch in the partition.
2. The loss gradient is the bitwise XOR sum of these batch sums.

Your task is to calculate the bitwise XOR sum of the loss gradient values of **all possible training schedules** of the sequence.

## Examples

### 1

#### Input
1
1

#### Output
1

#### Explanation
Total XOR sum: 1.

### 2

#### Input
2
1 2

#### Output
0

#### Explanation
Partition {1}, {2}: Group sums are 1, 2. XOR sum = 1 ^ 2 = 3.
Partition {1, 2}: Group sum is 3. XOR sum = 3.
Total Result = 3 ^ 3 = 0.

## Input Format
- The first line contains a single integer $n$ — the length of the sequence.
- The second line contains $n$ space-separated integers $a_1, a_2, \dots, a_n$.

## Output Format
- Return a single integer representing the total XOR sum of loss gradients of all possible partitions.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ a_i ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming, array
