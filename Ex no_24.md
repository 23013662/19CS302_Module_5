# EX 24 Create a structure program to read(empno,dept and basic pay) and store the data of 3 employees and calculate their Gross Salary(da =10% and HRA=30% from BP).
## DATE:
## AIM:
To Create a structure program to read(empno,dept and basic pay) and store the data of 3 employees and calculate their Gross Salary(da =10% and HRA=30% from BP).

## Algorithm
1.Define Structure – Create a struct Employee with fields for employee number, department, basic pay, and gross salary.

2.Input Data – Use a loop to collect employee details from the user, storing them in the array.

3.Compute Gross Salary – Calculate gross salary as basicPay + (10% of basicPay) + (30% of basicPay).

4.Display Information – Loop through the stored data and print employee details, including computed salary.

5.End Program – Terminate execution with return 0. 
   

## Program:
```
/*
A structure program to read(empno,dept and basic pay) and store the data of 3 employees and calculate their Gross Salary(da =10% and HRA=30% from BP).
Developed by: 
RegisterNumber:  
*/
#include <stdio.h>

struct Employee {
    int empno;
    char dept[30];
    float basicPay;
    float grossSalary;
};

int main() {
    struct Employee emp[3];
    int i;

    for (i = 0; i < 3; i++) {
        printf("\nEnter details of Employee %d:\n", i + 1);
        printf("Employee Number: ");
        scanf("%d", &emp[i].empno);
        printf("Department: ");
        scanf(" %[^\n]", emp[i].dept);
        printf("Basic Pay: ");
        scanf("%f", &emp[i].basicPay);

        emp[i].grossSalary = emp[i].basicPay + (0.10 * emp[i].basicPay) + (0.30 * emp[i].basicPay);
    }
    printf("\n--- Employee Details with Gross Salary ---\n");
    for (i = 0; i < 3; i++) {
        printf("\nEmployee %d:\n", i + 1);
        printf("Emp No     : %d\n", emp[i].empno);
        printf("Department : %s\n", emp[i].dept);
        printf("Basic Pay  : %.2f\n", emp[i].basicPay);
        printf("Gross Salary: %.2f\n", emp[i].grossSalary);
    }

return 0;
}
```

## Output:
![image](https://github.com/user-attachments/assets/c820b61d-6dc6-4f1f-837a-11c4e44b88f1)



## Result:
Thus the program was executed and the output was verified successfully.
