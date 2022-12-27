## Program 34: Write a program to perform bubble sort
```c
#include <stdio.h>

void bubbleSort(int *arr,int len){
    int temp;
    for(int i=0;i<len;i++){
        for(int j=0;j<len-1-i;j++){
            if(arr[j+1] < arr[j]){
                //swap
                temp = arr[j];
                arr[j] = arr[j+1];
                arr[j+1] = temp;
            }
        }
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
    bubbleSort(arr, len);

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
7
Enter elements 
Enter element at index 0 -> 77
Enter element at index 1 -> 88
Enter element at index 2 -> 99
Enter element at index 3 -> 0
Enter element at index 4 -> 75
Enter element at index 5 -> 85
Enter element at index 6 -> 95
Unsorted array is :
77	88	99	0	75	85	95	

Sorted array is :
0	75	77	85	88	95	99	
