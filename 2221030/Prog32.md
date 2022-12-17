## Program 32: Write a program to perform binary search
```c
#include <stdio.h>
int main(){
    int len,target;
    int left,right,mid;
    printf("Enter size of array\n");
    scanf("%d",&len);
    int arr[len];
    printf("Enter elements [must be in ascending order]\n");
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
    left=0;
    int i = 0;
    right=len-1;
    while(left!=right){
        mid = (left+right)/2;
        if(arr[mid]==target)break;
        else if(arr[mid]>target){
            right=mid-1;
        } else {
            left=mid+1;
        }
        i++;
        if(i>10)break;
    }
    printf("\nLocation of %d in array = %d\n",target,mid);
}
```
## Output :
```

Enter size of array
6
Enter elements [must be in ascending order]
Enter element at index 0 -> 85
Enter element at index 1 -> 95
Enter element at index 2 -> 102
Enter element at index 3 -> 134
Enter element at index 4 -> 225
Enter element at index 5 -> 256
Enter element to search -> 285
Entered array is :
85	95	102	134	225	256	

Location of 285 in array = 4
