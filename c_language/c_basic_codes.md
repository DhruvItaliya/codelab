# Abstract
Codelab is initiative taken by our prof. Mosin Hasan sir.

## Pointer related basic questions for C language

1. Quesion:
    ```
    Write a C program that demonstrates how to use a pointer to  an integer.
    (Use pointer syntax)

    - syntax of pointer declaration
    int *pointer;
    pointer = &variable;
    
    ```

    Code:
    ```
   #include <stdio.h>

    int main() {
        int num;
        int *p = &num;
        scanf("Enter an integer: %d",&num)
        printf("Value of num: %d\n", *p);
        return 0;
    }


    ```

    test cases:
    - 1st (Visible to user)
    ```
    Enter an integer: 25
    Value of num: 25


    ```
    - 2nd
    ```
    Enter an integer: -15
    Value of num: -15

    
    ```

    - 3rd
    ```
    Enter an integer: 1000
    Value of num: 1000

    ```

    - 4th
    ```
    Enter an integer: 0
    Value of num: 0

    ```
2. Quesion:
    ```
    Write a C program that uses a pointer to change the value of an integer.
    (Use pointer dereferencing)
    
    - syntax of pointer dereferencing
    
    *pointer = new_value;


    ```

    Code:
    ```
    #include <stdio.h>

    int main() {
        int num;
        int *p = &num;
        scanf("Enter an integer: %d",&num)
        int new_num;
        *p = num;
        scanf("Enter new integer: %d",&new_num)
        printf("New value of num: %d\n", new_num);
        return 0;
    }


    ```

    test cases:
    - 1st (Visible to user)
    ```
    Enter an integer: 10
    Enter new integer: 20
    New value of num: 20

    ```
    - 2nd
    ```
    Enter an integer: -10
    Enter new integer: -20
    New value of num: -20

    ```

    - 3rd
    ```
    Enter an integer: 34
    Enter new integer: 32
    New value of num: 32
    ```

    - 4th
    ```
    Enter an integer: 14343
    Enter new integer:45343
    New value of num: 45343
    ```


3. Quesion:
    ```
    Write a C program that demonstrates the use of a pointer to an array.
    (Use pointer arithmetic)
    
    - syntax of array and pointer
    
    int arr[] = {1, 2, 3};
    int *p = arr;

    ```

    Code:
    ```
    #include <stdio.h>

    int main() {
        int arr[5];
        int *p = arr;
        printf("Enter 5 integers: ");
        for (int i = 0; i < 5; i++) {
            scanf("%d", ptr + i); 
        }

        printf("First element: %d\n", *p);
        printf("Second element: %d\n", *(p + 1));
        return 0;
    }


    ```

    test cases:
    - 1st (Visible to user)
    ```
    Enter 5 Integer: 5 3 8 1 4
    First element: 5
    Second element: 3
    ```
    - 2nd
    ```
    Enter 5 Integer: 10 20 30 40 50
    First element: 10
    Second element: 20
    ```

    - 3rd
    ```
    Enter 5 Integer: 1 2 3 4 5
    First element: 1
    Second element: 2
    ```

    - 4th
    ```
    Enter 5 Integer: -1 -5 -3 -2 -4
    First element: -1
    Second element: -5
    ```

4. Quesion:
    ```
    Write a C program that uses a pointer to a pointer (double pointer).
    (Use pointer-to-pointer syntax)
    
    - syntax of double pointer
    
    int **pp = &p;
    
    ```

    Code:
    ```
    #include <stdio.h>

    int main() {
        int num;
        int *p = &num;
        int **pp = &p;
        scanf("Enter an number: %d",&num)
        printf("Value of num using double pointer: %d\n", **pp);
        return 0;
    }
    


    ```

    test cases:
    - 1st (Visible to user)
    ```
    Enter two integers: 30
    Value of num using double pointer: 30
    
    ```
    - 2nd
    ```
    Enter two integers: 1
    Value of num using double pointer: 1
    
    ```

    - 3rd
    ```
    Enter two integers: 45
    Value of num using double pointer: 45
    ```

    - 4th
    ```
    Enter two integers: 676
    Value of num using double pointer: 676
    ```


5. Quesion:
    ```
    Write a C program that demonstrates pointer arithmetic with an integer array.
    (Use pointer increment)
    
    - syntax of pointer arithmetic
    
    pointer++;

    ```

    Code:
    ```
    #include <stdio.h>

    int main() {
        int arr[5];
        int *ptr = arr;
        
        printf("Enter 5 integers: ");
        
        for (int i = 0; i < 5; i++) {
            scanf("%d", ptr + i); 
        }
        
        p++;  // Move to the next element
        
        printf("Second element: %d\n", *ptr);
        return 0;
    }

    ```

    test cases:
    - 1st (Visible to user)
    ```
    Enter 5 Integer: 5 3 8 1 4
    Second element: 3
    ```
    - 2nd
    ```
    Enter 5 Integer: 10 20 30 40 50
    Second element: 20
    ```

    - 3rd
    ```
    Enter 5 Integer: 1 2 3 4 5
    Second element: 2
    ```

    - 4th
    ```
    Enter 5 Integer: -1 -5 -3 -2 -4
    Second element: -5
    ```

