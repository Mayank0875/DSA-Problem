## Title

Bulb Chain Alignment

## Slug

bulb-chain-alignment

## Difficulty

Medium

## Description

There is a row of $n$ light bulbs indexed from $1$ to $n$. Initially, all bulbs are turned **OFF** (0).

You turn the bulbs **ON** (1) one by one in a specific order given by an array `flips`. In the $i$-th step (1-indexed), you turn on the bulb at the position `flips[i-1]`.

A state is called **prefix-aligned** if, after performing $k$ steps, exactly the first $k$ bulbs (indices $1$ to $k$) are ON and all other bulbs are OFF.

Your task is to calculate how many times the row of bulbs becomes prefix-aligned during the entire process.

## Examples

### 1

#### Input

5
3 2 4 1 5

#### Output

2

#### Explanation

- Step 1 (flip 3): "00100" (Not aligned)
- Step 2 (flip 2): "01100" (Not aligned)
- Step 3 (flip 4): "01110" (Not aligned)
- Step 4 (flip 1): "11110" (Aligned: first 4 are ON)
- Step 5 (flip 5): "11111" (Aligned: first 5 are ON)
Total aligned states: 2.
    
### 2

#### Input

4
4 1 2 3

#### Output

1

#### Explanation

- Step 1 (flip 4): "0001" (Not aligned)
- Step 2 (flip 1): "1001" (Not aligned)
- Step 3 (flip 2): "1101" (Not aligned)
- Step 4 (flip 3): "1111" (Aligned)
Total aligned states: 1.
  

## Input Format  

- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `flips`.

## Output Format  

- Return a single integer representing the number of times the state was prefix-aligned.  

## Constraints  

- 1 ≤ n ≤ 1e4
- `flips` is a permutation of numbers from $1$ to $n$.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array

## Company
grab