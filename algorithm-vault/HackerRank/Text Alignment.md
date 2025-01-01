---
Date: 2025-01-01
Link: https://www.hackerrank.com/challenges/text-alignment/problem
tags:
  - String
  - python
---
<iframe src="https://www.hackerrank.com/challenges/text-alignment/problem" style="width: 100%; max-width: 800px; height: auto; aspect-ratio: 1/1; @media (max-width: 600px) { aspect-ratio: 4/5; }"></iframe>

```python
letter = 'H'

blank = " "

width = int(input().strip())

  

# Top Left Triangle

for n in range(width):

## width: 5

## n: 0, 1, 2, 3, 4

## length: 1, 3, 5, 7, 9

line = letter * (2*(n+1)-1)

print(line.center(2*width))

  

# Parallel Block

for n in range(width+1):

block = letter * width

blankSpace = blank * width * 3

line = block + blankSpace + block

print(line.center(6*width))

  

# Horizontal Block

for n in range((width+1) // 2):

line = letter * width * 5

print(line.center(6*width))

  

# Parallel Block

for n in range(width+1):

block = letter * width

blankSpace = blank * width * 3

line = block + blankSpace + block

print(line.center(6*width))

  

# Top Right Triangle

for n in range(width):

## width: 5

## n: 0, 1, 2, 3, 4

## length: 9, 3, 5, 7, 1

line = letter * (2*(width-n)-1)

print(line.center(2*width).rjust(6*width))
```

