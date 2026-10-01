Program
```
#include <stdio.h>
#include <string.h>

int main()
{
    char s[5];

    printf("Enter any operator: ");
    fgets(s, sizeof(s), stdin);

    switch (s[0])
    {
        case '>':
            if (s[1] == '=')
                printf("Greater than or equal\n");
            else
                printf("Greater than\n");
            break;

        case '<':
            if (s[1] == '=')
                printf("Less than or equal\n");
            else
                printf("Less than\n");
            break;

        case '=':
            if (s[1] == '=')
                printf("Equal to\n");
            else
                printf("Assignment\n");
            break;

        case '!':
            if (s[1] == '=')
                printf("Not Equal\n");
            else
                printf("Bit Not\n");
            break;

        case '&':
            if (s[1] == '&')
                printf("Logical AND\n");
            else
                printf("Bitwise AND\n");
            break;

        case '|':
            if (s[1] == '|')
                printf("Logical OR\n");
            else
                printf("Bitwise OR\n");
            break;

        case '+':
            printf("Addition\n");
            break;

        case '-':
            printf("Subtraction\n");
            break;

        case '*':
            printf("Multiplication\n");
            break;

        case '/':
            printf("Division\n");
            break;

        case '%':
            printf("Modulus\n");
            break;

        default:
            printf("Not an operator\n");
    }

    return 0;
}
```
Output:
<img width="273" height="172" alt="image" src="https://github.com/user-attachments/assets/ba5b013b-3488-4c7a-bd4d-4f6bd094883d" />
