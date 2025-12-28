## Title
Taxonomy Classification

## Slug
taxonomy-classification

## Difficulty
Easy

## Description
A biologist classifies a species. A Genus is nested within a Family. The classification string must properly close the Genus group before closing the Family group.

A sequence is considered valid if:
    1. Every opening taxonomic rank has a corresponding closing taxonomic rank of the same type.
    2. taxonomic ranks are closed in the correct order (no crossing pairs like `([)]`). An empty string is also considered valid.

Given a string consisting only of these characters, determine if it is valid.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All taxonomic ranks are matched correctly.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The square taxonomic rank `[` is closed by a parenthesis `)` before the parenthesis `(` is closed. This violates the nesting order.

## Input Format
- A single line containing a string s consisting only of the characters '(', ')', '{', '}', '[' and ']'

## Output Format
- Return true if the string is valid, and false otherwise.

## Constraints
- 1 ≤ length(s) ≤ 1e5
- s contains only characters '()', '[]', and '{}'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string
