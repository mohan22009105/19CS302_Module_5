# EX 23 C program to store and display the name, id, age and salary of an employee using structure(using array of structure).
## DATE:
## AIM:
To write a C program to store and display the name, id, age and salary of an employee using structure(using array of structure).

## Algorithm
Start.

Define a variables.

Write program to to store and display the name, id, age and salary of an employee using structure(using array of structure).

Read the value using scanf.

Ask the user to make an input.

Print out the answer.

End.
## Program:
```

#include <stdio.h>

struct emp
{
    int id;
    char name[50];
    int age;
    int salary;
};

int main()
{
    int n, i;
    scanf("%d", &n);

    struct emp e[n];

    for (i = 0; i < n; i++)
        scanf("%d %s %d %d", &e[i].id, e[i].name, &e[i].age, &e[i].salary);

    printf("Employee Details\n");

    for (i = 0; i < n; i++)
        printf("%d %s %d %d\n", e[i].id, e[i].name, e[i].age, e[i].salary);

    return 0;
}

```

## Output:

<img width="1108" height="378" alt="image" src="https://github.com/user-attachments/assets/a2b4e60c-a421-4a42-9e0f-b438f6ecd31f" />




## Result:
Thus the program was executed and the output was verified successfully.
