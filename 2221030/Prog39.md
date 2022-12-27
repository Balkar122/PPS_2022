## Program 39: Write a program to compare two string using strcpy()
```c
#include <stdio.h>
#include <string.h>

int main() {
    char str1[50],str2[50];
    printf("Enter a string -> ");
    scanf("%s",str1);
    printf("Enter another string -> ");
    scanf("%s",str2);

    int x = strcmp(str1,str2);
    if(x>0)printf("First string is greater/longer\n");
    else if(x<0)printf("First string is smaller/lesser\n");
    else printf("Both strings are equal\n");

    return 0;
}
```
## Output :
```
Enter a string -> cat

Enter another string -> kitten

First string is smaller/lesser
