## Title

The Scribe's Forgotten Anagrams

## Slug

the-scribes-forgotten-anagrams

## Difficulty

Medium

## Description

In the dusty archives of the Great Library, an ancient scribe has discovered a peculiar stone tablet containing a sequence of runic characters. This sequence, represented as a string `S`, is believed to be a password to a hidden vault.

However, legends say that the true password is not necessarily the sequence found on the tablet, but rather one of the many possible distinct rearrangements of its runes. The scribe knows the specific set of characters, but the order has been lost to time.

Your task is to help the scribe calculate the total number of distinct strings that can be formed using the characters from the found string `S`. Since the number of permutations can be very large, print the result modulo `10^9 + 7`.

## Examples

### 1

#### Input

aabac

#### Output

20

#### Explanation

The string has repeated characters (a appears 3 times).
The number of distinct permutations is calculated by dividing the total permutations by repetitions.
Final number of unique rearrangements is 20.
    
### 2

#### Input

abc

#### Output

6

#### Explanation

The characters are distinct. The permutations are: "abc", "acb", "bac", "bca", "cab", "cba". Total is 6.
  

## Input Format  

- The first and only line of input contains a string `S` consisting of lowercase English letters (a–z).

## Output Format  

- Return one integer: the number of different strings that can be created modulo `10^9+7`.
  

## Constraints  

- 1 ≤ S.length ≤ 1e6

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

dynamic-programming, maths, hash-table, hackwithinfy

## Companies
infosys
