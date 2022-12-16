## Program 26: Write a program to show the factorial of a given number
```c
#include <stdio.h>
//Program to calculate factorial of a number
long int fact(int n){
    if(n<=1)return 1;
    else return fact(n-1)*n;
}
int main(){
    int n;
    printf("Enter a number: ");
    scanf("%d",&n);

    printf("Factorial of %d = %ld\n",n,fact(n));
return 0;
}
```
## Output :
```
Enter a number: 10
Factorial of 10 = 3628800
