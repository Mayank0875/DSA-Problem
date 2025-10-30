## Title

Army Squad Reassignment

## Slug

army-squad-reassignment

## Difficulty

Medium

## Description

An army has N squads, with `A[i]` soldiers in the i-th squad. A drill sergeant wants to divide all squads into equal-sized "fireteams". This is only possible if the squad sizes share a common divisor. The sergeant can reassign exactly one squad, changing its size to any number between 1 and 10⁹. What is the maximum possible fireteam size (GCD of all squad sizes) the sergeant can achieve?

## Examples

### 1

#### Input

3 
[7, 6, 8]

#### Output

2

#### Explanation

If the sergeant reassigns the squad of 7 to be a squad of 4, the squads [4, 6, 8] can all be divided into fireteams of size 2.

### 2

#### Input

2
[100, 100]

#### Output

100

#### Explanation

The sergeant can "reassign" a squad to have the same size it already has.

## Input Format

- First line: integer 'n' representing the number of elements written on the blackboard .  
- Second line: 'n' integers representing the elements that are written on blackboard.
- You will be given the array as an input to your function

## Output Format

- Return an integer representing the greatest common divisor after making your move.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ arr[i] ≤ 10^9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, prefix sum, suffix sum, math