# EX 25 C program to check whether a given character is a vowel or consonant using pointer
## DATE:
## AIM:
To write a C program to check whether a given character is a vowel or consonant using pointer

## Algorithm
1.Initialize Variables – Declare a character variable ch and create a pointer ptr to store its address.

2.User Input – Prompt the user to enter an alphabet and store the input using scanf(), utilizing the pointer for input storage.

3.Handle Invalid Input – If the character is not an alphabet, print an error message.

4.Terminate Program – End execution with return 0.

5.Convert to Lowercase – Use tolower() to ensure uniform comparison of letters, making vowel/consonant detection case-insensitive. 

## Program:
```
/*
C program to check whether a given character is a vowel or consonant using pointer
Developed by: 
RegisterNumber:  
*/
int main() {
    char ch;
    char *ptr = &ch;

    printf("Enter an alphabet: ");
    scanf(" %c", ptr);

    *ptr = tolower(*ptr);  // Convert to lowercase for uniform comparison

    if ((*ptr >= 'a' && *ptr <= 'z')) {
        if (*ptr == 'a' || *ptr == 'e' || *ptr == 'i' || *ptr == 'o' || *ptr == 'u') {
            printf("The character '%c' is a vowel.\n", *ptr);
        } else {
            printf("The character '%c' is a consonant.\n", *ptr);
        }
    } else {
        printf("Invalid input. Please enter an alphabet.\n");
    }

    return 0;
}
```

## Output:
![image](https://github.com/user-attachments/assets/ac890097-4b3f-4e10-8bb3-21c7818da21e)



## Result:
Thus the program was executed and the output was verified successfully.
