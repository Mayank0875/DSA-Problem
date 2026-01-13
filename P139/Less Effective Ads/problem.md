## Title
Less Effective Ads

## Slug
less-effective-ads

## Difficulty
Medium

## Description
A marketing team analyzes campaigns.

You have a list of $n$ campaigns. Each campaign has two main properties: **reach** and **conversion rate**. You are given a 2D integer array `properties` where `properties[i] = [reach_i, conversion rate_i]` represents the attributes of the $i$-th campaign.

A campaign is considered **less effective** if there exists another campaign that has **both** strictly greater reach and strictly greater conversion rate.

More formally, the $i$-th campaign is less effective if there exists an index $j$ such that `reach_j > reach_i` and `conversion rate_j > conversion rate_i`.

Your task is to return the number of less effective campaigns.

## Examples

### 1

#### Input
3
5 5
6 3
3 6

#### Output
0

#### Explanation
No campaign has strictly greater reach and conversion rate than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first campaign (2, 2) is less effective because the second campaign (3, 3) has strictly greater reach and conversion rate.

## Input Format
- The first line contains an integer $n$, the number of campaigns.
- The next $n$ lines each contain two space-separated integers, representing the reach and conversion rate of a campaign.

## Output Format
- Return a single integer representing the number of less effective campaigns.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ reach, conversion rate ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
