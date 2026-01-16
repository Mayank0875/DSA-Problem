## Title

Vikram's Potion Brewing

## Slug

vikrams-potion-brewing

## Difficulty

Hard

## Description

Vikram is a master alchemist trying to brew a legendary potion. The potion's instability level is given by an integer $n$, which is calculated using two magical ingredients $a$ and $b$ as $n = \frac{a!}{b!}$.

To make the potion safe, Vikram must stabilize it through a series of filtration rounds. In each round, he can choose an integer $x > 1$ such that the current instability $n$ is divisible by $x$. He then reduces the instability to $n / x$. The process stops when the instability reaches 1.

Vikram wants to analyze the potion thoroughly, so he aims to maximize the total number of filtration rounds performed. Your task is to calculate this maximum number of rounds for various pairs of $a$ and $b$.

## Examples

### 1

#### Input

3 1

#### Output

2

#### Explanation

$n = \frac{3!}{1!} = 6$.
Round 1: Choose $x=2$, new $n = 3$.
Round 2: Choose $x=3$, new $n = 1$.
Total rounds: 2.
    
### 2

#### Input

6 3

#### Output

5

#### Explanation

$n = \frac{6!}{3!} = 6 \times 5 \times 4 = 120$.
$120 = 2 \times 2 \times 2 \times 3 \times 5$.
We can divide by prime factors one by one: $2, 2, 2, 3, 5$.
Total rounds: 5.
  

## Input Format  

- The lines contains two integers $a$ and $b$ defining $n = \frac{a!}{b!}$.

## Output Format  

- Return one integer: maximum number of rounds possible.
  

## Constraints  

- 1 ≤ b ≤ a ≤ 1e5

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

math, number-theory