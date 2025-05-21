# EX 21 C program to calculate the area of a triangle using pointer.
## DATE:
## AIM:
To write a C program to calculate the area of a triangle using pointer.

## Algorithm
1.Initialize Variables – Declare base, height, and area as floating-point variables and create pointers to store their addresses.

2.User Input – Prompt the user to enter values for base and height, storing them using pointers.

3.Calculate Area – Compute the area using the formula 0.5 * base * height and store the result in the pointer pArea.

4.Display Result – Print the calculated area using the dereferenced pointer.

5.End Program – Terminate execution with return 0.

## Program:
```
/*
C program to calculate the area of a triangle using pointer.
Developed by:santhiya C 
RegisterNumber:212223060247 
*/
#include <stdio.h>

int main() {
    float base, height, area;
    float *pBase = &base, *pHeight = &height, *pArea = &area;

    printf("Enter base of the triangle: ");
    scanf("%f", pBase);

    printf("Enter height of the triangle: ");
    scanf("%f", pHeight);

    *pArea = 0.5 * (*pBase) * (*pHeight);
    printf("Area of the triangle = %.2f\n", *pArea);
    return 0;
}
```

## Output:
![image](https://github.com/user-attachments/assets/06a38b1c-af72-4681-b0d1-bccd67e04e30)



## Result:
Thus the program was executed and the output was verified successfully.
