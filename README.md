PRINTING PATTERN:
6666

555

44

3

PREREQUISITE:
Basic knowledge of C language and use of loops.

ALGORITHM:
Take the number of rows as input from the user  and store it in any variable.(‘r‘ in this case).
Initialise an integer variable count=r+2 .
Run a loop ‘r’ number of times to iterate through each of the rows. From i=0 to i<r. The loop should be structured as for( i=0 ; i<r : i++).
 Run a nested loop inside the main loop to print the digits in each row of the triangle. From j=r to j>i. The loop should be structured as for( j=r; j>i ; j–).
In the nested loop print count.
In the main loop decrement count and print a new line.
CODE IN C:
#include<stdio.h>
int main()
{
int i,j,r,count;//declaring integer variables i,j for loops , r for number of rows
printf("Enter the number of rows/columns :\n");//asking user for the number of rows;
scanf("%d",&r);//taking number of rows and saving in variable r
count=r+2;
for(i=0;i<r;i++) //loop for number of rows
   {
      for(j=r;j>i;j--)//loop to print digit in every column of a row
         {
            printf("%d",count);//printing digit
         }
      count--;
      printf("\n");//printing newline
   }
}
TAKING INPUT:
DISPLAYING OUTPUT:
