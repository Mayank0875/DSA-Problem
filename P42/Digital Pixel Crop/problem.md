## Title
Digital Pixel Crop

## Slug
digital-pixel-crop

## Difficulty
Easy

## Description
You are writing image processing software. You have a raw data stream consisting of a total number of pixels. You need to form the largest possible square image from these pixels without scaling or stretching. Given the total pixel count, determine the width (in pixels) of the largest square image you can construct.

## Examples

### 1

#### Input
10

#### Output
3

#### Explanation
3² = 9 ≤ 10, 4² = 16 > 10

### 2

#### Input
25

#### Output
5

#### Explanation
5² = 25 ≤ 25, 6² = 36 > 25

## Input Format
- A single integer x — the total number of pixels available.

## Output Format
- Return single integer — the maximum possible side length r of the square image that can be built using those pixels.

## Constraints
- 0 ≤ x ≤ 1e9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, math, number-theory
