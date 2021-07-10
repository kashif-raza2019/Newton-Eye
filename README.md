# Algo-Eye
Algorithm Visualizer in Node JS &amp; Angular JS

## From Start: 
### 1. Searching Algorithm
- <a href='#linearSearch'>Linear Search</a>
- <a href='#binarySearch'>Binary Search</a>
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
<h4 id='linearSearch'> Linear Search</h4><br />

- C++ Code of Linear Search for understanding<br />

```cpp
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
<br /><br /><br />
<h4 id='binarySearch'> Binary Search</h4><br />

- C++ Code of Binary Search Algorithm for better understanding<br />

```cpp
/*
  This function will return index, if element found or -1 if not found!
  Avg. Time Complexity: O(logn), Best: O(1) (Element found at index '0')
*/
//Without Recursion
int binarySearch(int arr[MAX], int n, int x){
    int s= 0, e = n;
    while(s<e){
        int mid = (s+e)/2;
        if(arr[mid] == x){
            return mid;
        }else if(arr[mid]> x){
            e = mid - 1;
        }else if(arr[mid]<x){
            s = mid + 1; 
        }
    }
    
    return -1;
    
}
//With Recursion
int binarySearchRecursive(int arr[MAX], int s, int e, int n, int key){
    //Middle Value 
    int mid = (s+e)/2;
    //If Starting Index becomes greater than End Index i.e. element is 
    //not present in array!
    if(s>e){
        return -1;
    }else if(arr[mid] == key){
        //Element if Found at Mid Value
        return mid;
    }else if(arr[mid]>key){
        //Searching First Half of array
        binarySearchRecursive(arr, s, mid-1, n, key);
    }else if(arr[mid]<key){
        //Searching Second Half of Array
        binarySearchRecursive(arr, mid+1, e, n, key);
    }
}
```
