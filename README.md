#include<stdio.h>
int main()
{
    int n, key, flag = 0;
    printf("Enter the size of array: ");
    scanf("%d", &n);

    printf("Enter the key: ");
    scanf("%d", &key);

    int arr[n];

    for(int i = 0; i < n; i++)
    {
        scanf("%d", &arr[i]);

        if(arr[i] == key)
        {
            flag = 1;
            break;
        }
    }

    if(flag == 0)
        printf("Key is not found\n");
    else
        printf("Key is found\n");

    return 0;
}
OUTPUT
Enter the size of array: 4
Enter the key: 10
20 
30
50
10
Key is found
