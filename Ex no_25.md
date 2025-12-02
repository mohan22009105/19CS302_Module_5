# EX 25 C program to check whether a given character is a vowel or consonant using pointer

## AIM:
To write a C program to check whether a given character is a vowel or consonant using pointer

## Algorithm
Start.

Declare a variable value of type char.

Prompt the user to enter a value.

Read the value using scanf.

Find vowel and consonants

End.

## Program:
```
#include <stdio.h>

int main()
{
    char s[100];
    int vowels = 0, consonants = 0;
    char *p;

    fgets(s, sizeof(s), stdin);
    p = s;

    while (*p)
    {
        if (*p >= 'A' && *p <= 'Z')
            *p = *p + 32;

        if (*p >= 'a' && *p <= 'z')
        {
            if (*p == 'a' || *p == 'e' || *p == 'i' || *p == 'o' || *p == 'u')
                vowels++;
            else
                consonants++;
        }
        p++;
    }

    printf("Vowels: %d\nConsonants: %d", vowels, consonants);

    return 0;
}
```

## Output:

<img width="825" height="308" alt="image" src="https://github.com/user-attachments/assets/4a913bda-0552-457b-b8bd-6bf43498f8fe" />




## Result:
Thus the program was executed and the output was verified successfully.
