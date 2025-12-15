## Title
Train Track Sabotage

## Slug
train-track-sabotage

## Difficulty
Medium

## Description
Trains carry gold to the vault. Bandits blow up tracks after a train passes.

The railway consists of $n$ stations and $m$ one-way tracks. Each track connects a specific source station to a destination station.

The process happens over several trains. In each train, you must send a train from station 1 (the source) to station $n$ (the destination). The catch is that each track is destroyed by sabotage after one traversal. This means each track can be used at most once across all trains combined.

Your goal is to determine the maximum number of trains you can successfully complete the journey from station 1 to station $n$.

## Examples

### 1

#### Input
6 7
1 2
1 3
2 6
3 4
3 5
4 6
5 6

#### Output
2

#### Explanation
You can complete 2 trains.
Path 1: 1 -> 2 -> 6
Path 2: 1 -> 3 -> 4 -> 6 (or 1 -> 3 -> 5 -> 6)

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
You can complete 1 train.

## Input Format
- The first line contains two integers $n$ and $m$: the number of stations and the number of tracks.
- The next $m$ lines describe the tracks. Each line contains two integers $a$ and $b$, indicating a directed track from station $a$ to station $b$.

## Output Format
- Return one integer: the maximum number of trains possible.

## Constraints
- 1 ≤ n ≤ 500
- 1 ≤ m ≤ 1000
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, breadth-first-search
