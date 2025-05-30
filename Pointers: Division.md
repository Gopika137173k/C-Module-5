# # Pointers: Division of Two Numbers Using Pointers in C

## 🎯 Aim

To write a C program that performs the division of two numbers using pointers.

## 🧠 Algorithm

1. **Declare** integer variables `a`, `b`, and `sub`, and pointers `c`, `d`.
2. **Read** values for `a` and `b` from the user.
3. **Assign** the addresses of `a` and `b` to the pointers `c` and `d` respectively.
4. **Calculate** the quotient by dereferencing the pointers:
   ```c
   sub = *c / *d;
5. Print the result (quotient) stored in sub.

## Program
```
#include <stdio.h>

int main() {
    int a, b, sub;
    int *c, *d;

    printf("Enter two integers (a and b): ");
    scanf("%d %d", &a, &b);

    c = &a;
    d = &b;

    if (*d == 0) {
        printf("Division by zero is not allowed.\n");
        return 1;
    }

    sub = *c / *d;

    printf("Quotient = %d\n", sub);

    return 0;
}
```

## Output
Sample Output 1:
Enter two integers (a and b): 10 2
Quotient = 5

Sample Output 2:
Enter two integers (a and b): 15 4
Quotient = 3

## Result
Program was implemented and executed.
