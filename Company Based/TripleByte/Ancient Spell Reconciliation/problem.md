## Title

Ancient Spell Reconciliation

## Slug

ancient-spell-reconciliation

## Difficulty

Medium

## Description

Two ancient magical scrolls, `s1` and `s2`, are believed to contain the same core spell. Unfortunately, over centuries, extra characters have been added to both scrolls. You are an apprentice tasked with reconciling them. To make the scrolls identical, you can delete characters from either scroll. Each deletion has a magical cost equal to the character's ASCII value. Your goal is to find the `minimum total magical cost` required to make the two scrolls equal. The resulting spell (which might be empty) must be identical for both.

## Examples

### 1

#### Input

sea 
eat

#### Output

231

#### Explanation

Deleting "s" from "sea" adds the ASCII value of "s" (115) to the sum.
Deleting "t" from "eat" adds 116 to the sum.
At the end, both strings are equal ("ea"), and 115 + 116 = 231 is the minimum sum possible.
    
### 2

#### Input

delete 
leet

#### Output

403

#### Explanation

Deleting "d", "e", "e" from "delete" leaves "let". Cost: 100 + 101 + 101 = 302.
Deleting "e" from "leet" leaves "let". Cost: 101.
The total cost is 302 + 101 = 403. This is the minimum cost to make both strings equal to "let".
  

## Input Format  

- The first line contains the string `s1`.
- The second line contains the string `s2`.

## Output Format  

- Return single integer representing the minimum total ASCII sum of deleted characters.
  

## Constraints  

- 1 ≤ s1.length, s2.length ≤ 1000
- `s1` and `s2` consist of lowercase English letters.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

dynamic-programming, strings