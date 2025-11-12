## Title

Digital Mirage: Nearest Higher Signal

## Slug

digital-mirage-nearest-higher-signal

## Difficulty

Easy

## Description

Imagine navigating through a corridor of holographic displays, each showing a numeric signal of varying intensity. As you stand before each display, you glance back (to your left) and want to know the intensity of the nearest previous display that emits a strictly stronger signal than the one you are currently observing. If all earlier displays have weaker or equal intensity, or if you are at the first display, there is no such stronger signal to the left. Your goal is to determine this stronger signal's intensity for every position along the corridor.

## Examples

### 1

#### Input

8
[30, 60, 90, 50, 80, 40, 70, 50]

#### Output

[-1, -1, -1, 90, 90, 80, 80, 70]

#### Explanation

Display 0 (30): No previous display. Output -1.  
Display 1 (60): Display 0 (30) is weaker. Output -1.  
Display 2 (90): Displays 0 (30), 1 (60) are weaker. Output -1.  
Display 3 (50): Display 2 (90) is the nearest stronger. Output 90.  
Display 4 (80): Display 2 (90) is the nearest stronger. Output 90.  
Display 5 (40): Display 4 (80) is the nearest stronger. Output 80.  
Display 6 (70): Display 4 (80) is the nearest stronger. Output 80.  
Display 7 (50): Display 6 (70) is the nearest stronger. Output 70.

### 2

#### Input

5
50 50 50 50 50

#### Output

[-1, -1, -1, -1, -1]

#### Explanation

All displays show equal intensity, so no strictly stronger previous display exists.

## Input Format

The first line contains a single integer n, the number of displays.  
The second line contains n space-separated integers h_0, h_1, ..., h_[n-1], representing the intensity of each display.

## Output Format

Return array of integers. The i-th integer should be the intensity of the nearest display j < i such that h_j > h_i. If no such day exists, then -1.

## Constraints

1 ≤ n ≤ 10^5  
1 ≤ h_i ≤ 10^9 for all 0 ≤ i < n.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

stack, array