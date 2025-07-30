# second-largest-number
#include <stdio.h>
// Find the second largest number from arrays.
int main()
{
    int arr[10];
    int l = 0;
    int s_l = 0;
    for (int i = 0; i < 10; i++)
    {
        printf("Enter the elements ");
        scanf("%d", &arr[i]);
    }
    for (int i = 0; i < 10; i++)
    {
        if (arr[i] > l)
        {
            l = arr[i];
        }
    }
    for (int i = 0; i < 10; i++)
    {
        if (arr[i] > s_l && arr[i] != l)
        {
            s_l = arr[i];
        }
    }
    printf("The value is %d ", l);
    printf("The value is %d ", s_l);
    return 0;
}
