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



```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```





```
iii)	# Find the element in a list using Binary Search (recursive Method).
```





```
## Sample Input and Output

![Screenshot 2023-06-09 203809](https://github.com/Janarthanan2/Search-Algorithm/assets/119393515/7df24a37-0518-4d1d-a7cd-83938aa64991)

![Screenshot 2023-06-09 204046](https://github.com/Janarthanan2/Search-Algorithm/assets/119393515/9032cd90-2ec2-483a-b3a2-a9e4ea26a107)




## Result
Thus the linear search and binary search algorithm is implemented using python programming.
