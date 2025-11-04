## Title

Magic Scroll Word Search

## Slug

magic-scroll-word-search

## Difficulty

Medium

## Description

You have found an ancient magic scroll, represented as a grid of letters. A powerful magic word is hidden inside. You must find out if the word exists on the scroll.

The word can be formed from letters in neighboring cells (up, down, left, or right). You must follow the path of letters in order. You cannot use the same letter cell more than once for a single word. Your task is to write a program that checks if the given `word` can be found on the `board`.
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