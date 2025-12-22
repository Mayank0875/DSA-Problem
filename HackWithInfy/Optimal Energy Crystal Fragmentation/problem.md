## Title

Optimal Energy Crystal Fragmentation

## Slug

optimal-energy-crystal-fragmentation

## Difficulty

Hard

## Description

You have discovered a rare raw energy crystal composed of $n$ fused segments. Each segment possesses a specific energy value. To utilize the crystal, you must separate every segment into an individual unit.

The separation process involves splitting the crystal or any of its resulting fragments into two parts. You can choose any fragment consisting of more than one segment and split it at any valid boundary between segments. However, the process consumes energy. The cost of a single split is equal to the sum of the energy values of all segments in the fragment being split. Your task is to determine the minimum total cost required to break the entire crystal down into single isolated segments.

## Examples

### 1

#### Input

5 
2 7 3 2 5

#### Output

43

#### Explanation

One optimal strategy involves splitting the array `[2, 7, 3, 2, 5]` (sum 19) into `[2, 7]` (sum 9) and `[3, 2, 5]` (sum 10). Cost so far: 19.
Then split `[2, 7]` into `[2]` and `[7]`. Cost: 19 + 9 = 28.
Then split `[3, 2, 5]` into `[3, 2]` (sum 5) and `[5]`. Cost: 28 + 10 = 38.
Finally split `[3, 2]` into `[3]` and `[2]`. Cost: 38 + 5 = 43.
    
### 2

#### Input

1
1

#### Output

0

#### Explanation

Already Single Element so cost is 0.
  

## Input Format  

- The first line contains an integer $n$: the number of segments in the crystal.
- The second line contains $n$ integers x_1, x_2, ...., x_n: the energy values of the segments.

## Output Format  

- Return one integer: the minimum total cost to separate all segments.
  

## Constraints  

- 1 ≤ n ≤ 5000
- 1 ≤ x_i ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

dynamic-programming, divide-and-conquer, hackwithinfy

## Companies
infosys