## Title

Counting Unique Artifacts

## Slug

counting-unique-artifacts

## Difficulty

Easy

## Description

An archaeologist has unearthed a collection of ancient artifacts. Each artifact is assigned a numerical identification code. However, some artifacts might be duplicates, sharing the same code. The archaeologist needs your help to determine exactly how many unique types of artifacts were found. You are given the list of identification codes for all discovered artifacts.

## Examples

### 1

#### Input

5 
[2, 3, 2, 2, 3]

#### Output

2

#### Explanation

The codes found are 2, 3, 2, 2, 3. The unique codes are 2 and 3. There are 2 distinct artifact types.

### 2

#### Input

8 
[10, 5, 10, 2, 5, 10, 5, 2]


#### Output

2

#### Explanation
The unique codes are 10, 5, and 2. There are 3 distinct artifact types.
  

## Input Format  

- The first line contains an integer n: the total number of artifacts found.
- The second line contains $n$ integers x_1, x_2, ...., x_n: the identification codes of the artifacts.

## Output Format  

- Return a single integer: the count of distinct identification codes.  

## Constraints  

- 1 ≤ n ≤ 1e5
- 1 ≤ x_i ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

sorting, hash-table 
