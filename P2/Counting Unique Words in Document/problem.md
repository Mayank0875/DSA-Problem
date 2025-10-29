## Title

Counting Unique Words in Document

## Slug

counting-unique-words-document

## Difficulty

Easy

## Description

A linguist is analyzing a document to determine its vocabulary richness. For simplicity, each word is represented by a unique numerical code. The document contains many words, and the same word code may appear multiple times. The linguist is interested in the size of the unique vocabulary used, not the total word count. Given the list of numerical word codes as they appear in the document, find the number of distinct word codes present.

## Examples

### 1

#### Input

5
[2, 3, 2, 2, 3]

#### Output

2

#### Explanation

The word codes are 2, 3, 2, 2, 3. The unique codes are 2 and 3. The document uses 2 distinct words.

### 2

#### Input

8
[10, 5, 10, 2, 5, 10, 5, 2]

#### Output

3

#### Explanation

The unique codes are 10, 5, and 2. The document uses 3 distinct words.

## Input Format

- The first line contains an integer n: the total number of words in the document.
- The second line contains $n$ integers x_1, x_2, ...., x_n: the numerical word codes.

## Output Format

- Return a single integer: the count of distinct word codes.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x_i ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

sorting, set, counting, text