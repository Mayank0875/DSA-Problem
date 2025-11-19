## Title
DNA Folding Simulation

## Slug
dna-folding-simulation

## Difficulty
Easy

## Description
A bioinformatics tool simulates RNA folding. Different bonding pairs are represented by different bracket types. For a stable structure, bonds must not cross (pseudoknots are excluded in this simplified model). This means if a bond type starts, any other bonds started after it must finish before the first bond closes. Given a string of bonding sites, check if it represents a stable secondary structure.

## Examples

### 1

#### Input
()[]{}

#### Output
Yes

#### Explanation
All opening brackets have matching closing brackets in the correct order.

### 2

#### Input
([)]

#### Output
No

#### Explanation
The bracket '[' is closed by ')' which is a mismatch in type and nesting order.

## Input Format
- A single line containing a string s consisting only of the characters '(', ')', '{', '}', '[' and ']'.

## Output Format
- Return true (printed as Yes) if the string is valid, and false (printed as No) otherwise.

## Constraints
- 1 ≤ length(s) ≤ 1e5
- s contains only parentheses '()', square brackets '[]', and curly braces '{}'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
stack, string
