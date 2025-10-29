## Title

Distinct IP Addresses Accessing Server

## Slug

distinct-ip-addresses-server

## Difficulty

Easy

## Description

A network administrator is analyzing server logs to identify unique visitors. Each incoming connection is logged with the source IP address, represented here as a numerical value. Over time, the same IP address might connect multiple times. To understand the breadth of the audience, the administrator needs to count how many distinct IP addresses accessed the server. You are provided with the list of numerical IP address values from the logs. Calculate the number of unique IPs.

## Examples

### 1

#### Input

5
[2, 3, 2, 2, 3]

#### Output

2

#### Explanation

The IP values logged are 2, 3, 2, 2, 3. The unique IPs are 2 and 3. There were 2 distinct source IPs.

### 2

#### Input

8
[10, 5, 10, 2, 5, 10, 5, 2]

#### Output

3

#### Explanation

The unique IPs are 10, 5, and 2. There were 3 distinct source IPs.

## Input Format

- The first line contains an integer n: the total number of connections logged.
- The second line contains $n$ integers x_1, x_2, ...., x_n: the numerical IP address values.

## Output Format

- Return a single integer: the count of distinct IP address values.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x_i ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

sorting, set, counting, networking