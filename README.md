Program 1

Aim:

To implement the Selection Sort algorithm in C++.

Theory:

Selection Sort is a simple comparison-based sorting algorithm. 
The idea is to repeatedly find the minimum element (for ascending order) from the 
unsorted part of the array and place it at the beginning.
Works by dividing the array into two parts:
Sorted part (built from the front).
Unsorted part (remaining elements)
Each pass selects the smallest element from the unsorted portion and swaps it with the first unsorted element.
Time Complexity:
Best Case: O(n²)
Average Case: O(n²)
Worst Case: O(n²)
Space Complexity: O(1) (in-place sorting)

Algorithm (Selection Sort):

- Repeat steps for i = 0 to n-2:
- a. Assume minIndex = i.
- b. For j = i+1 to n-1, if arr[j] < arr[minIndex], update minIndex = j.
- c. Swap arr[i] and arr[minIndex].
- End.

Program 2

Aim:
To implement the Bubble Sort algorithm in C++.

Theory:
Bubble Sort is the simplest sorting algorithm that works by repeatedly swapping adjacent 
elements if they are in the wrong order. The largest element “bubbles up” to the
end in each pass.
After each iteration, the next largest element is placed in its correct position.
Best suited for small datasets or when the array is nearly sorted.
Time Complexity:
Best Case: O(n) (when already sorted with optimized version)
Average Case: O(n²)
Worst Case: O(n²)
Space Complexity: O(1)

Algorithm (Bubble Sort):
- Repeat for i = 0 to n-2:
- a. For j = 0 to n-i-2:
- If arr[j] > arr[j+1], swap them.
- End.

Program 3

Aim:
To implement the Quick Sort algorithm in C++.

Theory:
Quick Sort is a divide and conquer algorithm.
It picks an element as a pivot and partitions the array around the pivot.
Elements smaller than the pivot are placed on the left, and elements greater than the pivot are placed on the right.
The process is recursively applied to left and right sub-arrays.
Time Complexity:
Best Case: O(n log n)
Average Case: O(n log n)
Worst Case: O(n²) (when pivot always ends up smallest/largest element, e.g., sorted array without randomization)
Space Complexity: O(log n) (recursive calls)

Algorithm (Quick Sort):

- If low < high:
- a. Choose a pivot (commonly last element).
- b. Partition the array: place pivot in its correct position, elements less than pivot to left, greater to right.
- c. Recursively apply Quick Sort to left and right sub-arrays.
- End.
