# Linear Search and Binary search
## Aim:
To write a program to perform linear search and binary search using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Linear Search:
1.	Start from the leftmost element of array[] and compare k with each element of array[] one by one.
2.	If k matches with an element in array[] , return the index.
3.	If k doesn’t match with any of elements in array[], return -1 or element not found.
## Binary Search:
1.	Set two pointers low and high at the lowest and the highest positions respectively.
2.	Find the middle element mid of the array ie. arr[(low + high)/2]
3.	If x == mid, then return mid.Else, compare the element to be searched with m.
4.	If x > mid, compare x with the middle element of the elements on the right side of mid. This is done by setting low to low = mid + 1.
5.	Else, compare x with the middle element of the elements on the left side of mid. This is done by setting high to high = mid - 1.
6.	Repeat steps 2 to 5 until low meets high
## Program:
i)	#Use a linear search method to match the item in a list.
```
''' 
Program for linear search method to match the item in a list
Developed by: JANARTHANAN V K
RegisterNumber: 212222230051
'''
def linearSearch(array,n,k):
    for i in  range(0,n):
        if(array[i]==k):
            return i
    return -1        
    
array = eval(input())
k = eval(input()) # k-item to be seared for
n=len(array)
array.sort()
result = linearSearch(array,n,k)# use the function for linear search
if(result==-1):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",result)
```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```
''' 
Program to find the element in a list using Binary Search(Iterative Method)..
Developed by: JANARTHANAN V K
RegisterNumber: 212222230051
 
'''
def binarySearchIter(array, k, low, high):
    while low<=high:
        mid=low+(high-low)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
array = eval(input())
# sort the array
array.sort()
k = eval(input()) #k-item to be searched

result=binarySearchIter(array,k,0,len(array)-1)
if result==-1:
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",result)

```
iii)	# Find the element in a list using Binary Search (recursive Method).
```
''' 
Program to find the element in a list using Binary Search (recursive Method).
Developed by: JANARTHANAN V K
RegisterNumber: 212222230051

'''
def BinarySearch(array, k, low, high):
    if high>=low:
        mid=low+(high-low)//2
        if array[mid]==k:
            return mid
        elif array[mid]>k:
            return BinarySearch(array,k,low,mid-1)
        else:
            return BinarySearch(array,k,mid+1,high)
    else:        
        return -1    
array = eval(input())
array.sort()
k = eval(input()) # k is the element to be searched for
result=BinarySearch(array,k,0,len(array)-1)
if result==-1:
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",result)
```
## Sample Input and Output

![Screenshot 2023-06-09 203809](https://github.com/Janarthanan2/Search-Algorithm/assets/119393515/7df24a37-0518-4d1d-a7cd-83938aa64991)

![Screenshot 2023-06-09 204643](https://github.com/Janarthanan2/Search-Algorithm/assets/119393515/03b792cc-9730-4506-8973-917d2dc9a26f)

![Screenshot 2023-06-09 204318](https://github.com/Janarthanan2/Search-Algorithm/assets/119393515/81384b39-f9bf-41a7-94f0-612cf7a3640a)




## Result
Thus the linear search and binary search algorithm is implemented using python programming.
