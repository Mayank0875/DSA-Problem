## Title

Bob's Pattern Removal Task

## Slug

bobs-pattern-removal-task

## Difficulty

Medium

## Description

Bob is working as a digital archivist and has stumbled upon a strange text processing rule in an ancient manual. The rule describes a procedure to "clean" a text string $s$ using a specific pattern string `part`.

The cleaning process involves the following operation repeated as many times as possible:
Find the **leftmost** occurrence of the substring `part` in $s$ and remove it.

Bob needs to apply this operation until the substring `part` no longer exists in $s$. Note that removing one occurrence might cause the remaining characters to concatenate and form a new occurrence of `part`.

Given the string $s$ and the pattern `part`, help Bob determine the final state of the string after all occurrences have been removed.

## Examples

### 1

#### Input

abbabba
bba

#### Output

a

#### Explanation

In the first example ($s=$ "abbabba", $part=$ "bba"):
Remove "bba" at index 2: "abbbabba" $\to$ "abba".
Remove "bba" at index 1: "abba" $\to$ "a".No more occurrences of "bba". Result is "a".
    
### 2

#### Input

aabbabba
bba

#### Output

aa

#### Explanation

In the Second example ($s=$ "aabbabba", $part=$ "bba"):
Remove "bba" at index 2: "aabbbabba" $\to$ "aabba".
Remove "bba" at index 1: "aabba" $\to$ "aa".No more occurrences of "bba". Result is "aa".
  

## Input Format  

- The first line contains the string $s$.
- The second line contains the string `part`.


## Output Format  

- Return the final string on a single line. If the string becomes empty, output an empty line.
  

## Constraints  

- 1 ≤ s.length ≤ 1000
- 1 ≤ part.length ≤ 1000
- Both strings consist of lowercase English letters.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

string, stack