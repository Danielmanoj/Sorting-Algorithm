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
```
''' 
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: MANOJ G
RegisterNumber: 212222240060
'''
def selection_sort(nums):
    for i in range(len(nums)):
        lowest_index=i
        for j in range(i+1,len(nums)):
            if nums[j]<nums[lowest_index]:
                lowest_index=j
        nums[i], nums[lowest_index]= nums[lowest_index],nums[i]     
    
    
    
    
list_of_nums = eval(input())
selection_sort(list_of_nums)
print(list_of_nums)






```
ii)	#Insertion Sort
```
''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: MANOJ G
RegisterNumber: 212222240060
'''
def insertion_sort(nums):
    for i in range(1,len(nums)):
        item=nums[i]
        j=i-1
        while j>=0 and nums[j] >item:
            nums[j+1]=nums[j]
            j-=1
        nums[j+1]=item
        
    
    
    
list_of_nums = eval(input())
insertion_sort(list_of_nums)
print(list_of_nums)






```

## Output:
i) #Selection Sort 
![243064761-4566af56-69e1-4064-9ffa-20889f70643c](https://github.com/Danielmanoj/Sorting-Algorithm/assets/69635071/a3ae84d3-8a75-452a-8836-bc1f15ca1d5b)
ii) #Insertion Sort 
![243064762-1fc4ac86-f30b-471b-bc8c-1b60c085d796](https://github.com/Danielmanoj/Sorting-Algorithm/assets/69635071/d50ab147-d246-412d-9b0c-15c06296a6da)


## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
