## Program 33: Write a program to perform selection sort
```c
#include <stdio.h>

void selSort(int *arr,int len){
    int min = 0,temp;
    for(int i=0;i<len;i++){
        min = i;
        //find min
        for(int j=i;j<len;j++){
            if(arr[j]<arr[min])min=j;
        }
        //swap
        temp = arr[i];
        arr[i] = arr[min];
        arr[min] = temp;
    }
}

int main(){
    int len;
    printf("Enter size of array\n");
    scanf("%d",&len);
    int arr[len];
    printf("Enter elements \n");
    for(int i=0;i<len;i++){
        printf("Enter element at index %d -> ",i);
        scanf("%d",&arr[i]);
    }
    printf("\nUnsorted array is :\n");
    for(int i=0;i<len;i++){
        printf("%d\t",arr[i]);
    }
    printf("\n");
    selSort(arr, len);

    printf("\nSorted array is :\n");
    for(int i=0;i<len;i++){
        printf("%d\t",arr[i]);
    }
    printf("\n");
}
```
## Output :
```
Enter size of array
10
Enter elements 
Enter element at index 0 -> 55
Enter element at index 1 -> 65
Enter element at index 2 -> 64
Enter element at index 3 -> 77
Enter element at index 4 -> 98
Enter element at index 5 -> 76
Enter element at index 6 -> 66
Enter element at index 7 -> 888
Enter element at index 8 -> 987
Enter element at index 9 -> 877
Unsorted array is :
55	65	64	77	98	76	66	888	987	877	

Sorted array is :
55	64	65	66	76	77	98	877	888	987	
