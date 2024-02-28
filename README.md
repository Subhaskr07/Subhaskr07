#include <stdio.h>
int main()
{
    int n=7;
    for (int i = 1; i <= n; i++)
    {

        for (int j = 1; j <= n; j++)
        {
            if ((j == 1 || j == n) && i != n)
                printf("* ");
            else if (i == n && j != 1 && j != n)
                printf("* ");
            else
                printf("  ");
        }

        for (int s = 1; s <= 3; s++)
        {
            printf(" ");
        }

        for (int j = 1; j <= n; j++)
        {
            if (i == 1 || i == n || j == n / 2 + 1)
                printf("* ");
            else
                printf("  ");
        }

        for (int s = 1; s <= 3; s++)
        {
            printf(" ");
        }

        for (int j = 1; j <= n; j++)
        {
            if (i == 1 || j == n / 2 + 1)
                printf("* ");
            else
                printf("  ");
        }

        for (int s = 1; s <= 1; s++)
        {
            printf(" ");
        }
        if(i==n)
         printf("*");
         else
         printf(" ");
         for (int s = 1; s <= 3; s++)
        {
            printf(" ");
        }

        for (int j = 1; j <= n; j++)
        {
            if (j == 1 || ((i == 1 || i == n || i == n / 2 + 1) && j <= n - 1))
                printf("* ");
            else if ((i != 1 && i != n) && (j == n))
                printf("* ");
            else
                printf("  ");
        }

        for (int s = 1; s <= 3; s++)
        {
            printf(" ");
        }

        for (int j = 1; j <= n; j++)
        {
            if ((j == 1 || j == n) && i != n)
                printf("* ");
            else if (i == n && j != 1 && j != n)
                printf("* ");
            else
                printf("  ");
        }
        printf("\n");
    }

    return 0;
}
