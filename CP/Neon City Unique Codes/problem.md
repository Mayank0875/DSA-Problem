## Title

Neon City Unique Codes

## Slug

neon-city-unique-codes

## Difficulty

Hard

## Description

In the futuristic Neon City, every building is assigned a unique identification number. The city planners are obsessed with aesthetics and visual clarity. To prevent short circuits in the neon signage and to ensure the numbers are easy to read from a distance, they established a strict rule: no two adjacent digits in a building's ID number can be the same.

For example, the ID `12321` is valid because no digits repeat side-by-side. However, the ID `1223` is invalid because the digit `2` appears twice consecutively.

You are given a range of potential ID numbers from $a$ to $b$ (inclusive). Your task is to calculate exactly how many integers in this range are valid according to the city's rules.

## Examples

### 1

#### Input

123 321

#### Output

171

#### Explanation

There are 171 integers between 123 and 321 (inclusive) that do not have any identical adjacent digits.
    
### 2

#### Input

5 5

#### Output

1

#### Explanation

There are 1 integers between 5 and 5 (inclusive) that do not have any identical adjacent digits.  

## Input Format  

- The input contains two space-separated integers, $a$ and $b$.

## Output Format  

- Return single integer representing the count of valid numbers in the range $[a, b]$.
  

## Constraints  

- 0 ≤ a ≤ b ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

dynamic-programming, maths