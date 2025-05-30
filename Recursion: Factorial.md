# 🔁 Recursion: (Factorial) Calculator in C

## 🎯 Aim

To write a C program to calculate the product (factorial) of a given natural number using recursion.

## 🧠 Algorithm

1. **Define** a function `find_factorial(int n)` that recursively calculates the factorial.
2. **Check** if `n == 0`, return `1` (base case, since 0! = 1).
3. **Otherwise**, return `n * find_factorial(n - 1)`.
4. In `main()`:
   - **Read** an integer `num` from the user.
   - **Call** `find_factorial(num)` and store the result in `fact`.
   - **Print** the result.

## Program
```
#include <stdio.h>

int find_factorial(int n) {
    if (n == 0)
        return 1;
    else
        return n * find_factorial(n - 1);
}

int main() {
    int num, fact;

    printf("Enter a natural number: ");
    scanf("%d", &num);

    if (num < 0) {
        printf("Factorial is not defined for negative numbers.\n");
    } else {
        fact = find_factorial(num);
        printf("Factorial of %d is %d\n", num, fact);
    }

    return 0;
}
```


## Output
Sample Output 1:
Enter a natural number: 5
Factorial of 5 is 120

Sample Output 2:
Enter a natural number: 0
Factorial of 0 is 1

## Result
Program was implemented and executed.
