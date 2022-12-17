## Program 30: Write a program to show two variable using a temporary variable
```c
#include <stdio.h>

int main(){
    int n1,n2;
    printf("Enter first number -> ");
    scanf("%d",&n1);
    printf("Enter second number -> ");
    scanf("%d",&n2);

    int temp = n1;
    n1 = n2;
    n2 = temp;

    printf("\nAfter swapping:\n");
    printf("First number -> %d\n",n1);
    printf("Second number -> %d\n",n2);

    return 0;
}
```
## Output :
```
Enter first number -> 80
Enter second number -> 50
After swapping:
First number -> 50
Second number -> 80
