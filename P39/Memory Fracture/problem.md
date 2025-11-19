## Title

Memory Fracture

## Slug

memory-fracture

## Difficulty

Easy

## Description

Imagine sifting through a chain of fragmented memories, each assigned an intensity value. As you examine each memory, you look back at the earlier moments (to your left) and want to know the intensity of the nearest previous memory that is strictly stronger than the one you are currently recalling. If all earlier memories are weaker or of equal intensity, or if it's the first memory, there is no such stronger memory to the left. Your goal is to determine this stronger memory's intensity for each position in the sequence.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

Memory 0 (30): No previous memory. Output -1.
Memory 1 (60): Memory 0 (30) is weaker. Output -1.
Memory 2 (90): Memories 0 (30), 1 (60) are weaker. Output -1.
Memory 3 (50): Memory 2 (90) is the nearest stronger. Output 90.
Memory 4 (80): Memory 2 (90) is the nearest stronger. Output 90.
Memory 5 (40): Memory 4 (80) is the nearest stronger. Output 80.
Memory 6 (70): Memory 4 (80) is the nearest stronger. Output 80.
Memory 7 (50): Memory 6 (70) is the nearest stronger. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All memories have equal intensity, so no strictly stronger previous memory exists.

## Input Format

The first line contains a single integer n, the number of memories.
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the intensity of each memory.

## Output Format

Return array of integers. The i-th integer should be the intensity of the nearest memory j < i such that h_j > h_i. If no such day exists, then -1.

## Constraints

1 ≤ n ≤ 10^5
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array