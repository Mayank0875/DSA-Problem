## Title

Parking Lot Check

## Slug

parking-lot-check

## Difficulty

Easy

## Description

A parking lot has `n` spaces in a single row. The `Parking Map` (an array) stores the car model ID for each space. A security alert is triggered if `any two cars of the same model` are parked `within a distance of 'k' spaces` of each other. Your task is to check the `Parking Map` for this security alert.

If an alert is triggered, return `true`; otherwise, return `false`.

## Examples

### 1

#### Input

5
1 0 1 1 3
1

#### Output

true

#### Explanation

The number `1` repeats at indices `2` and `3`, and their distance is `1`, which is ≤ `k (1)`.  
Hence, return `true`. 


### 2

#### Input

6
4 5 6 7 8 4
3

#### Output

false

#### Explanation

The duplicate number `4` appears at indices `0` and `5`.  
The distance between them is `5`, which is greater than `k (3)`.  
Therefore, return `false`.

## Input Format  

- First line: integer `n` — the size of the Cipher Sequence.  
- Second line: `n` space-separated integers — elements of the Cipher Sequence.  
- Third line: integer `k` — the maximum allowed distance between two duplicate numbers.

## Output Format  

Return `true` if there exist two identical numbers within distance `k`, otherwise print `false`.  



## Constraints  

- 1 ≤ n ≤ 1e4  
- −1e9 ≤ nums[i] ≤ 1e9  
- 0 ≤ k ≤ 1e5  

## Time Limit

1 second

## Memory Limit

512 MB

## Tags

arrays, sliding-window