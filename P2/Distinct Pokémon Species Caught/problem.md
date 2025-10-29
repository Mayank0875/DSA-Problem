## Title

Distinct Pokémon Species Caught

## Slug

distinct-pokemon-species-caught

## Difficulty

Easy

## Description

A Pokémon trainer is reviewing their collection. Each Pokémon species has a unique Pokédex number (a numerical ID). The trainer has caught many Pokémon, including duplicates of the same species. To complete their Pokédex, they need to know how many different species they have registered. You are given the list of Pokédex numbers for all the Pokémon the trainer has caught. Determine the total count of unique Pokémon species in their collection.

## Examples

### 1

#### Input

5
[2, 3, 2, 2, 3]

#### Output

2

#### Explanation

The Pokédex numbers are 2, 3, 2, 2, 3. The unique numbers are 2 and 3. The trainer has caught 2 distinct species.

### 2

#### Input

8
[10, 5, 10, 2, 5, 10, 5, 2]

#### Output

3

#### Explanation

The unique numbers are 10, 5, and 2. The trainer has caught 3 distinct species.

## Input Format

- The first line contains an integer n: the total number of Pokémon caught.
- The second line contains $n$ integers x_1, x_2, ...., x_n: the Pokédex numbers.

## Output Format

- Return a single integer: the count of distinct Pokédex numbers.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x_i ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

sorting, set, counting