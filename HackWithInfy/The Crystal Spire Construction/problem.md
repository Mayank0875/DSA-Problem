## Title

The Crystal Spire Construction

## Slug

crystal-spire-construction

## Difficulty

Medium

## Description

The Master Architects of the High Council are commissioning a new Crystal Spire of infinite glory. The spire must reach a precise total height of $n$ meters.

The construction materials available are enchanted crystal blocks with heights ranging from 1 meter to 6 meters. To ensure the spire's stability, the blocks are stacked one on top of another in a single vertical column. The order in which the blocks are placed matters; a 1-meter block followed by a 2-meter block is a different design from a 2-meter block followed by a 1-meter block.

Your task is to calculate the total number of distinct ways to construct the spire such that its height is exactly $n$ meters. Since the number of possibilities can be astronomical, output the result modulo $10^9 + 7$.

## Examples

### 1

#### Input

8

#### Output

125

#### Explanation

There are 125 distinct sequences of blocks.
    
### 2

#### Input

3

#### Output

4

#### Explanation

There are 4 distinct sequences of blocks.

## Input Format  

- The only input line has an integer n the target height of the spire..

## Output Format  

- Return one integer: the number of ways to build the spire modulo $10^9 + 7$.

## Constraints  

- 1 ≤ n ≤ 1e18

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

dynamic-programming, maths