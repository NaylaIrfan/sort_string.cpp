# sort_string.cpp

# Sort Letters in a String (C++)

A beginner-friendly C++ program that sorts the letters of a string in alphabetical order using bubble sort.

## About

The program reads a full line of text and rearranges its characters in ascending order. It compares neighbouring letters and swaps them if they are in the wrong order, repeating this until the whole string is sorted.

## Example

```
Enter a string: programming
Sorted string: aggimmnoprr
```

```
Enter a string: hello
Sorted string: ehllo
```

## How It Works

1. Read the full line using `getline(cin, str)`.
2. The outer loop repeats the process `n - 1` times (where `n` is the length of the string).
3. The inner loop compares each pair of neighbouring letters, `str[j]` and `str[j + 1]`.
4. If the left letter is greater than the right letter, swap them.
5. After each round, the largest remaining letter moves to its correct place at the end.
6. Print the sorted string.

## Descending Order

To sort from z to a instead, change the comparison in the code from `>` to `<`:

```cpp
if (str[j] < str[j + 1]) {
```

## Things to Note

- Sorting uses ASCII values, so capital letters come before small letters (for example, `bAaB` becomes `ABab`).
- Spaces are also sorted, and they come first because a space has a smaller ASCII value than any letter.
- The STL function `sort(str.begin(), str.end())` from `<algorithm>` can do the same job in one line.

## Concepts Used

- Strings (`string`)
- Input and output (`cin`, `cout`, `getline`)
- Nested `for` loops
- `if` condition
- Swapping two variables using a temporary variable
- Bubble sort

## How to Run

Make sure a C++ compiler such as `g++` is installed.

```bash
# Compile
g++ sort_string.cpp -o sort_string

# Run (Linux / macOS)
./sort_string

# Run (Windows)
sort_string.exe
```

## Project Structure

```
sort-string-cpp/
├── README.md
└── sort_string.cpp
```

## Author

NAYLA IRFAN 
B.Tech CSE

## License

This project is free to use for learning purposes.
