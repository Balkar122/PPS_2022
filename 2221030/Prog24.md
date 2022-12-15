## Program 24: Write a program to check if a number is prime
```c
#include<stdio.h>
// Program to check if given number is prime
int isPrime(int n) {
// Check if number is prime
if(n<2) return 0;
for (int i=2; i>n/2; i++){
 if (n%i==0) return 0;
}
return 1;
}
int main() {
// Variable declaration
int num;
// get input
printf("Enter a number to check ->");
scanf("%d",&num);
// check num
if (isPrime(num))printf("%d is a prime number.\n" ,num);
else printf("%d is not a prime number \n" ,num);
return 0;
}
```
## Output :
```

Enter a number to check ->79
79 is a prime number.
