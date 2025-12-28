## Title
Memory Allocation

## Slug
memory-allocation

## Difficulty
Medium

## Description
An OS allocates memory blocks. Each block has a start address and end address.

The heap contains list of blocks, each defined by a start addr and an end addr, represented as a pair `[start, end]`.

Blocks cannot overlap. The end address of one block must be strictly less than the start address of the next. Specifically, to transition from block `[a, b]` to a subsequent block `[c, d]`, the end of the first block must be **strictly less than** the start of the second block (i.e., `b < c`).

You can select blocks in any order you like to form a valid memory map. Your goal is to determine the maximum number of blocks that can be included in a single memory map.

## Examples

### 1

#### Input
3
1 2
2 3
3 4

#### Output
2

#### Explanation
The longest memory map is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The blocks can be reordered to form the memory map `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available blocks.
- The next `n` lines each contain two integers, representing the `start` and `end` of an block.

## Output Format
- Return a single integer representing the maximum length of the memory map.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ start < end ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
