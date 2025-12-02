# EX 21 C program to calculate the area of a triangle using pointer.

## AIM:
To write a C program to calculate the area of a triangle using pointer.

## Algorithm
Start.

Declare three variable value of type float.

Prompt the user to enter values.

Read the values using scanf.

Find the area of triangle using formula

End

## Program:
```
#include <stdio.h>

int main()
{
    float a, b, area;
    float *x = &a, *y = &b;

    scanf("%f %f", x, y);

    area = 0.5 * (*x) * (*y);

    printf("%.2f", area);

    return 0;
}

```

## Output:

<img width="577" height="193" alt="image" src="https://github.com/user-attachments/assets/4541b368-56c9-4530-8594-e15e96d1fdd1" />



## Result:
Thus the program was executed and the output was verified successfully.
