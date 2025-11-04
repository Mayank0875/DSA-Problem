## Title

Museum Heist Path

## Slug

museum-heist-path

## Difficulty

Medium

## Description

A thief is navigating a museum laid out as a `board` (grid). Each room has a letter. The thief's escape plan is a `word`. They must move from room to adjacent room (up, down, left, or right) to spell the `word`. They cannot enter the same room twice. Can they follow the escape plan?
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