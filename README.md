# EX-06 - Looping
## AIM:
Write a C program to print  numbers ranging from M to N (including M and N values).

## ALGORITHM:
```
1.	Declare two integer variables to store the values of M and N.
2.	Use the printf function to prompt the user to enter the values of M and N.
3.	Use the scanf function to read the values of M and N from the user.
4.	Use a loop (for or while) to iterate from M to N.
5.	If the current number is even, print it.
6.	Continue the loop until you have iterated through all numbers from M to N.
```

## PROGRAM:
```
#include<stdio.h>
int main()
{   int i,m,n;
    scanf("%d%d",&m,&n);
    for(i=m;i<=n;i++)
       printf("%d ",i);
 
    return 0;
}
```

## OUTPUT: 

![Screenshot 2025-04-29 193808](https://github.com/user-attachments/assets/5c649d79-876c-469c-aeef-9b40c3a53f31)

## RESULT:
Thus the program to print numbers ranging from M to N (including M and N values) has been executed successfully
 
 

# EX-07-Nested-loop

## AIM:

Write a C program to print the given triangular pattern using loop.

## ALGORITHM:
```
1.	Declare a variable to store the number of rows in the triangle.
2.	Use the printf function to prompt the user to enter the number of rows.
3.	Use a loop (for or while) to iterate through each row.
4.	Inside the loop, use another loop to print the desired number of asterisks for each row.
5.	Continue the loop until you have printed the entire triangular pattern.
```
## PROGRAM:
```
# include <stdio.h>
int main(){
    int i,j,n;
    scanf("%d",&n);
    for(i=1;i<=n;i++){
       for(j=n;j>=i;j--){
          printf("A");
   }
     printf("\n");
}
    return 0;
}
```

## OUTPUT:

![Screenshot 2025-04-29 194122](https://github.com/user-attachments/assets/588dd39f-3edb-41d9-b7d5-be3f2a7dfe02)

## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully
 
 

# EX-08-Functions

## AIM:

Write a C program to perform addition and subtraction of two numbers using functions (with argument and without return type).

## ALGORITHM:
```
1.	Declare two functions, one for addition and one for subtraction. Both functions should take two integer arguments.
2.	Inside the addition & subtraction function, add & subtract the two numbers and print the result.
3.	In the main function, declare two integer variables and read their values from the user.
4.	Call the addition and subtraction functions, passing the two numbers as arguments.
```
## PROGRAM:
```
# include <stdio.h>
void addition(int n1,int n2)
{
    int add;
    add=n1+n2;
    printf("Addition: %d\n",add);
}
void subtraction(int n1,int n2)
{
    int sub;
    sub=n1-n2;
    printf("Subtraction: %d\n",sub);
}
int main()
{
    int n1,n2;
    scanf("%d%d",&n1,&n2);
    addition(n1,n2);
    subtraction(n1,n2);
    return 0;
}
```

## OUTPUT:

![Screenshot 2025-04-29 194320](https://github.com/user-attachments/assets/853a8c0a-9b38-419a-92fa-51ada83acd5d)

## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 
 

# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop

## ALGORITHM:
```
1.	Declare variables to store the input number and the sum of odd digits.
2.	Initialize the sum of odd digits to 0.
3.	Use a for loop to iterate through each digit of the input number.
4.	Inside the loop, extract the rightmost digit of the number (using the modulo operator % and division by 10).
5.	If the digit is odd, add it to the sum of odd digits.
6.	Print the sum of odd digits.
```
## PROGRAM:
```
#include <stdio.h>

int main() {
    int num, sum = 0;
    printf("Enter a number: ");
    scanf("%d", &num);

    for(int count = 1; count <= num; count++) {
        if(count % 2 != 0) {
            sum += count;
        }
    }

    printf("Sum of odd numbers from 1 to %d is: %d\n", num, sum);
    return 0;
}

```

## OUTPUT:

![Screenshot 2025-04-29 194847](https://github.com/user-attachments/assets/8a55bf91-e5fd-4026-8289-523da4731644)

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
```
# include <stdio.h>

long long fact(int n) {
    int i;
    long long fact=1;
    for(i=1;i<=n;i++){
        fact=fact*i;
    }
    return fact;
}

int main() {
    int n;
    scanf("%d",&n);
    if(n<0) {
        printf("Factorial value is not defined negative number.");
    }
    else {
        printf("Factorial value is: %lld\n",fact(n));
    }
    return 0;
}
```

## OUTPUT:

![Screenshot 2025-04-29 195146](https://github.com/user-attachments/assets/00af85d8-485c-462a-85f0-86d3978e9aa7)

## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
