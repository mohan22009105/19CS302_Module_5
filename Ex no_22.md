# EX 22 C program to count total number of even elements in an array using calloc().

## AIM:
To write a C program to count total number of even elements in an array using calloc().

## Algorithm
Start.

Define a variables.

Write program to count total number of even elements in an array using calloc().

Read the value using scanf.

Ask the user to make an input.

Print out the answer.

End. 

## Program:
```
#include <stdio.h>
#include <stdlib.h>

int main()
{
    int n, i, count = 0;
    scanf("%d", &n);

    int *a = (int *)calloc(n, sizeof(int));

    for (i = 0; i < n; i++)
        scanf("%d", &a[i]);

    for (i = 0; i < n; i++)
        if (a[i] % 2 == 0)
            count++;

    printf("Total even elements: %d", count);

    free(a);
    return 0;
}
```

## Output:

<img width="1042" height="390" alt="image" src="https://github.com/user-attachments/assets/464c4309-9f22-40d0-afbe-aff4eea932f0" />



## Result:
Thus the program was executed and the output was verified successfully.
