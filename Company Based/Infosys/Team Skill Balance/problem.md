## Title

Team Skill Balance

## Slug

team-skill-balance

## Difficulty

Medium

## Description

You are a manager at a new tech startup. You have N potential candidates, and each candidate i has a skill rating `ratings[i]`. This rating can be positive (a specialized strength) or negative (a specific weakness). You need to form "balanced teams" of three. A team is balanced if the sum of the ratings of its three distinct members (i, j, k) is exactly zero: `ratings[i] + ratings[j] + ratings[k] == 0`. Your task is to determine the total number of unique triplets of ratings that sum to zero.

## Examples

### 1

#### Input

6 
[-1, 0, 1, 2, -1, -4]

#### Output

2

#### Explanation

The distinct triplets of ratings that sum to 0 are `[-1, 0, 1]` and `[-1, -1, 2]`.
    
### 2

#### Input

3 
[0, 1, 1]


#### Output

0

#### Explanation

The only possible triplet (0, 1, 1) sums to 2, not 0.
  

## Input Format  

- The first line contains a single integer N, the number of candidates.
- The second line contains N space-separated integers, representing the `ratings` array.

## Output Format  

- Return single integer representing the total count of unique triplets that sum to zero.
  

## Constraints  

- 3 ≤ x ≤ 3000
- -1e5 ≤ x ≤ 1e5

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array

## Companies
infosys