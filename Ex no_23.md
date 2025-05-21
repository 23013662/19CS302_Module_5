# EX 23 C program to store and display the name, id, age and salary of an employee using structure(using array of structure).
## DATE:
## AIM:
To write a C program to store and display the name, id, age and salary of an employee using structure(using array of structure).

## Algorithm
1.Define Structure – Create a struct Employee containing fields for name, ID, age, and salary.

2.Input Employee Count – Accept the number of employees from the user and dynamically create an array of structures.

3.Store Employee Details – Use a loop to collect name, ID, age, and salary for each employee using scanf().

4.Display Stored Data – Iterate through the array and print all employee details in a formatted output.

5.End Program – Terminate execution using return 0. 

## Program:
```
/*
C program to store and display the name, id, age and salary of an employee using structure(using array of structure).
Developed by: 
RegisterNumber:  
*/
#include <stdio.h>

struct Employee {
    char name[50];
    int id;
    int age;
    float salary;
};

int main() {
    int i, n;

    printf("Enter the number of employees: ");
    scanf("%d", &n);

    struct Employee emp[n];

    for (i = 0; i < n; i++) {
        printf("\nEnter details of employee %d:\n", i + 1);
        printf("Name: ");
        scanf(" %[^\n]", emp[i].name);
        printf("ID: ");
        scanf("%d", &emp[i].id);
        printf("Age: ");
        scanf("%d", &emp[i].age);
        printf("Salary: ");
        scanf("%f", &emp[i].salary);
    }
    printf("\n--- Employee Details ---\n");
    for (i = 0; i < n; i++) {
        printf("\nEmployee %d:\n", i + 1);
        printf("Name: %s\n", emp[i].name);
        printf("ID: %d\n", emp[i].id);
        printf("Age: %d\n", emp[i].age);
        printf("Salary: %.2f\n", emp[i].salary);
    }

    return 0;
}
```

## Output:
![image](https://github.com/user-attachments/assets/de420a33-4602-4c17-93ba-88519fb33498)



## Result:
Thus the program was executed and the output was verified successfully.
