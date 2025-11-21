## Title
The Potion Master's Spells

## Slug
the-potion-masters-spells

## Difficulty
Easy

## Description
Alice is a potion master who uses magical runes to cast spells. She has a collection of runes represented by a string, where each character is a specific rune. She also has a spellbook containing a list of possible spells.

To cast a specific spell, Alice must use runes from her collection to form the spell's name. Each rune in her collection can only be used once for a single spell. However, the collection of runes resets after she finishes checking or casting a spell, meaning she can reuse the same collection for the next spell in the book.

Your task is to calculate the total power Alice can generate. A spell is considered "good" if she can form it completely using her runes. The power of a good spell is equal to its length. Return the sum of the lengths of all good spells.

## Examples
### 1
#### Input
4
["cat", "bt", "hat", "tree"]
"atach"
#### Output
6
#### Explanation
The spells that can be formed are "cat" and "hat".
"cat" requires 'c', 'a', 't'. The runes "atach" have all of these.
"hat" requires 'h', 'a', 't'. The runes "atach" have all of these.
"bt" requires 'b', which is missing.
"tree" requires 'r' and 'e', which are missing.
Total power = length("cat") + length("hat") = 3 + 3 = 6.

### 2
#### Input
3
["hello", "world", "code"]
"welldonehoneyr"
#### Output
10
#### Explanation
Alice can form "hello" and "world".
Total power = 5 + 5 = 10.

## Input Format
- The first line contains an integer $n$, the number of spells.
- The second line contains $n$ space-separated strings representing the `words`.
- The third line contains a single string representing the `runes`.

## Output Format
- Return a single integer representing the sum of lengths of all good spells.

## Constraints
- 1 ≤ n ≤ 1000
- 1 ≤ words[i].length, chars.length ≤ 100
- All strings consist of lowercase English letters.

## Time Limit
1 second

## Memory Limit
256 MB

## Tags
string-manipulation, hash-table, counting