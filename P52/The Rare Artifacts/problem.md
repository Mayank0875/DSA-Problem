## Title

The Rare Artifacts

## Slug

the-rare-artifacts

## Difficulty

Easy

## Description

An archaeologist has discovered a chest filled with ancient artifacts, where each artifact is identified by an integer value. The archaeologist wants to arrange these items for a museum display based on their rarity.

The sorting rule is strictly defined: artifacts that appear less frequently in the collection are considered rarer and must be placed first. However, if two different types of artifacts have the same frequency count, the one with the higher identification number is deemed more prestigious and should be placed before the lower one. Your task is to help the archaeologist sort the collection of artifacts according to these rules.

## Examples

### 1

#### Input

6
[1, 1, 2, 2, 2, 3]

#### Output

[3, 1, 1, 2, 2, 2]

#### Explanation

'3' has a frequency of 1, '1' has a frequency of 2, and '2' has a frequency of 3. They are sorted by increasing frequency.
    
### 2

#### Input

5
[2, 3, 1, 3, 2]

#### Output

[1, 3, 3, 2, 2]

#### Explanation

'1' has a frequency of 1. Both '2' and '3' have a frequency of 2. Since they have the same frequency, '3' is placed before '2' because it has a larger value.
  

## Input Format  

- The first line contains a single integer $n$, representing the number of artifacts.
- The second line contains $n$ space-separated integers representing the artifacts.

## Output Format  

- Return the sorted array of integers.
  

## Constraints  

- 1 ≤ n ≤ 100
- -100 ≤ nums[i] ≤ 100

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array, hash-table