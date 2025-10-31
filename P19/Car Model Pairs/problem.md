## Title

Car Model Pairs

## Slug

car-model-pairs

## Difficulty

Easy

## Description

You are surveying a parking lot. Each car is identified by its model ID (an integer). A 'model pair' exists if you find exactly two cars of that model in the lot. Given the list of all car model IDs, find all paired models. Return the model IDs in increasing order. If no pairs are found, return an empty list.

## Examples

### 1
#### Input
8
1 2 2 3 3 3 4 4

#### Output
2 4

#### Explanation
Model 2 appears twice, Model 4 appears twice. Model 3 appears thrice, Model 1 appears once.

### 2
#### Input
5
5 5 5 6 7

#### Output


#### Explanation
No number appears exactly twice.

## Input Format
- First line: integer n — number of elements.
- Second line: n space-separated integers.

## Output Format
- Return all integers that appear exactly twice in increasing order, as a list/array. If none, return an empty list/array.

## Constraints
- 1 ≤ n ≤ 10^5
- Values fit in 32-bit signed integer

## Time Limit
1 second

## Memory Limit
256 MB

## Tags 
map, sorting