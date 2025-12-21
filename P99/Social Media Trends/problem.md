## Title
Social Media Trends

## Slug
social-media-trends

## Difficulty
Hard

## Description
Influencers hijack hashtags. Hashtags trend into specific related tags.

Influencer and Troll are playing a strategic game using a trend list $p$ of length $n$. The game starts with a virality of 0.

The players take turns, with Influencer moving first. On each turn, a player chooses an integer $x$ from the trend list that has not been chosen before.
- If it is Influencer's turn, the chosen value $x$ is **added** to the virality.
- If it is Troll's turn, the chosen value $x$ is **subtracted** from the virality.

The rules for choosing $x$ are:
1. On the very first move of the game, Influencer may choose **any** unselected hashtag from the trend list.
2. On every move after the first:
   - Let $m$ be the index of the hashtag chosen in the previous move (that is, the previous player chose $p[m]$).
   - If the value $p[m]$ has not yet been chosen, the current player **must** choose $p[m]$.
   - If $p[m]$ has already been chosen, the current player may choose **any** unselected hashtag.

The game continues until all hashtags of the trend list have been chosen.

Influencer plays optimally to **maximize** the final virality, while Troll plays optimally to **minimize** it.

Your task is to compute the final virality assuming both players play optimally.

## Examples

### 1

#### Input
3
2 3 1

#### Output
4

#### Explanation
Final virality is 4.

### 2

#### Input
2
2 1

#### Output
1

#### Explanation
Final virality is 1.

## Input Format
- The first line contains an integer $n$ (length of trend list).
- The second line contains $n$ space-separated integers $p_1, \dots, p_n$.

## Output Format
- Return one integer: the final virality on a new line.

## Constraints
- 1 ≤ n ≤ 10^6
- 1 ≤ p_i ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, graph, combinatorics
