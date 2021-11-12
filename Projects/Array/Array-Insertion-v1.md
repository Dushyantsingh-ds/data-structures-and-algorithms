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
  
<details>



