## Title

Balanced XML Tags

## Slug

balanced-xml-tags

## Difficulty

Easy

## Description

You are writing an XML parser. A simple XML document consists of $n$ opening tags `<T>` and $n$ closing tags `</T>`. A document is 'well-formed' if all tags are properly nested (e.g., `<T><T></T></T>`). How many different well-formed XML structures can be made with $n$ pairs of tags? You just need to return the total count.
## Examples

### 1

#### Input

3

#### Output

5

#### Explanation

The 5 unique well-formed combinations are:
((()))
(()())
(())()
()(())
()()()

### 2

#### Input

1

#### Output

1

#### Explanation
The only combination is ().

## Input Format  

- The input consists of a single line containing one integer, `n`.

## Output Format  

- Return single integer representing total number of well-formed parenthesis combinations.
  

## Constraints  

- 1 ≤ n ≤ 8

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

backtracking, recursion