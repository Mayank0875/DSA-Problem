## Title

The Time Traveler's Itinerary

## Slug

the-time-travelers-itinerary

## Difficulty

Medium

## Description

A time traveler has a list of historical eras they wish to visit. Each era is defined by a start year and an end year, represented as a pair `[start, end]`.

Due to the laws of temporal mechanics, the traveler cannot be in two eras simultaneously. Furthermore, a "cooling off" period is required between jumps. Specifically, to travel from an era `[a, b]` to a subsequent era `[c, d]`, the end year of the first era must be **strictly less than** the start year of the second era (i.e., `b < c`).

You can select eras in any order you like to form a valid itinerary. Your goal is to determine the maximum number of eras the traveler can visit in a single sequence.

## Examples

### 1

#### Input

3 
1 2
2 3
3 4

#### Output

2

#### Explanation

The longest chain is `[1, 2] -> [3, 4]`. The traveler cannot visit `[2, 3]` because `2` is not strictly less than `2` (from the first pair) and `3` is not strictly less than `3` (for the next pair).
    
### 2

#### Input

3 
1 2 
7 8 
4 5

#### Output

3

#### Explanation

The eras can be reordered to form the chain `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.
  

## Input Format  

- The first line contains an integer `n`, the number of available eras.
- The next `n` lines each contain two integers, `start` and `end`, representing an era.

## Output Format  

- Return a single integer representing the maximum length of the chain.
  

## Constraints  

- 1 ≤ n ≤ 1000
- -1000 ≤ start < end ≤ 1000

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array, dynamic-programming