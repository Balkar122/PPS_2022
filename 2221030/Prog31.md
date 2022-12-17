## Program 31: Write a program to perform linear search
```c
#include <stdio.h>

int main(){
    int len,target,ind;
    printf("Enter size of array\n");
    scanf("%d",&len);
    int arr[len];
    printf("Enter elements:\n");
    for(int i=0;i<len;i++){
        printf("Enter element at index %d -> ",i);
        scanf("%d",&arr[i]);
    }
    printf("Enter element to search -> ");
    scanf("%d",&target);
    printf("\nEntered array is :\n");
    for(int i=0;i<len;i++){
        printf("%d\t",arr[i]);
    }
    printf("\n");
    for(int i=0;i<len;i++){
        if(arr[i] == target)ind=i;
    }
    printf("\nLocation of %d in array = %d\n",target,ind);
}
```
## Output :
```

Enter size of array
7
Enter elements:
Enter element at index 0 -> 65
Enter element at index 1 -> 85
Enter element at index 2 -> 92
Enter element at index 3 -> 74
Enter element at index 4 -> 655
Enter element at index 5 -> 876
Enter element at index 6 -> 778
Enter element to search -> 999
Entered array is :
65	85	92	74	655	876	778	

Location of 999 in array = 32764
