# PPS-Assingnment>
## Ques.1  To change temperature from degree fahrenheit
```c 
#include<stdio.h> 
int main()
{
printf("Enter temp in fahrenheit:");
float f,c=0;
scanf("%f",&f);
c=(5.0/9)*(f-32.0);
printf("Temp in centigrade:%f\n",c);
}

Output: 
Enter temp in farenheit: 45
Temp in centigrade:7.222222
 ```


 ## Ques2. To find whether number is odd or even
 ```c
 #include<stdio.h>
int main()
{
int i;
printf("Enter the Number:");
scanf("%d",&i);
if (i%2==0)
printf("Number is Even\n");
else
printf("Number is Odd\n");
} 
Output:
Enter the number:7
Number is Odd

```
## Ques3.To display the pattern
```c 
#include<stdio.h>
int main()
{
int n,i,j;
printf("Enter desired number:\n");
scanf("%d",&n);
for (i=1;i<=n;i++)
{
for(j=1;j<=i;j++)
{
printf("*");
}
printf("\n");
}
}

Output:
Enter desired number:6
*
**
***
****
*****
```

## Ques4.To find greates among three numbers
```c 
#include <stdio.h>
    int main()
       {
           int num1,num2,num3,largest;
           printf("Enter first number\n");
           scanf("%d",&num1);
            printf("Enter second number\n");
           scanf("%d",&num2);
            printf("Enter three number\n");
           scanf("%d",&num3);
           if(num1>num2)
           {
               if(num1>num3)
               largest=num1;
               else
               largest=num3;
           }
           else
           {
               if(num2>num3)
               largest=num2;
               else
               largest=num3;
           }
           printf("Largest number is %d",largest);
       }
Output:
Enter first number
8
Enter second number
6
Enter three number
9
Largest number is 9


```
## Ques5.To display table of any number
```c 
#include<stdio.h>
int main()
{ 
printf("Enter Number:");
int n;
scanf("%d",&n);
int i;
for(i=1;i<=10;i++)
{
printf("%d x %d = %d\n",n,i,n*i);
}
}
Output:
Enter Number:6
6 x 1 = 6
6 x 2 = 12
6 x 3 = 18
6 x 4 = 24
6 x 5 = 30
6 x 6 = 36
6 x 7 = 42
6 x 8 = 48
6 x 9 = 54
6 x 10 = 60

```
## Ques6: To check whether number is prime or composite between the given range
```c 
#include <stdio.h>
int main()
{
printf("Enter 1st Number:\n");
int n1;
scanf("%d",&n1);
printf("Enter 2nd Number:\n");
int n2;
scanf("%d",&n2);
int j,i,a,d;
for(j=n1;j<=n2;j++)
{
for(i=1;i<=j;i++)
{                                    
 d=j%i;
if(d==0)
a++;
}

if(a==2)
printf("%d is prime\n",j);
else
printf("%d is  composite\n",j); 
a=0;
}
}
Output:
Enter 1st Number:
3
Enter 2nd Number:
9
3 is prime
4 is  composite
5 is prime
6 is  composite
7 is prime
8 is  composite
9 is  composite

                                                         
```
## Ques7: To display table between a given range
```c 
#include<stdio.h>
int main()
{ 
printf("Enter 1st Number:");
int n1;
scanf("%d",&n1);
printf("Enter 2nd Number:");
int n2;
scanf("%d",&n2);
int i,j;
for(j=n1;j<=n2;j++)
{
for(i=1;i<=10;i++)
{
printf("%d x %d = %d\n",j,i,j*i);
}
printf("\n");
}
}

Output:
Enter 1st Number:3
Enter 2nd Number:5
3 x 1 = 3
3 x 2 = 6
3 x 3 = 9
3 x 4 = 12
3 x 5 = 15
3 x 6 = 18
3 x 7 = 21
3 x 8 = 24
3 x 9 = 27
3 x 10 = 30

4 x 1 = 4
4 x 2 = 8
4 x 3 = 12
4 x 4 = 16
4 x 5 = 20
4 x 6 = 24
4 x 7 = 28
4 x 8 = 32
4 x 9 = 36
4 x 10 = 40

5 x 1 = 5
5 x 2 = 10
5 x 3 = 15
5 x 4 = 20
5 x 5 = 25
5 x 6 = 30
5 x 7 = 35
5 x 8 = 40
5 x 9 = 45
5 x 10 = 50






                                 
```
## Ques8
```c 

```
## Ques9:To print the following pattern(2)


