# Selection sort and Insertion sort
### NAME: SHYAM S
### REG.NO: 23012478
### DEPT: AIML
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
```

''' 
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: SHYAM S
RegisterNumber: 23012478
'''
def selection_sort(nums):
    for i in range(len(nums)):
        lowest_value_index=i
        for j in range(i+1,len(nums)):
            if nums[j]<nums[lowest_value_index]:
                lowest_value_index=j
        nums[i],nums[lowest_value_index]=nums[lowest_value_index],nums[i]
list_of_nums=eval(input())
selection_sort(list_of_nums)
print(list_of_nums)

```
ii)	#Insertion Sort
```

''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: SHYAM S
RegisterNumber: 23012478
'''
def insertion_sort(nums):
    for i in range(len(nums)):
        item_to_insert=nums[i]
        j=i-1
        while j>=0 and nums[j]>item_to_insert:
            nums[j+1]=nums[j]
            j-=1
        nums[j+1]=item_to_insert
list_of_nums=eval(input())
insertion_sort(list_of_nums)
print(list_of_nums)
    
```

## Output:
![Screenshot 2023-12-30 193607](https://github.com/SridharShyam/Sorting-Algorithm/assets/144871368/c951823d-1021-4d8a-8ce3-b5a4dd7194c5)

![Screenshot 2023-12-30 193630](https://github.com/SridharShyam/Sorting-Algorithm/assets/144871368/f9e9611f-4f05-4cda-be00-88902608309d)

## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
