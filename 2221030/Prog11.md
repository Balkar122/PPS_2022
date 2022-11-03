## Program 11: Write a program to show ascii character of a given code
```
#include<stdio.h>
int main()
{
int x;
printf("Enter a ascii value: ");
scanf("%d", &x);
printf("character for ascii value %d: %c\n ",x,(char)x);
return 0;
}
```
## Output :
```
Enter a ascii value: 97
character for ascii value 97: a
 
