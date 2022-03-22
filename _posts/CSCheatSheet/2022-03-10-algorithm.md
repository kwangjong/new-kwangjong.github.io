---
layout: post
title: Algorithm
tags: CSCheatSheet, algorithm
date: 2022-03-10 15:32 +0800
toc: true
categories: ComputerScienceCheatSheet
hidden: true
---

## Algorithm Basics
### Iterative Algorithm
An algorithm that performs number of steps repeatedly for a finite number of times. 
* Each repetition is called ***iteration***.
* Uses looping statement like ***for*** and ***while***.
* Mostly used to move through a data set like an array or a list. 


### Recursive Algorithm
An algorithm that calls itself.
* Recursive alorithm is divided into two parts: a ***recursive case*** and a ***base case***.
* ***Recursive case*** is a condition where a recursion is triggered.
* ***Base case*** is a condition that stops the recursion and evaluates the result.
* Often used in Depth First Search


## Search Algorithms
### Linear Search / Sequential Search
A very simple searching algorithm. It starts from one end checking every element until the desired element is found.
* It can be performed in an unsorted list.
* Time Complexity : **O(n<sup>2</sup>)**

![linear-search](https://kwangjong.github.io/CSCheatSheet/img/linear-search.gif)


### Binary Search
A search algorithm that repeatedly divides the search interval in half until the desired element is found or the interval is empty.
* It can only be performed in a sorted list.
* Time Complexity : **O(log n)**

[Implementation](https://github.com/Kwangjong/CSCheatSheet/blob/main/implementation/binary-search.py)

![binary-search](https://kwangjong.github.io/CSCheatSheet/img/binary-search.gif)
  
  
## Sorting Algorithms
### Selection Sort
***Selection Sort*** is a comparison based algorithms. It divides the list into a sorted part and an unsorted part, and repeatedly searches the unsorted part and "select" the smallest or greates element to move from the unsorted part to the end of the sorted part.
* Optimized for small lists (fewer than 10-20elements).
* It may require many comparisions for big lists.
* Time Complexity: **O(n<sup>2</sup>)**

[Implementation](https://github.com/Kwangjong/CSCheatSheet/blob/main/implementation/selection-sort.py)

![selection-sort](https://kwangjong.github.io/CSCheatSheet/img/selection-sort.gif)


### Insertion Sort
***Insertion Sort*** is a comparision based algorithm that searches the sorted part for the next element in the unsorted list to be "inserted".
* Optimized for small lists (fewer than 10-20elements).
* It may require many comparisions for big lists.
* It may require lesser comparision compare to ***selection sort***. ***Insertion sort*** only scans as many as it need to place ith element, while **selection sort*** always scans all elements in the unsorted part. ***Insertion sort*** is typically very efficient for list that are "nearly sorted".
* Time Complexity: **O(n<sup>2</sup>)**

[Implementation](https://github.com/Kwangjong/CSCheatSheet/blob/main/implementation/insertion-sort.py)

![insertion-sort](https://kwangjong.github.io/CSCheatSheet/img/insertion-sort.gif)


### Quick Sort
***Quick Sort*** is a divide and conquer algorithm that recursively partitions the input into low and high parts and sorts each of those parts. A ***pivot*** is any value within the array that divide the data into low and high parts. To partition the input, All values in the low partition are less than or equal to the pivot value, and alll the values in the high partition are greater than or equal to the pivot value. The values in each partition are not necessarily sorted.
* It is fast for the most cases. **O(n log n)**.
* However, if the pivot selected is the smallest or largest element, it results an uneven partitioning. If uneven partitioning happens at every level the runtime is **O(n<sup>2</sup>)**. This rarely happens.
* Time Complexity:
  * Average: **O(n log n)**
  * Worst: **O(n<sup>2</sup>)**

[Implementation](https://github.com/Kwangjong/CSCheatSheet/blob/main/implementation/quick-sort.py)

![quick-sort](https://kwangjong.github.io/CSCheatSheet/img/quick-sort.gif)


### Merge Sort
***Merge Sort*** is a divide and conquer algorithm that divides a list into two halves, recursively sorts each half and merges the sorted halves. Recursive partitioning happens until only one element is in the partition.
* It requires additional memory during merging process.
* It is not highly affected by the distribution of the array given.
* Time Complexity: **O(n)**

[Implementation](https://github.com/Kwangjong/CSCheatSheet/blob/main/implementation/merge-sort.py)

![merge-sort](https://kwangjong.github.io/CSCheatSheet/img/merge-sort.gif)


## Author
All implementations and visual aids are created by me.--If you find any mistakes (syntax, logic, or grammar), criticisms are always welcomed! Feel free to reach out to me.