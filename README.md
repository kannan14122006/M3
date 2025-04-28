# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <math.h>

// Function to calculate EMI (with arguments, no return value)
void calculateEMI(float principal, float annualRate, int months) {
    float monthlyRate = annualRate / (12 * 100);  // Convert annual rate to monthly
    float emi;

    emi = (principal * monthlyRate * pow(1 + monthlyRate, months)) /
          (pow(1 + monthlyRate, months) - 1);

    printf("Monthly EMI is: %.2f\n", emi);
}

int main() {
    float principal, annualRate;
    int months;

    // Input from user
    printf("Enter the loan amount: ");
    scanf("%f", &principal);

    printf("Enter the annual interest rate (in %%): ");
    scanf("%f", &annualRate);

    printf("Enter the loan tenure (in months): ");
    scanf("%d", &months);

    // Call EMI calculator function
    calculateEMI(principal, annualRate, months);

    return 0;
}
```
## OUTPUT


![image](https://github.com/user-attachments/assets/e163e9a4-e3a3-4692-934f-e6c47369ba7e)



## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n = 6;            // Number of terms
    int first = 0, second = 1, next;

    printf("Fibonacci Series for %d terms:\n", n);

    for (int i = 1; i <= n; i++) {
        printf("%d ", first);
        next = first + second;
        first = second;
        second = next;
    }

    printf("\n");
    return 0;
}
```

## OUTPUT




![image](https://github.com/user-attachments/assets/d7897cc4-49c3-495e-8ae1-e6596cc3599e)




## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n;

    // Ask user for number of elements
    printf("Enter the number of elements: ");
    scanf("%d", &n);

    int arr[n];  // Declare array of size n

    // Read elements into the array
    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    // Print the last element
    printf("Last element of the array is: %d\n", arr[n - 1]);

    return 0;
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/04728705-144b-4637-879e-ecb170a2df11)








## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n, count = 0;

    // Input number of elements
    printf("Enter the number of elements: ");
    scanf("%d", &n);

    int arr[n];

    // Read array elements
    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);

        // Check if element is positive
        if (arr[i] > 0) {
            count++;
        }
    }

    // Output the count of positive elements
    printf("Total number of positive elements: %d\n", count);

    return 0;
}
```


## OUTPUT
![image](https://github.com/user-attachments/assets/7df1c37d-14a0-4c21-950f-b9733b8b6b69)





## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
```
#include <stdio.h>

int main() {
    int n;

    // Input number of elements
    printf("Enter the number of elements: ");
    scanf("%d", &n);

    int arr[n];

    // Input array elements
    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    // Output with 'E' in place of even numbers
    printf("Modified array:\n");
    for (int i = 0; i < n; i++) {
        if (arr[i] % 2 == 0) {
            printf("E ");
        } else {
            printf("%d ", arr[i]);
        }
    }

    printf("\n");
    return 0;
}
```
## Output:
 
![image](https://github.com/user-attachments/assets/5c0da27c-7344-4edd-bec8-8c502521ca7c)


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



