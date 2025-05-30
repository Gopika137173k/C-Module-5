# Arrays: Matrix Addition in C (Using 2D Arrays)

## 🎯 Aim

To write a C program that adds two matrices using 2-dimensional arrays.

## 🧠 Algorithm

1. **Input**:
   - Read the number of rows and columns.
   - Read elements of Matrix A.
   - Read elements of Matrix B.
2. **Matrix Addition**:
   - Create a third matrix C.
   - For each element `C[i][j]`, compute `C[i][j] = A[i][j] + B[i][j]`.
3. **Output**:
   - Print `"Sum of two matrices:"` followed by elements of Matrix C row by row.

## Progam
```
#include <stdio.h>

int main() {
    int rows, cols;
    int A[10][10], B[10][10], C[10][10];
    int i, j;

    printf("Enter number of rows: ");
    scanf("%d", &rows);

    printf("Enter number of columns: ");
    scanf("%d", &cols);

    printf("Enter elements of Matrix A:\n");
    for (i = 0; i < rows; i++) {
        for (j = 0; j < cols; j++) {
            scanf("%d", &A[i][j]);
        }
    }

    printf("Enter elements of Matrix B:\n");
    for (i = 0; i < rows; i++) {
        for (j = 0; j < cols; j++) {
            scanf("%d", &B[i][j]);
        }
    }

    // Matrix Addition
    for (i = 0; i < rows; i++) {
        for (j = 0; j < cols; j++) {
            C[i][j] = A[i][j] + B[i][j];
        }
    }

    printf("Sum of two matrices:\n");
    for (i = 0; i < rows; i++) {
        for (j = 0; j < cols; j++) {
            printf("%d ", C[i][j]);
        }
        printf("\n");
    }

    return 0;
}
```

## Output
Sample Output 1:
Enter number of rows: 2
Enter number of columns: 2
Enter elements of Matrix A:
1 2
3 4
Enter elements of Matrix B:
5 6
7 8
Sum of two matrices:
6 8
10 12

Sample Output 2:
Enter number of rows: 3
Enter number of columns: 3
Enter elements of Matrix A:
1 0 2
-1 3 1
3 4 5
Enter elements of Matrix B:
2 3 4
1 0 0
1 2 3
Sum of two matrices:
3 3 6
0 3 1
4 6 8

## Result
Program was implemented and executed.
