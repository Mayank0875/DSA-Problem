## Title

Pairing Ingredients for Recipes

## Slug

pairing-ingredients-recipes

## Difficulty

Easy

## Description

A cooking show requires contestants to pair ingredients. Each ingredient has a 'flavor intensity' score. A pair of ingredients (or a single ingredient) can be used in one dish segment. The combined flavor intensity of ingredients in a segment cannot exceed a maximum value `x`. Given the flavor intensities of `n` available ingredients, what is the minimum number of dish segments needed to use all ingredients?

## Examples

### 1

#### Input

4 10
[7, 2, 3, 9]

#### Output

3

#### Explanation

One minimal set of segments:
    - Segment 1: Ingredient with intensity 2 and ingredient with intensity 7 (Total 9 <= 10)
    - Segment 2: Ingredient with intensity 3 (Total 3 <= 10)
    - Segment 3: Ingredient with intensity 9 (Total 9 <= 10)
This requires 3 segments.

### 2

#### Input

5 5
[2, 2, 2, 3, 4]

#### Output

3

#### Explanation

One minimal set of segments:
    - Segment 1: Ingredient with intensity 2 and ingredient with intensity 3 (Total 5 <= 5)
    - Segment 2: Two ingredients with intensity 2 (Total 4 <= 5)
    - Segment 3: Ingredient with intensity 4 (Total 4 <= 5)
This requires 3 segments.

## Input Format

- The first line contains two integers n and x: the number of ingredients and the maximum combined flavor intensity per segment.
- The second line contains n integers p_1, p_2, ..., p_n: the flavor intensity of each ingredient.

## Output Format

- Return a single integer: the minimum number of dish segments required.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x ≤ 1e9
- 1 ≤ p_i ≤ x

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

greedy, sorting, two pointers