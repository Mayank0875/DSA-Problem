## Title

The Celestial Access Code

## Slug

celestial-access-code

## Difficulty

Hard

## Description

Captain Nova has discovered an ancient alien vault floating in the Andromeda galaxy. The vault is locked by a complex security mechanism that requires a specific access code. The panel displays a massive number $K$ and a divisor $D$.

To unlock the vault, Nova must calculate the count of integers between $1$ and $K$ (inclusive) that satisfy a specific "harmonic" property: the sum of their digits (in base 10) must be perfectly divisible by $D$.

Since the number of valid codes can be astronomical, the vault requires the answer modulo $10^9 + 7$. Can you help Captain Nova determine the correct count to open the vault?

## Examples

### 1

#### Input

30 4

#### Output

6

#### Explanation

The integers between 1 and 30 where the sum of digits is a multiple of 4 are:
4 (sum=4), 8 (sum=8), 13 (sum=4), 17 (sum=8), 22 (sum=4), 26 (sum=8).
There are 6 such numbers.
    
### 2

#### Input

1000000009 1

#### Output

2

#### Explanation

Make sure to print the number modulo 10^9 + 7.
  

## Input Format  

- The first line contains the integer K as a string (since $K$ can be very large).
- - The second line contains the integer $D$.

## Output Format  

- Return one integer: the minimum number of crystals required.
  

## Constraints  

- 1 ≤ K.length ≤ 1e5
- 1 ≤ D ≤ 100

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

dynamic-programming, maths