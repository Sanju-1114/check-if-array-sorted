# Check If Array Is Sorted

This repository contains a C++ program to check if an array is sorted in non-decreasing order using recursion.

## Overview

The program defines a recursive function `isSorted` that checks whether a given array (stored in a `vector<int>`) is sorted in non-decreasing order. It uses a recursive approach to compare adjacent elements and determine if the array is sorted.

- **Time Complexity**: O(n), where n is the size of the array.
- **Space Complexity**: O(n) due to the recursive call stack.

## Files

- **check_ifArrayIsSortedOrNot_usingRecursion.cpp**: The main C++ program that implements the recursive sorting check.

## How It Works

1. The `isSorted` function takes a vector of integers (`nums`) and its size (`n`) as parameters.
2. Base case: If the array has 0 or 1 element (`n == 0` or `n == 1`), it is considered sorted, so the function returns `true`.
3. Recursive case: The function checks if the last element (`nums[n-1]`) is greater than or equal to the second-to-last element (`nums[n-2]`). It then recursively calls itself with `n-1` to check the rest of the array.
4. The main function initializes a sample array `{1, 2, 3, 4, 5}` and calls `isSorted` to check if it is sorted, printing the result (`1` for true, `0` for false).

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/Sanju-1114/check-if-array-sorted.git
   ```
2. Navigate to the project directory:

   ```bash
   cd check-if-array-sorted
   ```
3. Compile the C++ program:

   ```bash
   g++ check_ifArrayIsSortedOrNot_usingRecursion.cpp -o check_sorted
   ```
4. Run the program:

   ```bash
   ./check_sorted
   ```

## Example Output

For the input array `{1, 2, 3, 4, 5}`:

```
1
```

For an unsorted array, e.g., `{1, 3, 2, 4, 5}`:

```
0
```

## Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License.