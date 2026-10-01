Program
```
#include <stdio.h>
#include <ctype.h>

int main()
{
    char a[20];
    int flag = 1;
    int i = 1;

    printf("Enter an identifier: ");
    fgets(a, sizeof(a), stdin);

    /* Check the first character */
    if (isalpha((unsigned char)a[0]))
    {
        while (a[i] != '\0' && a[i] != '\n')
        {
            if (!isdigit((unsigned char)a[i]) &&
                !isalpha((unsigned char)a[i]))
            {
                flag = 0;
                break;
            }

            i++;
        }
    }
    else
    {
        flag = 0;
    }

    if (flag == 1)
    {
        printf("Valid identifier\n");
    }
    else
    {
        printf("Not a valid identifier\n");
    }

    return 0;
}
```
Output
<img width="347" height="177" alt="image" src="https://github.com/user-attachments/assets/940fe9a1-04bc-48a7-8a36-87a78efa3b4d" />
