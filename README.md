# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <math.h>
void emic(float,float,float);
int main()
{
    float principle,rate,time;
    scanf("%f%f%f",&principle,&rate,&time);
    printf("Monthly EMI is= %.3f",emic(principle,rate,time));
    return 0;
}
void emic(float p, float r,float t)
{
    float emi;
    r=r/(12*100);
    t*=12;
    emi=(p*r*pow(1+r,t))/(pow(1+r,t)-1);
}
```


## OUTPUT
![Screenshot 2025-05-06 094715](https://github.com/user-attachments/assets/05171bcb-8fb7-4802-b5e8-a2f93c25d2a6)


## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main()
{
    int i=3,n,sum=0,a=0,b=1;
    scanf("%d",&n);
    printf("%d %d ",a,b);
    while(i<=n)
    {
        sum=a+b;
        printf("%d ",sum);
        a=b;
        b=sum;
        i++;
    }
    return 0;
}
```
## OUTPUT
![Screenshot 2025-05-06 095019](https://github.com/user-attachments/assets/b5f99bee-845d-4e1e-9ce6-52d331de5fed)








## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main()
{
 int i,n,a[10];
 scanf("%d",&n);
 for(i=0;i<n;i++)
  scanf("%d",&a[i]);
 printf("%d",a[n-1]);
}
```

## OUTPUT

![Screenshot 2025-05-06 095548](https://github.com/user-attachments/assets/c6c493cf-37b7-4de7-bcc3-59d047255e38)

## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main()
{
 int i,n,a[10],c=0;;
 scanf("%d",&n);
 for(i=0;i<n;i++)
  scanf("%d",&a[i]);
 for(i=0;i<n;i++)
{
 if(a[i]>0)
  c++;
}
printf("Positive elements in a array: %d",c);
}
```


## OUTPUT
![Screenshot 2025-05-06 100414](https://github.com/user-attachments/assets/1ea78ddc-60ee-474f-b3a3-fd9f27a3a139)






## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
```
#include <stdio.h>
int main()
{
 int i,n,a[10];
 printf("Enter Number of elements:");
 scanf("%d",&n);
 printf("Enter elements:");
 for(i=0;i<n;i++)
   scanf("%d",&a[i]);
 if(a[i]%2==0)
  a[i]='E';
 for(i=0;i<n;i++)
 {
  if(a[i]=='E'
   printf("E ");
  else
   printf("%d",a[i]);
 }
}
```
## Output:
![Screenshot 2025-04-27 203414](https://github.com/user-attachments/assets/4ed29a55-b2f2-485b-bff0-3a06da1031b8)

 


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



