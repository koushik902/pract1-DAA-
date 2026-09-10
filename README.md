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
# pract2-DAA-
Summary
The binary_search() function repeatedly divides the search range into two halves. It compares the target value with the middle element and eliminates the half of the list where the target cannot exist. This process continues until the target is found or the search range becomes empty.


The program also uses time.perf_counter() to measure and display the execution time of the binary search operation. If the target is found, its index in the sorted list is displayed; otherwise, the program reports that the target was not found.

Time Complexity:

Best Case: O(1)
Average Case: O(log n)
Worst Case: O(log n)
Space Complexity: O(1)

Conclusion
Binary Search is an efficient searching algorithm, especially for large sorted datasets. By eliminating half of the remaining elements after each comparison, it significantly reduces the number of operations required compared with a linear search.

The program demonstrates that Binary Search has a worst-case time complexity of O(log n) and uses constant extra space, making it highly efficient. However, the list must be sorted before searching. Therefore, Binary Search is most beneficial when the data is already sorted or when the same sorted data will be searched multiple times.

# pract3-DAA-
Summary
In the Max-Heap Sort implementation, the elements are converted to negative values because Python's heapq provides a Min Heap by default. The elements are then repeatedly removed from the heap and converted back to positive values, producing the array in descending order. For example, [1, 5, 3] produces [5, 3, 1].

In the Min-Heap Sort implementation, the input list is directly converted into a Min Heap using heapq.heapify(). The smallest element is repeatedly removed from the heap, producing the array in ascending order. For example, [18, 7, 45] produces [7, 18, 45].

Both implementations have:

Best Case: O(n log n)
Average Case: O(n log n)
Worst Case: O(n log n)

The programs also calculate the actual execution time for the sorting operation.
Conclusion
Heap Sort is an efficient sorting technique that provides a consistent O(n log n) time complexity in the best, average, and worst cases. The Min Heap can be used to sort elements in ascending order, while the Max Heap can be used to sort elements in descending order.

The programs demonstrate how heaps can be effectively used for sorting and how Python's heapq module simplifies heap operations. Compared with simpler sorting algorithms such as Bubble Sort and Selection Sort, Heap Sort is generally more suitable for larger datasets because its performance remains O(n log n) even in the worst case.

# pract4-DAA-
Summary
In the Iterative method, a for loop multiplies all integers from 1 to n to calculate the factorial. In the Recursive method, the function repeatedly calls itself with n-1 until it reaches the base case of 0 or 1.

For example, when the input is 5, both methods produce the result 120.

The time complexity of both methods is O(n) because they perform approximately n multiplication operations.

Iterative Time Complexity: O(n)
Recursive Time Complexity: O(n)
Iterative Space Complexity: O(1)
Recursive Space Complexity: O(n), due to the function call stack

The program also compares the execution times of the two approaches.
Conclusion

Both iterative and recursive methods successfully calculate the factorial of a number and have O(n) time complexity. The iterative approach generally uses less memory because it does not require recursive function calls, giving it an advantage for very large values of n.

The recursive approach is simpler and  the concept of recursion, but it requires additional stack memory and may encounter Python's recursion-depth limitation for sufficiently large inputs. Therefore, the iterative method is generally more memory-efficient, while the recursive method is useful for understanding and demonstrating recursive problem-solving.]

# practical-DAA-7
summary:

The Making Change Problem is solved using Dynamic Programming by dividing the problem into smaller subproblems. An array dp stores the minimum number of coins required to make each amount from 0 to the given amount. The solution for a larger amount is obtained using previously calculated smaller amounts. This avoids repeated calculations and makes the algorithm more efficient.

CONCLUSION:

The Dynamic Programming approach provides an efficient solution to the Making Change Problem. It finds the minimum number of coins required to form the target amount and works well when there are many possible combinations of coins. The time complexity is O(n × A), where n is the number of coin denominations and A is the target amount. The space complexity is O(A).

# PRACTICAL-5-DAA
SUMAAARY

The 0/1 Knapsack Problem is solved efficiently using Dynamic Programming by dividing the problem into smaller subproblems. A two-dimensional DP table is used to store the maximum value possible for different numbers of items and capacities. For every item, the algorithm decides whether including or excluding it gives a better result.

# CONCLUSSION
The implementation of the 0/1 Knapsack Problem using Dynamic Programming successfully finds the maximum possible value without exceeding the knapsack's capacity. Dynamic Programming avoids repeated calculations and provides an efficient solution compared with a simple recursive approach. 
This method is useful in resource allocation, budget planning, cargo loading, and other optimization problems.
# Practical_6
# Summary
Matrix Chain Multiplication is an optimization problem where the objective is to 
determine the best order for multiplying a sequence of matrices.
Dynamic Programming is used to store the minimum multiplication cost of smaller,
matrix chains and reuse those results to solve larger chains efficiently.

# Conclusion
The Matrix Chain Multiplication problem using Dynamic Programming successfully. 
finds the minimum number of scalar multiplications required to multiply a sequence of matrices.
By solving smaller subproblems and storing their results in a DP table, 
The algorithm avoids repeated calculations and provides an efficient solution with O(n³) time complexity
