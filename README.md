# EX-16-LEFT-SHIFT-OPERATION
## AIM:
To write a C Program to perform the basic left shift operation for 44 integer number with 3 shifts.

## ALGORITHM:
1.	Start the program.
2.	Assign values of a and b as 44 and 3.
3.	Use left shift operator (<<) and shift the value of a three times.
4.	Display the result.
5.	Stop the program.

## PROGRAM:
```c
#include <stdio.h> 
int main() { 
int a = 44, b = 3; 
int result = a << b; 
printf("result: %d\n", result); 
return 0; 
}
```
## OUTPUT:
![image](https://github.com/user-attachments/assets/0e309ccc-05a0-4641-811e-6b58fea2ab10)



## RESULT:
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.




 
 


# EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT


## AIM:

Write a C Program to check whether the two numbers are equal or not using simple if statement.

## ALGORITHM:

1.	Start the program.
2.	Read two numbers.
3.	If first number is equal to second number, display both are equal.
4.	Otherwise display both are not equal.
5.	Stop the program.

## PROGRAM:
```c
#include <stdio.h>
int main() {
    int num1, num2;
    printf("Enter first number: ");
    scanf("%d", &num1);
    printf("Enter second number: ");
    scanf("%d", &num2);
    if (num1 == num2) {
        printf("The numbers are equal.\n");
    }

    if (num1 != num2) {
        printf("The numbers are not equal.\n");
    }

    return 0;
}
```
## OUTPUT:
<img width="446" alt="image" src="https://github.com/user-attachments/assets/b6373de0-b99a-418b-8b93-489e89642d05" />

## RESULT:

Thus the program to check whether the two numbers are equal or not using simple if statement has been executed successfully
 
 


# EX-18-STRING-LOWERCASE-CONVERSION
## AIM:
Write a C Program to convert the given string into lowercase.

## ALGORITHM:
1.	Start the program.
2.	Read a string variable.
3.	Using tolower( ) function convert the given string into its lowercase.
4.	Display the result.
5.	Stop the program.

## PROGRAM:
```c
#include <stdio.h>
#include <ctype.h>

int main() {
    char str[10];
    int i = 0;
    scanf("%s", str);
    while (str[i] != '\0') {
        str[i] = tolower(str[i]);
        i++;}
printf("%s\n", str);return 0;
}
```
## OUTPUT:
<img width="391" alt="image" src="https://github.com/user-attachments/assets/799a3c20-4085-4fff-a0c4-8b3fba228bc6" />

## RESULT:
Thus the program to convert the given string into lowercase has been executed successfully
 
 


# EX-19-COUNT-OF-WORDS-IN-A-STRING
## AIM:
Write a C Program to count the total number of words in a given string using do While loop.

## ALGORITHM:
1.	Start the program.
2.	Read a string variable.
3.	Using for loop, inspect the string character by character.
4.	Whenever a space is encountered increment count by 1.
5.	Display the result.
6.	Stop the program.

## PROGRAM:
```c
#include <stdio.h>

int main() {
    char str[1000];
    int i=0,w=1;
    scanf("%[^\n]",str);
    do{
        if (str[i]==' '){
            w++;
        } i++;
    }while(str[i]!='\0');
    printf("No of words: %d\n",w);}
```
## OUTPUT:
<img width="444" alt="image" src="https://github.com/user-attachments/assets/a21682d7-3666-4335-ba65-247a131da6ce" />

## RESULT:
Thus the program to count the total number of words in a given string using do While loop has been executed successfully
 
 


# EX  -20 -COMPARING TWO STRINGS
## AIM:
write a Program to compare two strings without using strcmp().
## ALGORITHM:
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

## PROGRAM:
```c
#include <stdio.h>
int main(){
    char c1[100],c2[100];
    int i=0,f=0;
    scanf("%[^\n]",c1);getchar();
    scanf("%[^\n]",c2);
    while(c1[i]!='\0'&& c2[i]!='\0'){
        if(c1[i]!=c2[i]){f=1;}i++;
    }
    if(f==0){printf("same");}
    else {printf("different");}
    
}
```
## OUTPUT:
<img width="296" alt="image" src="https://github.com/user-attachments/assets/3263b9d7-ac03-4796-b51b-0c4303e1e1a2" />

## RESULT:
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

