## Title
Subway Tunnel Lights

## Slug
subway-tunnel-lights

## Difficulty
Medium

## Description
Emergency lights turn on. The tunnel is 'safe' up to point k if lights 1 to k are all on.

There is a sequence of $n$ lights indexed from $1$ to $n$. Initially, all lights are **dark**.

You activate the lights one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you activate the light at the position `sequence[i-1]`.

A state is called **safe** if, after performing $k$ steps, exactly the first $k$ lights (indices $1$ to $k$) are on and all other lights are dark.

Your task is to calculate how many times the system becomes **safe** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "00*00" (Not safe)
- Step 2 (index 2): "0**00" (Not safe)
- Step 3 (index 4): "0***0" (Not safe)
- Step 4 (index 1): "****0" (safe: first 4 are on)
- Step 5 (index 5): "*****" (safe: first 5 are on)
Total safe states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "000*" (Not safe)
- Step 2 (index 1): "*00*" (Not safe)
- Step 3 (index 2): "**0*" (Not safe)
- Step 4 (index 3): "****" (safe)
Total safe states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was safe.

## Constraints
- 1 ≤ n ≤ 10^4
- `sequence` is a permutation of numbers from $1$ to $n$.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy

## Company
google
