## Program 11: Write a program to use jump statements(break and continue)
```c
#include<stdio.h>
int main ()
{
for (int i=1;i<=60;i++)
{
if(i==20)break;
if(i%2==0)continue;
printf("%d\n",i);
}
return 0;
} 
```
## Output:
```
1
3
5
7
9
11
13
15
17
19
