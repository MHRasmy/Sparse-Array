# Sparse Array

This project provides an implementation of a sparse array using a linked list data structure. It is designed to represent arrays with huge indices but mostly consisting of zeros in a more efficient way.

## Getting Started

To use this project, simply clone the repository and compile the `SparseArray.cpp` file using your preferred C++ compiler. The program will prompt you to enter the size of the array and its elements. You can then perform various operations on the sparse array, such as setting and getting positions, printing the array, and adding arrays.

## Usage

Here are some examples of how to use this program:

```c++
// Create a new sparse array
SparseArray arr;

// Set values at specific positions
arr.set_value(0, 5);
arr.set_value(2, 10);
arr.set_value(4, 15);

// Get values at specific positions
cout << arr.get(0) << endl; // Output: 5
cout << arr.get(1) << endl; // Output: 0

// Print the entire array
arr.print_array(); // Output: [5, 0, 10, 0, 15]

// Add two arrays together
SparseArray arr2;
arr2.set_value(1, 20);
arr2.set_value(3, 25);

SparseArray result = arr.add_arrays(arr2);
result.print_array(); // Output: [5, 20, 10, 25, 15]
```

