## Title

Music Harmony Score

## Slug

music-harmony-score

## Difficulty

Medium

## Description

A composer is exploring harmonies using $n$ musical notes (ranked 1 to $n$) and $n$ instruments (ranked 1 to $n$). The "harmony score" of playing note $i$ on instrument $j$ is $i \times j$.The composer needs to find the median harmony score from all $n^2$ note-instrument pairs to understand the typical sound. Given $n$ is an odd integer, find this value.

## Examples

### 1

#### Input

3

#### Output

3

#### Explanation

The numbers in increasing order are [1,2,2,3,3,4,6,6,9], so the answer is 3. 
    
### 2

#### Input

5

#### Output

8

#### Explanation
The middle element is 8.
  

## Input Format  

- The only input line has an integer n.

## Output Format  

- Return one integer: the answer to the task.
  

## Constraints  

- 1 ≤ x ≤ 1e6

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory