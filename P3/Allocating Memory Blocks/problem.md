## Title

Allocating Memory Blocks

## Slug

allocating-memory-blocks

## Difficulty

Easy

## Description

A memory manager needs to allocate processes to memory blocks. Each block can hold one or two processes. The total memory required by the process(es) in a block cannot exceed the block's size `x`. You have `n` processes, each requiring a certain amount of memory. Find the minimum number of memory blocks needed to accommodate all processes without exceeding the size limit for any block.

## Examples

### 1

#### Input

4 10
[7, 2, 3, 9]

#### Output

3

#### Explanation

One optimal allocation:
    - Block 1: Process requiring 2 units and process requiring 7 units (Total memory 9 <= 10)
    - Block 2: Process requiring 3 units (Total memory 3 <= 10)
    - Block 3: Process requiring 9 units (Total memory 9 <= 10)
This requires 3 blocks.

### 2

#### Input

5 5
[2, 2, 2, 3, 4]

#### Output

3

#### Explanation

One optimal allocation:
    - Block 1: Process requiring 2 units and process requiring 3 units (Total memory 5 <= 5)
    - Block 2: Two processes requiring 2 units (Total memory 4 <= 5)
    - Block 3: Process requiring 4 units (Total memory 4 <= 5)
This requires 3 blocks.

## Input Format

- The first line contains two integers n and x: the number of processes and the size of each memory block.
- The second line contains n integers p_1, p_2, ..., p_n: the memory requirement of each process.

## Output Format

- Return a single integer: the minimum number of memory blocks required.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x ≤ 1e9
- 1 ≤ p_i ≤ x

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

greedy, sorting, two pointers