## Title

Connecting Runes

## Slug

connecting-runes

## Difficulty

Medium

## Description

You have a stone tablet, a `board` (grid) of runes (letters). A magic `word` is formed by connecting adjacent runes (horizontally or vertically). The same rune (cell) cannot be part of the connection twice. Write a function to check if the `word` is on the tablet.
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