## Title

Palindromic String Division

## Slug

palindromic-string-division

## Difficulty

Medium

## Description

An ancient scroll contains a single, long string of lowercase English letters. An archivist believes the string is a combination of three ancient, smaller words. After some research, they discover that these ancient words were all palindromes. A palindrome is a word that reads the same forwards and backwards, like "racecar" or "madam".

Your task is to determine if the given string `s` can be split into exactly three non-empty, contiguous substrings, where each of the three substrings is a palindrome.

## Examples

### 1

#### Input

abcbdd

#### Output

Yes

#### Explanation

The string can be split as "a" + "bcb" + "dd". All three substrings are non-empty and are palindromes.
    
### 2

#### Input

bcbddxy

#### Output

No

#### Explanation

It is impossible to split this string into three non-empty palindromic substrings.
  

## Input Format  

- The first line contains a single string, `s`.

## Output Format  

- Return the string "Yes" if the string can be split into three non-empty palindromic substrings. Otherwise, return the string "No".
  

## Constraints  

- 1 ≤ s.length ≤ 3000
- `s` consists only of lowercase English letters.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

dynamic-programming, string, palindrome