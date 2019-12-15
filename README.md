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
 ```
Output:


 ## Ques2.
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
```
## Ques3.
```c 
#include<stdio.h>
int main()
{
int n,i,j;
printf("Enter desired number");
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
```

## Ques4.
```c 
nclude<stdio.h>
int main()
{
int n,i,j;
printf("Enter desired number");
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
```
## Ques5.
```c 
#include<stdio.h>
int main()
{ 
printf("Enter Number");
int n;
scanf("%d",&n);
int i;
for(i=1;i<=10;i++)
{
printf("%d x %d = %d\n",n,i,n*i);
}
}
```
## Ques6
```c 
#include <stdio.h>
int main()
{
printf("Enter 1st Number");
int n1;
scanf("%d",&n1);
printf("Enter 2nd Number");
int n2;
scanf("%d",&n2);
int j,i,a,d;
for(j=n1;j<=n2;j++)
{
for(i=1;i<=j;i++)
{
{                                                        
 d=j%i;
if(d==0)
a++;
}                                                        
if(a==2)
printf("Number is prime");
else
printf("Number is  composite");                          
}
}

                                                         
```
## Ques7
```c 
#include<stdio.h>
int main()
{ 
printf("Enter 1st Number");
int n1;
scanf("%d",&n1);
printf("Enter 2nd Number");
int n2;
scanf("%d",&n2);
int i,j;
for(j=n1;j<=n2;j++)
{
for(i=1;i<=10;i++)
{
printf("%d x %d = %d\n",j,i,j*i);
}
}
}




                                 
```
## Ques8
```c 
#include<stdio.h>
int main()
{
int n,i,j;
printf("Enter desired number");
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
```
## Ques9


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
```
## Ques10.
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

## Ques11.
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
```
## Ques12
```c 
#include<stdio.h>
int main()
{
printf("Enter Number");
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
```
## Ques13.
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

```

## Question 14.
```c 

#include <stdio.h>
    void main()
    {
 
         int ARR[10], EAR[10];
        int i, j = 0, k = 0, n;
 
        printf("Enter the size of array AR n");
        scanf("%d", &n);
 
        printf("Enter the elements of the array n");
        for (i = 0; i < n; i++)
        {
            scanf("%ld", &ARR[i]);
            fflush(stdin);
        }
 
 
        for (i = 0; i < n; i++)
        {
            if (ARR[i] % 2 == 0)
            {
                EAR[j] = ARR[i];
                j++;
            }

 
        printf("The elements of EAR are n");
        for (i = 0; i < j; i++)
        {
            printf("%ldn", EAR[i]);
        }
 
    }
    ```

