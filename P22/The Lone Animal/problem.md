## Title

The Lone Animal

## Slug

the-lone-animal

## Difficulty

Medium

## Description

You are helping to board animals onto a giant ark. The animals are lined up, sorted by a unique species ID. Every species is supposed to board in a pair (two of each kind), standing side-by-side. However, one animal is unique and has no pair. Your task is to quickly find the species ID of this single, unpaired animal from the sorted line.

You must write an algorithm with O(log n) runtime complexity.

## Examples

### 1

#### Input

9 
[1, 1, 2, 3, 3, 4, 4, 8, 8]


#### Output

2

#### Explanation

In the sequence [1, 1, 2, 3, 3, 4, 4, 8, 8], the number 2 appears only once.

### 2

#### Input

7 
[3, 3, 7, 7, 10, 11, 11]

#### Output

10

#### Explanation

In the sequence [3, 3, 7, 7, 10, 11, 11], the number 10 appears only once.

## Input Format

- The first line contains an odd integer n, the total number of animals.
- The second line contains n space-separated integers representing the sorted species IDs.

## Output Format

- Return a single integer: the species ID of the animal that appears only once.

## Constraints