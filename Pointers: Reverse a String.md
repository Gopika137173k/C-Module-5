# Pointers: Reverse a String Using Pointers in C

## 🎯 Aim

To write a C program that prints a string in reverse using a pointer.

## 🧠 Algorithm

1. **Input**: Read a string from the user.
2. **Reverse String**:
   - Use a pointer to traverse the string to find its length.
   - Then, move the pointer to the last character of the string.
   - Print characters in reverse by decrementing the pointer.
3. **Output**: Display the reversed string.

## Program
```
#include <stdio.h>

int main() {
    char str[100], *ptr;
    int length = 0;

    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);

    // Calculate length excluding newline if present
    ptr = str;
    while (*ptr != '\0' && *ptr != '\n') {
        length++;
        ptr++;
    }

    // Move pointer to last character of the string
    ptr = str + length - 1;

    printf("Reversed string: ");
    while (length--) {
        printf("%c", *ptr);
        ptr--;
    }
    printf("\n");

    return 0;
}
```

## Output
Sample Output 1:
Enter a string: Hello World
Reversed string: dlroW olleH

Sample Output 2:
Enter a string: CProgramming
Reversed string: gnimmargorPC

## Result

Program was implemented and executed.
