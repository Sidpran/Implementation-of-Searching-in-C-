# Implementation-of-Searching-in-C-

Aim: To explore and implement searching algorithms in C++

Software:  
- Mingw C/C++ compiler  
- Visual Studio Code  
- Online C++ compiler

# Program 1. Binary Search
Theory with explanation of the code:

- Binary Search is an efficient divide-and-conquer algorithm for searching in **sorted arrays**.  
- It repeatedly divides the search interval in half to narrow down the target.  
- The middle element is compared with the target value.  
- If the middle element matches the target, the search is successful.  
- If the target is smaller, the search continues in the left half.  
- If the target is larger, the search continues in the right half.  
- Time complexity is O(log n), making it suitable for large datasets.  
- Space complexity is O(1) for the iterative implementation.  
- The array must be sorted before applying binary search.  
- Deterministic and guarantees finding the target if it exists.

Algorithm:  
- Start  
- Accept the number of elements from the user.  
- Input all elements into a vector or array.  
- Sort the array in ascending order.  
- Display the sorted array.  
- Prompt the user to enter the target element.  
- Initialize start and end pointers to the beginning and end of the array.  
- Calculate the middle index.  
- If the middle element equals the target, return its index.  
- If the target is smaller, update `end = middle - 1`.  
- If the target is larger, update `start = middle + 1`.  
- Repeat the above steps until `start > end`.  
- If not found, return -1.  
- Ask the user if they want to search another element and repeat if required.  
- End  

# Program 2. Linear Search
Theory with explanation of the code:

- Linear Search is a simple algorithm to find an element in a list.  
- It checks each element sequentially from start to end.  
- If a match is found, the index is returned immediately.  
- If no match is found, it returns -1.  
- Works on both sorted and unsorted arrays.  
- Time complexity is O(n) for average and worst cases.  
- Best case is O(1) if the element is at the beginning.  
- Space complexity is O(1) since no extra memory is needed.  
- Simple to implement and easy to understand.  
- Suitable for small datasets or when sorting is not feasible.

Algorithm:  
- Start  
- Define the array or list of elements.  
- Set the target element to search for.  
- Begin from the first element of the array.  
- Compare each element with the target.  
- If a match is found, return the index.  
- If no match is found by the end, return -1.  
- Display whether the element was found or not.  
- Repeat for additional search queries if needed.  
- End  

# Conclusion
The two search implementations demonstrate key techniques for locating elements in arrays:  

- **Binary Search** is fast and efficient, working in logarithmic time, but requires a sorted array. It is ideal for large datasets or performance-critical applications.  
- **Linear Search** is simple and works on any array, sorted or unsorted, making it flexible for small or unsorted data.  

Together, they highlight the trade-off between **speed and flexibility**. Understanding both equips programmers with versatile tools and reinforces the importance of selecting the appropriate search method for a given dataset.
