# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Selection Sort Algorithm:
1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.
3.	If yes, set the element as the new minimum.
4.	Swap minimum with first unsorted position.
5.	Repeat the steps 2 and 3 for all the elements in the array.
## Insertion Sort Algorithm:
1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.
3.	If yes, move sorted element to the right by 1.
4.	Break the loop and insert X.
5.	Repeat the steps 2 to 4 for sorting all the elements in the array.
## Program:
```
Developed by: T. Gayathri
Reg No: 212223100007
```
i)	#Selection Sort
```
def selection_sort(arr):
    n = len(arr)
    for i in range(n - 1):
        min_index = i
        for j in range(i + 1, n):
            if arr[j] < arr[min_index]:
                min_index = j
        arr[i], arr[min_index] = arr[min_index], arr[i]

arr = eval(input())
selection_sort(arr)
print(arr)
```
ii)	#Insertion Sort
```
def insertion_sort(arr):
    n = len(arr)
    for i in range(1, n):
        key = arr[i]
        j = i - 1
        while j >= 0 and arr[j] > key:
            arr[j + 1] = arr[j]
            j -= 1
        arr[j + 1] = key
arr = eval(input())
insertion_sort(arr)
print(arr)
```
## Output:
![image](https://github.com/gayumee/Sorting-Algorithms/assets/149037327/577719c8-4360-4dd1-abf4-25114d4cd36a)
![image](https://github.com/gayumee/Sorting-Algorithms/assets/149037327/67161ebd-9fdd-4089-bf77-6a404be0b8aa)

## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
