## Title
Ancient Hieroglyphs

## Slug
ancient-hieroglyphs

## Difficulty
Easy

## Description
Archaeologists found an inscription with paired symbols acting as punctuation. There are three distinct pairs. For the text to be grammatically correct in the ancient language, chunks of text enclosed by these symbols must be perfectly nested. You are given the transcription of these symbols. Determine if the text follows the grammatical rules of the ancient civilization.

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
