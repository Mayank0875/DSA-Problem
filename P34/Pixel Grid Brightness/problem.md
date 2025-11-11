## Title

Pixel Grid Brightness

## Slug

pixel-grid-brightness

## Difficulty

Medium

## Description

An experimental $n \times n$ monitor is being tested. The monitor is organized as a grid of pixels, with rows and columns indexed from 1 to $n$. Each pixel at row $i$ and column $j$ has a specific brightness level calculated as $i \times j$.To calibrate the display, engineers need to find the median brightness value across all $n^2$ pixels. You are given that $n$ is an odd integer. Find this median value.

## Examples

### 1

#### Input

3

#### Output

3

#### Explanation

The numbers in increasing order are [1,2,2,3,3,4,6,6,9], so the median (the 5th element in 1-indexing) is 3.
    
### 2

#### Input

5

#### Output

8

#### Explanation
For n=5, the sorted list has 25 elements. The median is the 13th element (since (25+1)/2=13). The value is 8.
  

## Input Format  

- The only input line has an integer n.

## Output Format  

- Return one integer: the answer to the problem.
  

## Constraints  

- 1 ≤ n ≤ 1e6

## Time Limit

2 seconds

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory<｜begin▁of▁sentence｜>