```c 
#include<stdio.h>
int main()
{
int n,i,j;
printf("Enter desired number");
scanf("%d",&n);
for (i=1;i<=n;i++)
{
for(j=n;j>=i;j--)
{
printf("*");
}
printf("\n");
}
}
Output:
Enter desired number4
****
***
**
*



```
## Ques10. To find Factorial of a number
```c
#include <stdio.h>
long int multiplyNumbers(int n);
int main()
{
    int n;
    printf("Enter a positive integer: ");
    scanf("%d", &n);
    printf("Factorial of %d = %ld", n, multiplyNumbers(n));
    return 0;
}
long int multiplyNumbers(int n)
{
    if (n >= 1)
        return n*multiplyNumbers(n-1);
    else
        return 1;
}
Output:
Enter a positive integer: 5
Factorial of 5 = 120

```

## Ques11. To do arithmatic operation using swtch statement
```c 
#include<stdio.h>
int main()
{
char o;
printf("Select an operator:");
scanf("%c",&o);
int a,b;
printf("Enter first number:");
scanf("%d",&a);
printf("Enter second nember:");
scanf("%d",&b);
switch(o)
{
case '+':
printf("Sum is %d",a+b);
break;

case '-':
printf("Difference is %d",a-b);
break;

case '*':
printf("Product is %d",a*b);
break;

case '/':
printf("Quotient is %d",a/b);                            
break;

case '%':
printf("Remainder is %d",a%b);                           
break;

default:
printf("Invalid Entry");
}
}
Output:
Select an operator:*
Enter first number:5
Enter second nember:9
Product is 45


```
## Ques12: To print table of even number
```c 
#include<stdio.h>
int main()
{
printf("Enter Number:");
int n;
scanf("%d",&n);
if(n%2==0)
{
int i;
for(i=1;i<=10;i++)
{
printf("%d x %d = %d\n",n,i,n*i);
}
}
else
{
printf("number is odd\n");
}
}
Output:
Enter Number:4
4 x 1 = 4
4 x 2 = 8
4 x 3 = 12
4 x 4 = 16
4 x 5 = 20
4 x 6 = 24
4 x 7 = 28
4 x 8 = 32
4 x 9 = 36
4 x 10 = 40

     OR
Enter Number7
number is odd


    
```
## Ques13.To print Reverse of number
```c 
#include <stdio.h>
int main()
{
    int n, reversedNumber = 0, remainder;
    printf("Enter an integer: ");
    scanf("%d", &n);
    while(n != 0)
    {
        remainder = n%10;
        reversedNumber = reversedNumber*10 + remainder;
        n /= 10;
    }
    printf("Reversed Number = %d", reversedNumber);
    return 0;
}
Output:
Enter an integer: 548
Reversed Number = 845



```

## Question 14. To find factorial of a number by recursion
```c 
#include<stdio.h>
long int multiplyNumbers(int n);
int main() {
    int n;
    printf("Enter a positive integer: ");
    scanf("%d",&n);
    printf("Factorial of %d = %ld", n, multiplyNumbers(n));
    return 0;
}
long int multiplyNumbers(int n) {
    if (n>=1)
        return n*multiplyNumbers(n-1);
    else
        return 1;
}
Output:
Enter a positive integer: 6
Factorial of 6 = 720


    ```
