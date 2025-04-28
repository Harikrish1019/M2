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
```

#include <stdio.h>
#include<math.h>
void emi(float p,float r,float n)
{
    r=r/(100*12);
    n=n*12;
    float emi=p*r*pow(1+r,n)/(pow(1+r,n)-1);
    printf("Monthly EMI is= %.3f",emi);
}
int main()
{
    float p,n,r;
    scanf("%f %f %f",&p,&r,&n);
    emi(p,r,n);
}


```
## OUTPUT:



![437940957-d15b6f9d-3da0-41ff-a814-e3ad3063745f](https://github.com/user-attachments/assets/5d9857ce-df66-4d3a-8ded-f44fc5399f92)







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
```

#include<stdio.h>
void fibonacci(int n)
{
    int temp=-1,a=1,b=0;
    for (int i=1;i<=n;i++)
    {
        temp=a+b;
        a=b;
        b=temp;
        printf("%d ",a);
       
    }
}
int main()
{
    int num;
    scanf("%d",&num);
    fibonacci(num);
}


```

## OUTPUT:
![437941008-cdc27f77-0a25-4bf3-8a0e-7ef322435607](https://github.com/user-attachments/assets/2c4b7cf5-5436-441f-9780-9a3d4b140506)





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
```

#include<stdio.h>
int main()
{
    int n,i;
    scanf("%d",&n);
    int arr[n];
    for (i=0;i<n;i++)
    {
        scanf("%d",&arr[i]);
    }
    if (n>0) printf("%d\n",arr[n-1]);
    else printf(" ");   
}

```

## OUTPUT:


![437941082-34851039-ad90-4502-b85c-dc0c5777a8a6](https://github.com/user-attachments/assets/b54af868-fec0-49da-890f-75551e49167e)




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

```

#include<stdio.h>
int main()
{
    int n,i;
    scanf("%d",&n);
    int arr[n],count_pos=0,count_neg=0;
    for (i=0;i<n;i++)
    {
        scanf("%d",&arr[i]);
        if (arr[i]>0) count_pos++;
        else count_neg++;
    }
    printf("count  of positive numbers  in array: %d\n",count_pos);
    printf("count  of negative numbers  in array: %d",count_neg);
}


```
## OUTPUT:
![437941144-cfca22c6-72b5-45c1-bfa6-52d15c754121](https://github.com/user-attachments/assets/a7fee542-01c4-4c00-88ed-e37edcc410ab)




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
#include <stdio.h>

int main() {
    int n;
    scanf("%d", &n);

    int arr[n];
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    for (int i = 0; i < n; i++) {
        if (arr[i] % 2 == 0) {
            arr[i] = 'E';  // Replacing even numbers with 'E'
        }
    }

    for (int i = 0; i < n; i++) {
        if (arr[i] == 'E') {
            printf("E ");
        } else {
            printf("%d ", arr[i]);
        }
    }

    return 0;
}

```

## OUTPUT:

![437946698-8069572d-0579-4e34-acf8-50030e3aea5f](https://github.com/user-attachments/assets/e8b0d0f5-7b86-49b9-828b-1cdd97d50028)


## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
