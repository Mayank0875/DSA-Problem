## Title

Enchanted Scroll Word Hunt

## Slug

enchanted-scroll-word-hunt

## Difficulty

Medium

## Description

You discover an ancient enchanted scroll covered with letters arranged in a grid. Somewhere within this grid, a hidden magic word is waiting to be found.
Your task is to determine whether the given word can be formed by moving through the grid one letter at a time, using only adjacent cells (up, down, left, or right).

You must follow the letters of the word in order, and no cell may be used more than once while forming the word.

Return true if the word can be found in the grid. Otherwise, return false.

## Examples

### 1

#### Input

[["A","B","C","E"],["S","F","C","S"],["A","D","E","E"]]
"SEE"

img(https://d3gmywgj71m21w.cloudfront.net/coding-questions/f38bb29e6cb34c8047e1d947df307df4)




#### Output

Yes

#### Explanation

img(https://d3gmywgj71m21w.cloudfront.net/coding-questions/39c703039d6f54dd1fd9c6d7641b2b5e)


Word Exist's in Grid.
    
### 2

#### Input

[["A","B","C","E"],["S","F","C","S"],["A","D","E","E"]]
"ABCB"

img(https://d3gmywgj71m21w.cloudfront.net/coding-questions/f38bb29e6cb34c8047e1d947df307df4)




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

backtracking, breadth-first-search