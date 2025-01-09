#Two Sum Solution in C++
This repository contains a C++ program to solve the "Two Sum" problem, a common algorithmic challenge where we find indices of two numbers in an array that add up to a given target value.

#Problem Description
The program accepts an array of integers nums and a target integer target, and returns indices of two numbers in the array such that their sum equals the target. Each input has exactly one solution, and the same element cannot be used twice.

#Examples
Input 1:
nums = [2,7,11,15]
target = 9
Output: [0,1]

Input 2:
nums = [3,2,4]
target = 6
Output: [1,2]

Input 3:
nums = [3,3]
target = 6
Output: [0,1]

Constraints
2 <= nums.length <= 10^4
-10^9 <= nums[i] <= 10^9
-10^9 <= target <= 10^9
Only one valid solution exists.

#How to Run the Program

Prerequisites
A C++ compiler (e.g., GCC or the Programiz Online Compiler).
Basic knowledge of running C++ programs.

Steps to Execute:
Clone the repository or download the file main.cpp.
Compile the code using the command:
g++ -o TwoSum main.cpp
Run the executable:
./TwoSum
Follow the prompts to input the size of the array, the elements of the array, and the target value.

#Code Explanation
Approach
The solution uses a Hash Map (unordered_map in C++) to efficiently find the complement of each array element. The steps are:

Traverse the array, and for each element, calculate its complement (target - nums[i]).
Check if the complement exists in the hash map.
If found, return the indices of the current element and the complement.
If not, add the current element to the hash map for future reference.
Complexity
Time Complexity: O(n), where n is the number of elements in the array. Each element is processed at most twice.
Space Complexity: O(n) for storing elements in the hash map.
Example Usage
Input
Enter the size of the array: 4
Enter the elements of the array: 2 7 11 15
Enter the target value: 9
Output
Indices of numbers that add up to the target: [0, 1]
Challenges Faced
Understanding Input Constraints: Ensured that the array size and target are handled appropriately.
Efficient Algorithm: Chose a hash map to achieve O(n) complexity.
