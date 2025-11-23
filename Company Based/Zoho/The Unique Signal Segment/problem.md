## Title

The Unique Signal Segment

## Slug

the-unique-signal-segment

## Difficulty

Medium

## Description

Commander Shepard is analyzing a mysterious distress signal received from the Andromeda galaxy. The signal appears as a stream of characters, including letters, digits, symbols, and spaces.

To triangulate the signal's origin, the ship's AI needs to identify the complexity of the transmission. This is determined by finding the length of the **longest substring** within the signal that contains **no repeating characters**.

A substring is a contiguous sequence of characters within the string. Your task is to help the AI compute this maximum length to lock onto the source coordinates.

## Examples

### 1

#### Input

abcabcbb

#### Output

3

#### Explanation

The answer is "abc", with the length of 3. Other valid substrings like "bca" and "cab" also have length 3.
    
### 2

#### Input

bbbbb

#### Output

1

#### Explanation

The answer is "b", with the length of 1.

## Input Format  

- The input consists of a single line containing the string `s`.

## Output Format  

- Return a single integer representing the length of the longest substring without duplicate characters.
  

## Constraints  

- 1 ≤ length(s) ≤ 1e5

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

string, hash-table
