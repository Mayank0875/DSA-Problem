## Title

The Harmonic Shield

## Slug

the-harmonic-shield

## Difficulty

Medium

## Description

Agent Alpha is trying to disable a “Harmonic Shield” powered by n energy crystals.
Each crystal has a frequency value ai.
To disable the shield safely, Alpha must create a Pure Resonance.
A Pure Resonance is any non-empty subsequence of crystals whose GCD of all chosen frequencies equals 1.

Your task:
Count how many subsequences have GCD exactly equal to 1.
Two subsequences are different if they use different indices.
Return the result modulo 1,000,000,007.

## Examples

### 1

#### Input

3
1 2 3

#### Output

5

#### Explanation

The valid subsequences are: [1], [1, 2], [1, 3], [1, 2, 3], and [2, 3]. Their GCDs are all 1. The subsequence [2] has GCD 2, and [3] has GCD 3, so they are excluded.
    
### 2

#### Input

4
1 1 1 1

#### Output

15

#### Explanation

Since every element is 1, any non-empty subsequence has a GCD of 1. There are $2^4 - 1 = 15$ such subsequences.
  
## Input Format  

- The only input line has an integer k.

## Output Format  

- The first line contains an integer $n$ (the number of crystals).
- The second line contains $n$ integers $a_1, a_2, \dots, a_n$ representing the frequencies.
  

## Constraints  

- 1 ≤ x ≤ 1e5
- 1 ≤ a_i ≤ 1e5


## Time Limit

2 second

## Memory Limit

256 MB

## Tags

combinatrics, dynamic-programming, maths