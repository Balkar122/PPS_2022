## Program 15: Write a program to use conditional operator
```c
#include<stdio.h>
int main ()
{
int x;
printf("Enter a number : ");
scanf("%d", &x);
(x%2==0)?printf("Number is even\n"):printf("Number is odd\n");
return 0;
}
```
## Output :
```
Enter a number : 11
Number is odd
