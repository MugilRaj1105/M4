# EX-16-LEFT-SHIFT-OPERATION
## AIM
To write a C Program to perform the basic left shift operation for 44 integer number with 3 shifts.

## ALGORITHM
```
1.Start the program.
2.Assign values of a and b as 44 and 3.
3.Use left shift operator (<<) and shift the value of a three times.
4.Display the result.
5.Stop the program.
```
## PROGRAM
```
#include<stdio.h>
int main(){
    int a=44;
    a=a<<3;
    printf("After Left Shift Operation value of a is:%d",a);
}
```
## OUTPUT

![WhatsApp Image 2025-04-27 at 15 24 04_37c40b2d](https://github.com/user-attachments/assets/f0698316-3bd1-4b5e-b7c0-06769988aea0)

## RESULT
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.


# EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT


## AIM

Write a C Program to check whether the two numbers are equal or not using simple if statement.

## ALGORITHM
```
1.Start the program.
2.Read two numbers.
3.If first number is equal to second number, display both are equal.
4.Otherwise display both are not equal.
5.Stop the program.
```
## PROGRAM
```
#include<stdio.h>
int main()
{
    int X,Y;
    scanf("%d%d",&X,&Y);
    if(X==Y)
    {
        printf("X is equal to Y");
    }
    else
    {
        printf("X is NOT equal to Y");
    }
    return 0;
}
```

## OUTPUT

![Screenshot 2025-04-27 151357](https://github.com/user-attachments/assets/6d8f7a05-b84b-4964-bb3d-80d09438cb86)

## RESULT

Thus the program to check whether the two numbers are equal or not using simple if statement has been executed successfully
 
 


# EX-18-STRING-LOWERCASE-CONVERSION
## AIM
Write a C Program to convert the given string into lowercase.

## ALGORITHM
```
1.Start the program.
2.Read a string variable.
3.Using tolower( ) function convert the given string into its lowercase.
4.Display the result.
5.Stop the program.
```
## PROGRAM
```
#include<stdio.h>
#include<ctype.h>
int main()
{
    char str[100];
    scanf("%s",str);
    for(int i=0;str[i] != '\0';i++)
    {
        str[i] = tolower(str[i]);
    }
    printf("Lower case String is:%s",str);
    return 0;
}

```

## OUTPUT
![Screenshot 2025-04-27 151457](https://github.com/user-attachments/assets/56e529b3-b03c-495a-bf4a-4ee5b170ec75)



## RESULT
Thus the program to convert the given string into lowercase has been executed successfully
 
 

# EX-19-COUNT-OF-WORDS-IN-A-STRING
## AIM
Write a C Program to count the total number of words in a given string using do While loop.

## ALGORITHM
```
1.Start the program.
2.Read a string variable.
3.Using for loop, inspect the string character by character.
4.Whenever a space is encountered increment count by 1.
5.Display the result.
6.Stop the program.
```
## PROGRAM
```
#include <stdio.h>

int main() {
    char str[1000];
    int i = 0, wordCount = 0;

    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);

    do {
        if ((str[i] != ' ' && str[i] != '\n' && str[i] != '\t') &&
            (str[i + 1] == ' ' || str[i + 1] == '\n' || str[i + 1] == '\t' || str[i + 1] == '\0')) {
            wordCount++;
        }
        i++;
    } while (str[i] != '\0');

    printf("Total number of words: %d\n", wordCount);
    return 0;
}

```


## OUTPUT


![Screenshot 2025-06-02 130606](https://github.com/user-attachments/assets/1530dd29-372a-4732-9ec4-122521228291)



## RESULT
Thus the program to count the total number of words in a given string using do While loop has been executed successfully
 
 

# EX  -20 -COMPARING TWO STRINGS
## AIM
write a Program to compare two strings without using strcmp().

## ALGORITHM
```
Step 1: Start the program.
Step 2: Declare two character arrays c1 and c2 of size 100 to store the strings. Also, declare an integer variable
             flag and initialize it to 0, and i for indexing.      
Step 3: Read the first string c1 using scanf("%[^\n]", c1); — this reads input until a newline is encountered 
            (i.e., can include spaces).
Step 4: Read the second string c2 using scanf("%s", c2); — this reads input until a space or newline (i.e., no 
            spaces in the second string).
Step 5: Start comparing characters of both strings from index i = 0.
Step 6: Repeat the following while neither c1[i] nor c2[i] is '\0' (i.e., end of string):
•	If c1[i] is not equal to c2[i], set flag = 1.
•	Increment i by 1.
Step 7: After the loop, check the value of flag:
•	If flag == 0, print "strings are same".
•	Otherwise, print "strings are not same".
Step 8: End the program.
```
## PROGRAM
```
#include <stdio.h>

int main() {
    char str1[1000], str2[1000];
    int i = 0, flag = 0;

    printf("Enter first string: ");
    fgets(str1, sizeof(str1), stdin);
    printf("Enter second string: ");
    fgets(str2, sizeof(str2), stdin);

    while (str1[i] != '\0' && str2[i] != '\0') {
        if (str1[i] != str2[i]) {
            flag = 1;
            break;
        }
        i++;
    }

    if (flag == 0 && str1[i] == str2[i])
        printf("Strings are equal.\n");
    else
        printf("Strings are not equal.\n");

    return 0;
}

```
## OUTPUT

![Screenshot 2025-06-02 130407](https://github.com/user-attachments/assets/b22ed48e-10f4-428a-baf7-ffcd0ecf2afa)



## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.
