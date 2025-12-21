## Title

The Alchemist's Essences

## Slug

the-alchemists-essences

## Difficulty

Hard

## Description

Zephyr is a master alchemist working with a collection of magical ingredients. He possesses a multiset of $n$ ingredients, where each ingredient is represented by an integer ID.

To create a new potion recipe, Zephyr must partition his ingredients into several non-empty groups (cauldrons). Every ingredient from his original collection must belong to exactly one cauldron. From each cauldron, he extracts the "essence," which is defined as the **mode** of the ingredients in that cauldron. If a cauldron has multiple ingredients tied for the most frequent appearance, any one of them can be chosen as the essence.

Zephyr collects all the extracted essences to form a final multiset. He wants to know how many distinct final multisets he can create using this process. Two multisets are considered different if the frequency of any ingredient ID differs between them.

## Examples

### 1

#### Input

3
1 2 3

#### Output

7

#### Explanation

Any non-empty subset of {1,2,3} can be achieved, for a total of 7 multisets.
    
### 2

#### Input

3
1 2 2

#### Output

4

#### Explanation
We can generate 4 different multisets:

Partition the elements into set {1,2,2}, resulting in multiset {2}.
Partition the elements into sets {1,2},{2}, resulting in multiset {2,2}.
Partition the elements into sets {1},{2,2}, resulting in multiset {1,2}.
Partition the elements into sets {1},{2},{2}, resulting in multiset {1,2,2}.


## Input Format  

- The first line contains an integer $n$, the number of ingredients.
- The second line contains $n$ space-separated integers representing the ingredient IDs.

## Output Format  

- Return a single integer representing the number of different multisets of essences Zephyr can obtain, modulo $998244353$.
  

## Constraints  

- 1 ≤ n ≤ 5000
- 1 ≤ a_i ≤ n

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

dynamic-programming, maths