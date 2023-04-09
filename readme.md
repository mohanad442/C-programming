# Assignment 1
download CodeBlocks IDE From https://sourceforge.net/projects/codeblocks/

## Answer the following questions:
--------------------------------

1- C Program to print "Hello World"

2- C Program to print ASCII number of a char

3- C Program to print a float number entered by the user

4- C Program to add two integers


## Answer "as much as you can" from the following:
------------------------------------------------

5 - C Program to make simple calculations (add, sub, multiply, divid) on two integers

6- C Program to print Hexa of a number

7- C Program to compute Quotient and Remainder

------------------------------------------------
# Assignment 2
## Answer the following questions:
--------------------------------

1- C Program to Check Whether a Number is Even or Odd

2- C Program to Find the Largest Number Among Three Numbers

3- C Program that takes the degree from user, and switch on it to print the corresponding Grade:
A => Excellent
B => Very Good
C => Good
D => fair
E => failed

4- C Program to print total of numbers when it gets to 100. (sum)

5- C Program to display simple menu. (menu)


## Answer "as much as you can" from the following:
------------------------------------------------

6- C Program to Generate Multiplication Table "1*3=3, 2*3=6, ..."
7- C Program to Check Whether a Character is an Alphabet or not
8- C Program to count number of Alphabets & number of words in a sentence. (word count) (required)
9- C Program to display "MagicBox"

function of x and y
-------------------
#include<windows.h>

COORD coord={0,0};                   // this is global variable
                                    //center of axis is set to the top left cornor of the screen
 void gotoxy(int x,int y)
 {
   coord.X=x;
   coord.Y=y;
   SetConsoleCursorPosition(GetStdHandle(STD_OUTPUT_HANDLE),coord);
 }
------------------------------------------------
Answer the following questions:
--------------------------------

## 1- C Program to take an array elements from user, then print them out. (Print Array)

## 2- C Program to find the maximum value of array elements. (Max Array)

## 3- C Program to add two matrix and put the result in a third one, then print the result.

## 4- C Program to find Sum & Average of 2D Array.
------------------------------------------------
# Assignment 4
Answer the following questions:
--------------------------------

## 1- C Program to take firstName and lastName from user, then displays fullName.

## 2- C Program to Find the Frequency of Characters in a String

## 3- C Program to take char and displays if it is "Normal or Extended key" along with its Ascii value.
 
## 4- New Colored Menu "with Arrows"



# Answer "as much as you can" from the following:
------------------------------------------------

## 5- C Program to Copy String Without Using strcpy()

## 6- C Program to Find the Length of a String without Using strlen()

## 7- C Program to Remove all Characters in a String Except Alphabet


------------------------------------------------------------------------------

#include<windows.h>

COORD coord={0,0};                   // this is global variable
                                    //center of axis is set to the top left cornor of the screen
 void gotoxy(int x,int y)
 {
   coord.X=x;
   coord.Y=y;
   SetConsoleCursorPosition(GetStdHandle(STD_OUTPUT_HANDLE),coord);
 }


void SetColor(int ForgC)
 {
    WORD wColor;

    HANDLE hStdOut = GetStdHandle(STD_OUTPUT_HANDLE);
    CONSOLE_SCREEN_BUFFER_INFO csbi;

    if(GetConsoleScreenBufferInfo(hStdOut, &csbi))
    {
        wColor = (csbi.wAttributes & 0xF0) + (ForgC & 0x0F);
        SetConsoleTextAttribute(hStdOut, wColor);
    }
    return;
}
------------------------------------------------
# Assignment 5
## Answer the following questions:
--------------------------------

1. write a function takes 3 numbers as parameter, and returns the largest one among them... write a program to test it.

2- C Program to take single Employee's information, and display them. (Emp_Struct)

3- C Program to take information of Array of Employees, then display them. (EmpArr_of_Struct)

4- Struct inside struct (Dept has Multiple Employees)

5- try to divide Ass#2 into 2 functions: 
	struct Employee AddEmployee();
	void DisplayEmployee(struct Employee); 

6- "Menu" of Array_Of_Struct



## Answer "as much as you can" from the following:
------------------------------------------------

5- C Program to Calculate Difference Between Two Time Period (Time_struct)
------------------------------------------------
# Assignment 6
Answer the following questions:
--------------------------------

## 1. C Program to swap 2 integer values. (Swap function, calling by address)


## 2. C Program that takes an array of integers and pass that array to a function to print array values after multiplying them to 10. 
	(try to use "Array Notation" and "Pointer notation")
	


## 3. C Program have a function changes the position of the first point of a given line struct "each line have 2 points", 
	then inside main displays the new coordinates along with line Length. (Pointer to struct)
   	function prototype should be like: 
		void change_Position(struct line *L, int newX, int newY)


## 4. C Program that asks the user for number of Lines he want "line is a struct, each line have 2 points", 
	then displays length of each one.(Dynamic Allocation of 1D Array of objects)

------------------------------------------------
# Assignment 7

Answer the following questions:
--------------------------------


## 1. C Program that has Array of pointers to struct Employee. (Array of pointers to struct) Array size is 3.

## 2. C Program to calculate sum of student degrees, and average of each subject, asks the user for students and subject numbers. (Dynamic Allocation of 2D Array - Pointer to Pointer)



# Answer "as much as you can" from the following:
------------------------------------------------

- Try to implement --jagged array-- on Assinment No.2 , which means:
 each student may have number of subjects different than the other. 
 and asks the user for each pointer size.


