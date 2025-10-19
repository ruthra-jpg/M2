# EX-06 - Looping
## AIM:
Write a C program to print even numbers ranging from M to N (including M and N values).

## ALGORITHM:
1.	Declare two integer variables to store the values of M and N.
2.	Use the printf function to prompt the user to enter the values of M and N.
3.	Use the scanf function to read the values of M and N from the user.
4.	Use a loop (for or while) to iterate from M to N.
5.	Inside the loop, check if the current number is even.
6.	If the current number is even, print it.
7.	Continue the loop until you have iterated through all numbers from M to N.

## PROGRAM:
#include<stdio.h>
int main()
{
    int M,N;
    scanf("%d %d",&M,&N);
    for(int i=N; i>=M; i--)
    {
        if(i%3==0)
        printf("%d ",i);
    }
 
    return 0;
}
## OUTPUT:
![WhatsApp Image 2025-10-19 at 17 20 58_adb7ceae](https://github.com/user-attachments/assets/c818505e-9d91-4ee7-86c4-c142b33ec742)

## RESULT:
Thus the program to print even numbers ranging from M to N (including M and N values) has been executed successfully
 
 


# EX-07-Nested-loop

## AIM:

Write a C program to print the given triangular pattern using loop.

## ALGORITHM:

1.	Declare a variable to store the number of rows in the triangle.
2.	Use the printf function to prompt the user to enter the number of rows.
3.	Use a loop (for or while) to iterate through each row.
4.	Inside the loop, use another loop to print the desired number of asterisks for each row.
5.	Continue the loop until you have printed the entire triangular pattern.

## PROGRAM:
#include <stdio.h>
int main()
{
    int N,row,col;
    scanf("%d",&N);
    for(row=1; row<=N; row++)
    {
        for(col=1; col<=N-row+1; col++)
        {
            printf("*");
        }
        printf("\n");
    }
    return 0;
}

## OUTPUT:

![WhatsApp Image 2025-10-19 at 17 22 57_c7f556b3](https://github.com/user-attachments/assets/f169037f-0c0f-4274-a34e-7d0fcfc21e9b)

## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully
 
 


# EX-08-Functions

## AIM:

Write a C program to perform addition and subtraction of two numbers using functions (with argument and without return type).

## ALGORITHM:

1.	Declare two functions, one for addition and one for subtraction. Both functions should take two integer arguments.
2.	Inside the addition & subtraction function, add & subtract the two numbers and print the result.
3.	In the main function, declare two integer variables and read their values from the user.
4.	Call the addition and subtraction functions, passing the two numbers as arguments.

## PROGRAM:
#include <stdio.h>
int addition(int num1, int num2)
{
     int sum;
     sum = num1+num2;
     return sum;
}
int subtraction(int num1, int num2)
{
     int sub;
     sub = num1-num2;
     return sub;
}
int main()
{
     int var1, var2;
     scanf("%d %d",&var1,&var2);
    
     int res = addition(var1, var2);
     int res1 = subtraction(var1, var2);
     printf ("Addition: %d", res);
     printf ("\nSubtraction: %d", res1);
     return 0;
}


## OUTPUT:

![WhatsApp Image 2025-10-19 at 17 25 24_61f9c9ca](https://github.com/user-attachments/assets/3a36d86d-eb18-4dc8-9c7d-51c005d9e4f8)

## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 
 


# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop

## ALGORITHM:

1.	Declare variables to store the input number and the sum of odd digits.
2.	Initialize the sum of odd digits to 0.
3.	Use a for loop to iterate through each digit of the input number.
4.	Inside the loop, extract the rightmost digit of the number (using the modulo operator % and division by 10).
5.	If the digit is odd, add it to the sum of odd digits.
6.	Print the sum of odd digits.

## PROGRAM:
#include <stdio.h>
int main()
{
    int start=10,end=20,sum=0;
    scanf("%d %d",&start,&end);
    
    do
    {
        if(start%2 != 0)
        sum+= start;
        start++;
    }
    
    while(start<end);
    printf("%d",sum);
    return 0;
}

## OUTPUT:

![WhatsApp Image 2025-10-19 at 17 27 35_c11f0556](https://github.com/user-attachments/assets/8ce39b7e-73a7-4327-85b2-2e558ce7321c)

## RESULT:

Thus the program to find the sum of odd digits using for loop has been executed successfully.




# EX – 10 - Factorial of a Number Using a Function
## AIM:
To write a C program that calculates the factorial of a given number using a user-defined function.
## ALGORITHM:
1.	Start
2.	Declare the function fact().
3.	In the main() function, call the fact() function.
4.	In fact() function:
a.	Declare variables i, N, and fact (initialized to 1).
b.	Read an integer N from the user.
c.	Use a for loop from 1 to N:
i.	Multiply fact by i in each iteration.
d.	After the loop, print the factorial value.
5.	End

## PROGRAM:
#include <stdio.h>

void computeFactorial(void)
{
    int num;
    unsigned long long fact = 1ULL;

    printf("Input: ");
    if (scanf("%d", &num) != 1) {
        printf("Invalid input.\n");
        return;
    }

    if (num < 0) {
        printf("Factorial not defined for negative numbers.\n");
        return;
    }

    for (int i = 1; i <= num; i++) {
        fact *= i;
    }

    printf("Factorial value is: %llu\n", fact);
}

int main(void)
{
    computeFactorial();
    return 0;
}

## OUTPUT:
![WhatsApp Image 2025-10-19 at 17 32 03_fc2556a9](https://github.com/user-attachments/assets/143115e6-32ba-47ca-9638-eaaadc030ff5)

## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
