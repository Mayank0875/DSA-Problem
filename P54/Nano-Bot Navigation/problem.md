## Title
Nano-Bot Navigation

## Slug
nano-bot-navigation

## Difficulty
Medium

## Description
A nano-bot travels through a cellular grid. It is programmed to target a specific sequence of cell receptors. It moves to adjacent cells. Verify if the target sequence exists in the tissue sample.

## Examples

### 1

#### Input
3 4
[["A","B","C","E"],["S","F","C","S"],["A","D","E","E"]]
"SEE"

#### Output
Yes

#### Explanation
The word "SEE" can be formed by moving:
(1, 0) -> 'S'
(2, 2) -> 'E' (No, this path is invalid, strictly adjacent: S(1,0) -> E(2,2) is not adjacent).
Correct Path: S(1,0) -> E(2,2) is invalid. 
Let's trace: S at (1,3) -> E at (1,2) -> E at (2,2)? No.
Trace: S at (1,0) -> F(1,1) -> C(1,2) ... 
Correct Trace: S(1,3) -> E(0,3) -> E(0,2) is invalid (C).
Actual valid path for SEE: S(1,3) -> E(2,3) -> E(2,2).
The word exists in the grid following the adjacent cells.

### 2

#### Input
3 4
[["A","B","C","E"],["S","F","C","S"],["A","D","E","E"]]
"ABCB"

#### Output
No

#### Explanation
Starting from A(0,0) -> B(0,1) -> C(0,2) -> B? 
The adjacent cells to C(0,2) are B(0,1), F(1,2), E(0,3).
B(0,1) is already used. F and E are not 'B'.
The word cannot be formed.

## Input Format
- The first line contains two integers, `m` and `n`, representing the grid dimensions.
- The next lines represent the `board` as a grid of characters.
- The last line contains the `word` string.

## Output Format
- Return `true` (printed as Yes) if the word exists in the grid. Otherwise `false` (printed as No).

## Constraints
- 1 ≤ m, n ≤ 6
- 1 ≤ word.length ≤ 15
- `board` and `word` consist of only uppercase English letters.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
backtracking, breadth-first-search
