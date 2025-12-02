# EX 24 Create a structure program to read(empno,dept and basic pay) and store the data of 3 employees and calculate their Gross Salary(da =10% and HRA=30% from BP).

## AIM:
To Create a structure program to read(empno,dept and basic pay) and store the data of 3 employees and calculate their Gross Salary(da =10% and HRA=30% from BP).

## Algorithm
Start.

Define a variables.

Create a structure program to read(empno,dept and basic pay) and store the data of 3 employees and calculate their Gross Salary(da =10% and HRA=30% from BP).

Read the value using scanf.

Ask the user to make an input.

Print out the answer.

End.   

## Program:
```
#include <stdio.h>

struct emp
{
    int empno;
    char dept[50];
    float bp;
};

int main()
{
    struct emp e[3];
    int i;

    for (i = 0; i < 3; i++)
        scanf("%d %s %f", &e[i].empno, e[i].dept, &e[i].bp);

    printf("Details of the Employee:\n");

    for (i = 0; i < 3; i++)
    {
        float da = e[i].bp * 0.10;
        float hra = e[i].bp * 0.30;
        float gross = e[i].bp + da + hra;

        printf("%d %s %.0f %.0f %.0f %.2f\n",
               e[i].empno, e[i].dept,
               e[i].bp, da, hra, gross);
    }

    return 0;
}

```

## Output:

<img width="1525" height="586" alt="image" src="https://github.com/user-attachments/assets/294ab7e7-9290-4811-8830-08b9f64cf885" />




## Result:
Thus the program was executed and the output was verified successfully.
