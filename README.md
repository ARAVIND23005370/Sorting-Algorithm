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
i)	#Selection Sort
```python
def selection(nums):
    for i in range(len(nums)):
        lowest=i
        for j in range(i+1,len(nums)):
            if nums[j]<nums[lowest]:
                lowest=j
        nums[i],nums[lowest]=nums[lowest],nums[i]
list=eval(input())
selection(list)
print(list)
```
ii)	#Insertion Sort
```python
def insertion_sort(nums):
    for i in range(1,len(nums)):
       item_to_insert=nums[i]
       j=i-1
       while j>=0 and nums[j]>item_to_insert:
           nums[j+1]=nums[j]
           j-=1
           nums[j+1]=item_to_insert
list_of_nums=eval(input())
insertion_sort(list_of_nums)
print(list_of_nums);

```

## Output:
![Screenshot 2023-12-29 212512](https://github.com/ARAVIND23005370/Sorting-Algorithm/assets/148514836/4c804bb4-5279-4d5c-aea3-370f10b3c378)
![Screenshot 2023-12-29 212523](https://github.com/ARAVIND23005370/Sorting-Algorithm/assets/148514836/9184a59d-27e2-475c-8040-e983d41ffe94)

## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
