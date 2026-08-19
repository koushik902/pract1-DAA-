# pract1-DAA-
Summary:
Bubble Sort: Repeatedly compares adjacent elements and swaps them when they are in the wrong order. It has a best-case complexity of O(n) and average/worst-case complexity of O(n²).
Selection Sort: Finds the smallest element from the unsorted portion and places it in the correct position. Its best, average, and worst-case complexity are O(n²).
Insertion Sort: Builds the sorted array one element at a time by inserting each element into its appropriate position. It performs well on nearly sorted data, with a best-case complexity of O(n) and average/worst-case complexity of O(n²).
Merge Sort: Divides the array into smaller parts, recursively sorts them, and merges them. It consistently provides O(n log n) time complexity but requires O(n) additional space.
Quick Sort: Selects a pivot and divides the elements into smaller and larger groups. Its average/best-case complexity is O(n log n), while its worst case is O(n²).

Conclusion:

The comparison shows that Merge Sort and Quick Sort are generally more efficient for large datasets than Bubble Sort, Selection Sort, and Insertion Sort. The first three algorithms have quadratic O(n²) average or worst-case performance, making them less suitable for large inputs. Merge Sort provides a consistent O(n log n) performance, while Quick Sort usually performs very efficiently in practice but can degrade to O(n²) in its worst case.

Therefore, the choice of sorting algorithm depends on the size and nature of the data. For small or nearly sorted datasets, Insertion Sort can be effective, whereas for larger datasets, Merge Sort or Quick Sort is generally preferable. The execution-time measurements also demonstrate how theoretical time complexity translates into practical performance.
