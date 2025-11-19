## Title

Previous Brighter Star in Celestial Circuit

## Slug

previous-brighter-star-celestial-circuit

## Difficulty

Easy

## Description

Imagine traveling along a celestial circuit where stars shine with varying brightness. As you hover in front of each star, you look back (to your left) along the circuit and want to know the brightness of the nearest star that is strictly brighter than the one you are currently observing. If all previous stars are dimmer or of equal brightness, or if it's the first star, there is no such brighter star to the left. Your goal is to determine this brighter star's brightness for each position along the circuit.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

Star 0 (30): No previous star. Output -1.  
Star 1 (60): Star 0 (30) is dimmer. Output -1.  
Star 2 (90): Stars 0 (30), 1 (60) are dimmer. Output -1.  
Star 3 (50): Star 2 (90) is the nearest brighter. Output 90.  
Star 4 (80): Star 2 (90) is the nearest brighter. Output 90.  
Star 5 (40): Star 4 (80) is the nearest brighter. Output 80.  
Star 6 (70): Star 4 (80) is the nearest brighter. Output 80.  
Star 7 (50): Star 6 (70) is the nearest brighter. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All stars have equal brightness, so no strictly brighter previous star exists.

## Input Format

The first line contains a single integer n, the number of stars.  
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the brightness of each star.

## Output Format

Return array of integers. The i-th integer should be the brightness of the nearest star j < i such that h_j > h_i. If no such day exists, then -1.

## Constraints

1 ≤ n ≤ 10^5  
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array