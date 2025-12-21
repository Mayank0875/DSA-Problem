## Title
Potion Brewing

## Slug
potion-brewing

## Difficulty
Hard

## Description
Ingredients are mixed in flasks. The effect of the flask is determined by the most potent ingredient ID (mode) present.

The Witch has a collection of $n$ ingredients, where each ingredient is represented by an integer ID.

To stock the shelves, The Witch must partition these ingredients into several non-empty flasks. Every ingredient from the original collection must belong to exactly one flask. From each flask, a "potion effect" is extracted. The potion effect is defined as the **mode** (most frequent element) of the ingredients in that flask. If a flask has multiple ingredients tied for the most frequent appearance, any one of them can be chosen as the potion effect.

The Witch collects all the extracted potion effects to form a final multiset. Your task is to calculate how many distinct final multisets can be created using this process. Two multisets are considered different if the frequency of any ID differs between them.

## Examples

### 1

#### Input
3
1 2 3

#### Output
7

#### Explanation
Any non-empty subset of {1, 2, 3} can be achieved, for a total of 7 multisets.

### 2

#### Input
3
1 2 2

#### Output
4

#### Explanation
We can generate 4 different multisets:
1. Partition into {1, 2, 2} -> potion effect is 2 -> Result {2}.
2. Partition into {1, 2}, {2} -> potion effects 1, 2 or 2, 2 -> Result {1, 2} or {2, 2}. (Wait, if {1, 2} mode can be 1 or 2. If we pick 2, result is {2, 2}).
3. Partition into {1}, {2, 2} -> potion effects 1, 2 -> Result {1, 2}.
4. Partition into {1}, {2}, {2} -> potion effects 1, 2, 2 -> Result {1, 2, 2}.
Total distinct multisets: {2}, {2, 2}, {1, 2}, {1, 2, 2}.

## Input Format
- The first line contains an integer $n$, the number of ingredients.
- The second line contains $n$ space-separated integers representing the ingredient IDs.

## Output Format
- Return a single integer representing the number of different multisets of potion effects possible, modulo $998244353$.

## Constraints
- 1 ≤ n ≤ 5000
- 1 ≤ ID ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math, combinatorics
