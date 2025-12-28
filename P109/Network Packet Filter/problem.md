## Title
Network Packet Filter

## Slug
network-packet-filter

## Difficulty
Easy

## Description
A firewall analyzes a stream of data packets. Each packet has a unique sequence ID. Duplicate IDs indicate a replay attack or network loop.

Your task is to determine if any packet ID appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The packet ID `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All packet IDs are distinct.

## Input Format
- The first line contains a single integer n, the number of packets.
- The second line contains n space-separated integers, representing the packet IDs.

## Output Format
- Return `Yes` if any packet ID appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
