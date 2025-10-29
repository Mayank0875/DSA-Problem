## Title

Unique Phone Numbers Called

## Slug

unique-phone-numbers-called

## Difficulty

Easy

## Description

A call center manager is reviewing the outgoing call log. Each phone number is represented as a large integer. The log lists every call made, meaning the same phone number might appear multiple times if it was called repeatedly. The manager wants to know how many distinct phone numbers were contacted. Given the list of all phone numbers called from the log, calculate the count of unique numbers.

## Examples

### 1

#### Input

5
[2, 3, 2, 2, 3]

#### Output

2

#### Explanation

The phone numbers called (represented as integers) are 2, 3, 2, 2, 3. The unique numbers are 2 and 3. Calls were made to 2 distinct numbers.

### 2

#### Input

8
[10, 5, 10, 2, 5, 10, 5, 2]

#### Output

3

#### Explanation

The unique numbers are 10, 5, and 2. Calls were made to 3 distinct numbers.

## Input Format

- The first line contains an integer n: the total number of calls logged.
- The second line contains $n$ integers x_1, x_2, ...., x_n: the phone numbers (as integers).

## Output Format

- Return a single integer: the count of distinct phone numbers called.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x_i ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

sorting, set, counting, logs