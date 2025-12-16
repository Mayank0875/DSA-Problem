## Title

Dutch Coalition Building

## Slug

dutch-coalition-building

## Difficulty

Medium

## Description

The process of forming the Dutch government has taken more than half a year for three elections in a row. To streamline the initial stages, we need to analyze potential coalitions.

The first step after election results is to identify a group of parties (called a **coalition**) that holds enough seats to command a strict majority. However, to maintain stability and efficiency, we are interested in coalitions that are "minimal" — meaning they don't contain any parties that aren't strictly necessary for the majority.

Your task is to count the number of **candidate coalitions**. A coalition is considered a candidate coalition if it satisfies two specific criteria:
1.  **Strict Majority:** The total number of seats held by the coalition is strictly greater than half of the total seats across all parties.
2.  **No Superfluous Parties:** The coalition is minimal. This means that removing **any one** party from the coalition would cause the remaining total to drop to half or less of the total seats (losing the strict majority).

## Examples

### 1

#### Input

5
3 1 4 1 5

#### Output

4

#### Explanation

The coalition $\{5, 4, 1\}$ (Sum 10) is not valid because removing 1 leaves 9, which is still a strict majority.
    
### 2

#### Input

4
1 2 3 4

#### Output

3

#### Explanation

Total seats = 10. Majority > 5.
Valid coalitions: $\{4, 2\}$, $\{4, 3\}$, $\{3, 2, 1\}$.
  

## Input Format  

- The first line contains an integer $n$: the number of parties.
- The second line contains $n$ integers p_1, p_2, ...., p_n: the number of seats each party has.

## Output Format  

- Return one integer: the total number of candidate coalitions.
  

## Constraints  

- 1 ≤ n ≤ 60
- 1 ≤ p_i ≤ 1e5

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

maths, dynamic-programming