Program
```
#include <stdio.h>

int main()
{
    char str[500];
    int whitespaces = 0;
    int newlines = 0;
    int characters = 0;

    printf("Enter text (use ~ to end):\n");
    scanf("%[^~]", str);

    for (int i = 0; str[i] != '\0'; i++)
    {
        if (str[i] == ' ' || str[i] == '\t')
        {
            whitespaces++;
        }
        else if (str[i] == '\n')
        {
            newlines++;
        }
        else
        {
            characters++;
        }
    }

    printf("\nTotal number of whitespaces: %d\n", whitespaces);
    printf("Total number of newline characters: %d\n", newlines);
    printf("Total number of characters: %d\n", characters);

    return 0;
}
```
Output
<img width="385" height="372" alt="image" src="https://github.com/user-attachments/assets/32cdb07f-2b29-4f5a-99ac-410812029c5e" />
