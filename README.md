# Algo-Eye
Algorithm Visualizer in Node JS &amp; Angular JS

## From Start: 
### 1. Searching Algorithm
- Linear Search
- Binary Search
- Jump Search
### 2. Sorting Algorithm
- Selection Sort
- Bubble Sort
- Insertion Sort
- Heap Sort
- Quick Sort
- Merge Sort
- Pigeonhole Sort
### 3. Backtracking Algorithm
- Rat in a Maze Solver (Web Game)
- Knight's Tour 
- N-Queen Problem
- Colored Balls Sequence (Permutation)
- Chess** (For Later as a complete Game Human vs Computer)
### 4. Shortest Path Algorithm
- Dijkstr's Shortest Path Algorithm
- Bellman Ford's Algorithm** (For Later)

## Want to collaborate with me for this project?
🖥 Open an issue in this Repository or DM me at kashifraza08012001@gmail.com
<br /><br /><br /><br />
#### Linear Search
- C++ Code of Linear Search for understanding<br />
```
/*
  This function will return index, if element found or -1 if not found!
  Avg. Time Complexity: O(n), Best: O(1) (Element found at index '0')
*/
int linearSearchInt(int arr[MAX], int x){
    int n = sizeof(arr);
    //Base case
    for(int i=0; i<n; i++){
        if(arr[i] == x){
            return i;
        }
    }
    return -1;
}
```
