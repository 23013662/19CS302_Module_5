# EX 22 C program to count total number of even elements in an array using calloc().
## DATE:
## AIM:
To write a C program to count total number of even elements in an array using calloc().

## Algorithm
1.Initialize Variables – Declare an integer pointer, size, counter, and loop variable.

2.Allocate Memory – Use calloc() to allocate memory dynamically for storing integer elements.

3.Check Memory Allocation – If calloc() fails, print an error message and exit.

4.Input Elements – Prompt user for size elements and store them in the allocated memory.

5.Count Even Numbers – Iterate through the array, checking for even numbers and updating the counter.

6.Terminate Program – Free allocated memory and end execution.   

## Program:
```
/*
C program to count total number of even elements in an array using calloc().
Developed by: 
RegisterNumber:  
*/
#include <stdlib.h>
int main() {
    int *arr, size, i, count = 0;

    printf("Enter the number of elements: ");
    scanf("%d", &size);

    arr = (int *)calloc(size, sizeof(int));

    if (arr == NULL) {
        printf("Memory allocation failed.\n");
        return 1;
    }
    printf("Enter %d elements:\n", size);
    for (i = 0; i < size; i++) {
        scanf("%d", &arr[i]);
    }

    for (i = 0; i < size; i++) {
        if (arr[i] % 2 == 0)
```

## Output:
![image](https://github.com/user-attachments/assets/3388309e-afbc-4a3b-b60d-6b7507968dcf)



## Result:
Thus the program was executed and the output was verified successfully.
