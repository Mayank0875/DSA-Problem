## Title

Letter Puzzle Box

## Slug

letter-puzzle-box

## Difficulty

Medium

## Description

You have a puzzle box with a `board` (grid) of letters on its lid. To open it, you must trace a secret `word`. You can trace the path by moving from a letter to an adjacent one (up, down, left, or right). You are not allowed to use the same letter tile twice for a single word. Can the `word` be found on the lid?
## Examples

### 1

#### Input

[["A","B","C","E"],["S","F","C","S"],["A","D","E","E"]]
"SEE"

#### Output

Yes

#### Explanation

Word Exist's in Grid.
 
### 2

#### Input

[["A","B","C","E"],["S","F","C","S"],["A","D","E","E"]]
"ABCB"

#### Output

No

#### Explanation

Word didn't Exist's in Grid.

## Input Format 

- The first line contains two integers, `m` and `n`, representing the number of rows and columns in the grid.
- The next `m` lines each contain `n` uppercase English letters, representing the `board`.
- The last line contains the `word` to search for.

## Output Format 

- Return `true` if the word exists in the grid. Otherwise `false`.
 

## Constraints 

- 1 ≤ m, n ≤ 5
- 1 ≤ word.length ≤ 5
- `board` and `word` consist of only uppercase English letters.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

backtracking, depth-first-search