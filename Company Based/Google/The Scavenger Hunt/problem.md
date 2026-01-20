## Title

The Scavenger Hunt

## Slug

the-scavenger-hunt

## Difficulty

Medium

## Description

Captain Nova commands a specialized scavenger ship designed to harvest energy from space debris. The ship begins with an initial energy level representing its `mass`. She encounters a field containing $n$ pieces of debris, where the energy value of each piece is listed in an integer array `asteroids`.

To successfully harvest a piece of debris, the ship's current energy must be greater than or equal to the debris's energy value. Once harvested, the debris is converted into fuel, and its energy is added to the ship's total mass.

Captain Nova can choose to harvest the debris in any order. Your task is to determine if it is possible for the ship to harvest every single piece of debris in the field. Return `true` if all debris can be harvested, and `false` otherwise.

## Examples

### 1

#### Input

5
3
4 4 1

#### Output

true

#### Explanation

The ship starts with mass 5.
1. Harvest debris of mass 1. Ship mass becomes $5 + 1 = 6$.
2. Harvest debris of mass 4. Ship mass becomes $6 + 4 = 10$.
3. Harvest debris of mass 4. Ship mass becomes $10 + 4 = 14$.
All debris harvested.
    
### 2

#### Input

3
2
4 5

#### Output

false

#### Explanation

The ship starts with mass 3. The smallest debris has mass 4. Since $3 < 4$, the ship cannot harvest any debris.

## Input Format  

- The first line contains an integer `mass`, the initial mass of the ship.
- The second line contains an integer `n`, the number of asteroids (debris).
- The third line contains `n` space-separated integers representing the `asteroids` array.

## Output Format  

- Return `true` if all asteroids can be destroyed/harvested, otherwise return `false`.
  

## Constraints  

- 1 ≤ mass ≤ 1e5
- 1 ≤ asteroids.length ≤ 1e5
- 1 ≤ asteroids[i] ≤ 1e5

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

greedy, array

## Company
google