
# EX-01-Datatypes-Operators
## AIM:
Write a C program to read 3 characters one by one and print the characters in a reverse order.

## ALGORITHM:
1.	Declare three character variables to store the input characters.
2.	Use the scanf function to read the characters one by one from the user.
3.	Print the characters in reverse order using the printf function.
4.	End the program.

## PROGRAM:
~~~
#include <stdio.h>
int main ()
{
    int a;
    scanf("%d",&a);
    printf("Character of ASCII Value %d is %c",a,a);
    return 0;
}
~~~
## OUTPUT:

![image](https://github.com/user-attachments/assets/ac68c514-fa9d-4429-9d44-7697cf1d7882)
















## RESULT:
Thus the program to read 3 characters one by one and print the characters in a reverse order has been executed successfully.


# EX-02- Conditional-Statements
## AIM:
Write a C program to read A values and check whether A is positive number or not.

# ALGORITHM:
1.	Declare a variable to store the input value A.
2.	Use the scanf function to read the value of A from the user.
3.	Check if the value of A is greater than zero.
4.	If A is greater than zero, print a message indicating that it's a positive number. 
5.	Otherwise, print a message indicating that it's not a positive number.
6.End the program.

# PROGRAM:
~~~
#include<stdio.h>
int main()
{
    int a;
    scanf("%d",&a);
    if (a>=10)
    {
        printf("Number is positive.");
    }
    else if (a<0)
    {
        printf("Number is negative.");
    }
    else
    {
        printf("Number is positive.");
    }
}
~~~
# OUTPUT:



![image](https://github.com/user-attachments/assets/08ccb9af-f8f6-4b39-8121-f722c788441d)








# RESULT:
Thus the program to read A values and check whether A is positive number or not has been executed successfully.
 
 
 


# EX-03- Operators-Expressions
## AIM:
Write a program to find minimum between two fraction numbers using conditional operator or ternary operator.

## ALGORITHM:
1.	Declare variables to store the two fraction numbers and the result.
2.	Use the printf function to prompt the user to enter the first fraction number (numerator and denominator separately).
3.	Use the scanf function to read the numerator and denominator of the first fraction.
4.	Repeat steps 2 and 3 to get the second fraction from the user.
5.	Calculate the decimal values of both fractions by dividing the numerators by the denominators.
6.	Use the conditional (ternary) operator to compare the decimal values and store the minimum value in the result variable.
7.	Print the minimum value.

## PROGRAM:
~~~
#include <stdio.h>

int main() {
    char input;
    scanf("%c", &input);
    ((input >= 'a' && input <= 'z') || (input >= 'A' && input <= 'Z')) 
        ? printf("It is an ALPHABET\n") 
        : printf("It is NOT AN ALPHABET\n");

    return 0;
}
~~~
## OUTPUT:

![image](https://github.com/user-attachments/assets/6a08a669-b2fb-4086-a002-e58d980e1a01)








## RESULT:
Thus the program to find minimum between two fraction numbers using conditional operator or ternary operator has been executed successfully.




# EX-04- Using Conditional Statements

## AIM:
Write a C program to check whether the input value is equal to 1 using simple if statement

## ALGORITHM:
1.	Declare a variable to store the input value.
2.	Use the scanf function to read the input value from the user.
3.	Use an if statement to check if the input value is equal to 1.
4.	If the condition in the if statement is true, print a message indicating that the input value is equal to 1.
5.	Otherwise, print a message indicating that it's not equal to 1.
6.	End the program.

## PROGRAM:
~~~
#include <stdio.h>

int main() {
    int number;
    scanf("%d", &number);
    if (number % 5 == 0) {
        printf("The number is multiples of 5\n");
        if (number % 10 == 0) {
            printf("The number is also divisible by 10\n");
        } else {
            printf("The number Not divisible by 10\n");
        }
    } else {
        printf("The number is NOT an multiples of 5\n");
    }

    return 0;
}
~~~
## OUTPUT:



![image](https://github.com/user-attachments/assets/9b54ea7d-4e7f-490f-b5b2-f621b9e33bf8)






	

## RESULT:
Thus the program to check whether the input value is equal to 1 using simple if statement has been executed successfully



# EX-05- Calculating Total, Percentage, And Division Using Conditional Statements 
## AIM:
To write a C program that reads marks of three subjects, calculates the total and percentage, and then determines the division (First, Second, Pass, or Fail) based on the percentage and minimum marks criteria.
## ALGORITHM:
1.	Start
2.	Declare integer variables m1, m2, m3 for marks, and float variables tot, per.
3.	Input the marks for three subjects.
4.	Calculate total marks: tot = m1 + m2 + m3
5.	Calculate percentage: per = tot / 3
6.	Display total and percentage.
7.	Check if all marks are greater than or equal to 40:
8.	If yes:
a.	If percentage >= 60: Print “Division = First”
b.	Else if percentage >= 48: Print “Division = Second”
c.	Else if percentage >= 36: Print “Division = Pass”
9.	Else: Print “Division = Fail”
10.	End
## PROGRAM:
~~~
#include <stdio.h>
#include <string.h>

int main()
{
    int phy,che,ca,total;
    float per;
    char div[10];

   
    scanf("%d%d%d",&phy,&che,&ca);
    total = phy+che+ca;
    per = total/3.0;
    if (per>=60)
	 strcpy(div,"First");
    else if (per<60 && per>=48)
	    strcpy(div,"Second");
	else
	    if (per<48 && per>=36)
		strcpy(div,"Pass");
	    else
		strcpy(div,"Fail");

      
       printf("Total Marks = %d\nPercentage = %5.2f\nDivision = %s\n",total,per,div);
       return 0;
}


~~~
## OUTPUT:
![image](https://github.com/user-attachments/assets/89646a7f-b45a-4e52-81c7-d7031a977e8e)

## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.

