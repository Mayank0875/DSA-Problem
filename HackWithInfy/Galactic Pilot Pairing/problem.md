## Title

Galactic Pilot Pairing

## Slug

galactic-pilot-pairing

## Difficulty

Medium

## Description

The United Space Force is preparing for a major expedition. The fleet consists of $n$ elite pilots and $m$ advanced navigation droids. To operate a Starfighter effectively, a pairing must consist of exactly one pilot and one droid.

However, not every pilot is compatible with every droid due to differences in neural interface protocols. You are given a list of $k$ compatible pairs, where a specific pilot can work with a specific droid.

Your task is to determine the maximum number of Starfighters that can be deployed simultaneously. Each pilot and each droid can be assigned to at most one Starfighter.

## Examples

### 1

#### Input

3 2 4
1 1
1 2
2 1
3 1

#### Output

2

#### Explanation

There are 3 pilots and 2 droids.
    
### 2

#### Input

2 2 1
1 1

#### Output

1

#### Explanation

Only Pilot 1 and Droid 1 are compatible. The maximum number of operational Starfighters is 1.
  

## Input Format  

- The first line contains three integers $n$, $m$, and $k$: the number of pilots, droids, and compatible pairs.
- The pilots are numbered $1, 2, \dots, n$ and the droids are numbered $1, 2, \dots, m$.
- The next $k$ lines describe the compatible pairs. Each line contains two integers $a$ and $b$, indicating that Pilot $a$ and Droid $b$ are compatible.

## Output Format  

- Return one integer: the maximum number of pairs that can be formed.
  

## Constraints  

- 1 ≤ n, m ≤ 500
- 1 ≤ k ≤ 1000
- 1 ≤ a ≤ n
- 1 ≤ b ≤ m

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

graph, hackwithinfy

## Companies
infosys