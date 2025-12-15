## Title

Signal Amplification Protocol

## Slug

signal-amplification-protocol

## Difficulty

Easy

## Description

An interstellar observatory has detected a mysterious stream of $n$ cosmic radiation bursts. These bursts were received sequentially over time, and each burst has a specific intensity magnitude. The observatory's AI algorithms suggest that a hidden message is embedded within this noise, encoded by an ancient alien civilization.

According to the "Amplification Hypothesis," a valid message segment consists of a sequence of bursts picked from the stream such that each chosen burst is strictly more intense than the one immediately preceding it in the sequence. This rising intensity represents a growing energy signature required to transmit data across galaxies.

You must filter the stream to find the longest possible valid message. You can skip any number of bursts to form the sequence, but you must maintain the original chronological order of the selected bursts. Calculate the maximum number of bursts that can form such a sequence.

## Examples

### 1

#### Input

8
7 3 5 3 6 2 9 8

#### Output

4

#### Explanation

The stream contains intensities: [7, 3, 5, 3, 6, 2, 9, 8]. The longest valid message sequences (strictly increasing) include:
3, 5, 6, 9
3, 5, 6, 8 The length of these sequences is 4.
    
### 2

#### Input

5
5 4 3 2 1

#### Output

1

#### Explanation

Since the intensities are strictly decreasing, we can pick at most 1 burst.
  

## Input Format  

- The first line contains an integer $n$: the number of radiation bursts.
- The second line contains $n$ integers x_1, x_2 ... x_n: the intensity of each burst in chronological order.

## Output Format  

- Return one integer: the length of the longest valid message sequence.
  

## Constraints  

- 1 ≤ n ≤ 2e5
- 1 ≤ x ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, dynamic-programming, greedy, hackwithinfy

## Companies
infosys