## Title

Binary Droid Sorting

## Slug

binary-droid-sorting

## Difficulty

Medium

## Description

You are the chief engineer on the starship `Odyssey` and must organize a squad of maintenance droids. Each droid has an integer serial number. The droids are sorted based on their "energy priority," which is determined by the number of 1s in the binary representation of their serial number. Droids with fewer 1s (lower energy) go first. If two droids have the same energy priority, the one with the lower serial number goes first. Your task is to return the list of serial numbers in this sorted order.

## Examples

### 1

#### Input

9
[0,1,2,3,4,5,6,7,8]

#### Output

[0,1,2,4,8,3,5,6,7]

#### Explanation

0 bits: [0]
1 bit: [1, 2, 4, 8]
2 bits: [3, 5, 6]
3 bits: [7]

Combining these groups, sorted by bit count and then by value, gives the final order.

### 2

#### Input

11
[1024,512,256,128,64,32,16,8,4,2,1]

#### Output

[1,2,4,8,16,32,64,128,256,512,1024]

#### Explanation

All integers in the input have exactly one '1' bit in their binary representation. Therefore, the tie-breaker rule applies to all of them, and they are sorted in ascending numerical order.

## Input Format  

- The only input line has an integer k.

## Output Format  

- Return the sorted integers array.
  

## Constraints  

- 1 ≤ x ≤ 500
- 1 ≤ a_i ≤ 1e4

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

sorting

## Companies
infosys