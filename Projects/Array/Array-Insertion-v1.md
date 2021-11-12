## Array Insertion Operation.

### 1- Program
Agenda:
- Get the value from user.
- Print the given values.


``` 
#include<stdio.h>

void main(){
    int size, arr[50], i;

    printf("Enter the size of array = ");
    scanf("%d", &size);

    for(i=0; i<=size-1; i++){
        printf("Enter the value for %d position \n", i+1);
        scanf("%d",&arr[i]);
    }

    for(i=0; i<=size-1; i++){
        printf("%d value at %d position \n", arr[i], i+1);
    }
}

//Coded by github.com/Dushyantsingh-ds
```
<details>
<summary>Expend Result</summary>


Result:
  
```
Enter the size of array = 5
Enter the value for 1 position 
24
Enter the value for 2 position 
4
Enter the value for 3 position 
19
Enter the value for 4 position 
7
Enter the value for 5 position 
26
24 value at 1 position 
4 value at 2 position 
19 value at 3 position 
7 value at 4 position 
26 value at 5 position 
```
  
</details>

<hr/>

### 2- Program

Objective: 
- Insert the value at certain index with swapping.

Agenda:
- Get the value from user.
- Print the given values.
- Get the Index to store the Value
- Get the Value to store in the given Index

``` 
#include<stdio.h>

void main(){
    int size, arr[50], i, index;

    printf("Enter the size of array = ");
    scanf("%d", &size);
    for(i=0; i<=size-1; i++){
        printf("Enter the value for %d position \n", i+1);
        scanf("%d",&arr[i]);
    }
    for(i=0; i<=size-1; i++){
        printf("%d value at %d position \n", arr[i], i+1);
    }
    
    printf("Enter the index to store the value = ");
    scanf("%d", &index);
    for(int i=size-1; i>=index-1;i--){
        arr[i+1]=arr[i];
    }
    printf("Enter the value your index = ");
    scanf("%d", &arr[index-1]);
    size++;
     for(i=0; i<=size-1; i++){
        printf("%d value at %d position \n", arr[i], i+1);
    }

}

//Coded by github.com/Dushyantsingh-ds
```
<details>
<summary>Expend Result</summary>


Result:
  
```
Enter the size of array = 5
Enter the value for 1 position 
24
Enter the value for 2 position 
4
Enter the value for 3 position 
19
Enter the value for 4 position 
7
Enter the value for 5 position 
26
24 value at 1 position 
4 value at 2 position 
19 value at 3 position 
7 value at 4 position 
26 value at 5 position 
Enter the index to store the value = 4
Enter the value your index = 2
24 value at 1 position 
4 value at 2 position 
19 value at 3 position 
2 value at 4 position 
7 value at 5 position 
26 value at 6 position 
```
  
</details>



