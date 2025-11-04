## Title

Labyrinth of Letters

## Slug

labyrinth-of-letters

## Difficulty

Medium

## Description

You are in a labyrinth made of rooms, each marked with a letter. The layout is a `board` (grid). You are given a `word` and must determine if you can walk through the labyrinth to spell it. You can move up, down, left, or right to an adjacent room, but you cannot visit the same room twice on your path. Check if the `word` can be found.
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