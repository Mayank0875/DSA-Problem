## Title

Magical Bacteria Growth

## Slug

magical-bacteria-growth

## Difficulty

Easy

## Description

You are a scientist studying a strange type of bacteria. You are given an array of integers nums representing bacteria colonies observed under a microscope. You start your experiment with a single bacterium of size original.

Your experiment follows these steps:

Check if a bacterium of size original exists in the nums array.

If it is found, the bacterium instantly multiplies by two (set original = 2 * original). This new size becomes the target for the next search.

If it is not found, the experiment stops.

You must repeat this process as long as you keep finding the current bacteria size in the array. Return the final size of the bacterium when the process stops.

## Examples

### 1

#### Input

5 3
[5, 3, 6, 1, 12]


#### Output

24

#### Explanation

Start with size 3. It is found in nums. The bacterium doubles to 6.
Search for 6. It is found. The bacterium doubles to 12.
Search for 12. It is found. The bacterium doubles to 24.
Search for 24. It is not found. The process stops.
    
### 2

#### Input

3 4
[2, 7, 9]


#### Output

4

#### Explanation

Start with size 4. It is not found in nums. The process stops immediately.
  

## Input Format  

- The first line contains an integer n and original, the number of observed colonies and original at start.
- The second line contains n space-separated integers representing the nums array.

## Output Format  

- Return single integer representing the final value of original when the process stops.
  

## Constraints  

- 1 ≤ x ≤ 1000
- 1 ≤ nums[i], original ≤ 1000

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array, hashmap