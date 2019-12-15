             ××××××××××××××××××
             ×   PRACTICAL FILE     ×
             ××××××××××××××××××
         
         












** • PROGRAMMING FOR PROBLEM SOLVING ESC-19104**

  **  • NAME- KANISHKA SHARMA**  
  
  **  •BRANCH - INFORMATION      TECHNOLOGY ** **  (B.TECH -FIRST YEAR)**
  
  ** ROLL NO.- 1905349**
  
  
  
  









** 1.) • WRITE A PROGRAM TO FIND WHETHER A NUMBER IS POSITIVE OR NEGATIVE :** 
  
  
```c 
#include<stdio.h>  
int main()
{ 
int n;
printf("enter any value\n");
scanf("%d",&n); 
if(n>0) printf(" the number entered is positive.\n");
else  
printf("the number entered is negative.\n");  
}  
```  


**Output:**
enter any value
6
 the number entered is positive
 
 


 **2.) • WRITE A PROGRAM TO FIND WHETHER A NUMBER IS ODD OR EVEN :** 
```c  
#include<stdio.h>  
int main() 
{  
int n; 
printf("enter any number:");  scanf("%d",&n); 
if(n % 2 == 0)  
printf("The number is even\n");  else  
printf("The number is odd\n");  
}  
```  


**Output:**
 enter any number:
   8465717
The number is odd                       






** 3.) • WRITE A PROGRAM TO FIND WHETHER A NUMBER IS PRIME OR NOT :** 
```c  
#include<stdio.h>  
int main() 
{  
int i,n;  
printf("enter any natural number\n");  
scanf("%d",&n);  
for(i=2;i<=n-1;i++)  
{  if(n%i==0)  
break;  
}  
if(i==n)  
{  
printf("the entered number is a prime number.\n",n);
}  
else  
printf(" the entered number is not prime number\n",n);  
return 0;  
}  
``` 


**Output:**
enter any natural number
67
the entered number  is a prime number.





 ** 4.) •WRITE A PROGRAM TO CHECK WHETHER A NUMBER IS PRIME OR NOT IN A RANGE :**
```c  
#include<stdio.h> 
int main()  
{ 
int i,j,s,l,p;  
printf("enter the starting number : \n");  
scanf("%d",&s);  
printf("enter the last number
:");  
scanf("%d",&l);   for(j=s;j<l;j++)  
{  
for(i=2;i<j;i++)
{  if(j%i==0)  
{  
p=1;  
}  
}  
if(p==1)  
printf("%d is not prime\n",j);  else  
printf("%d is prime\n",j);  
}  
return 0; 
}  
```  



**Output:**
enter the starting number :
5
enter the last number : 9                                                               5 is prime                                                                              6 is not prime
7 is prime
8 is not prime








** 5.) • WRITE A PROGRAM TO FIND FACTORIAL OF A NUMBER:** 
```c  
#include<stdio.h> 
int main()  
{  
int c,n,fact=1;  
printf("enter a number to calculate it's factorial:\n");  scanf("%d",&n);  for(c=1;c<=n;c++)  
fact=fact*c;  
printf("factorial of %d =%d\n",n,fact);  
return 0;  
} 
```



**Output:**
enter a number to calculate it's factorial:
8
factorial of 8 =40320






**  6.) •  WRITE A PROGRAM TO FIND TO WRITE TABLE OF A NUMBER: **

```c
#include<stdio.h>  
int main()  
{  
int i,n;  
printf(" enter any number = \n");  scanf("%d",&n);  for(i=1;i<=10;i++)  printf("%d×%d=%d\n",n,i,n*i);  return (0);  
} 
```  



**Output:**
enter any number =
23
23×1=23
23×2=46
23×3=69
23×4=92
23×5=115
23×6=138
23×7=161
23×8=184
23×9=207
23×10=230








**7.) • WRITE A PROGRAM TO FIND FACTORIAL OF A NUMBER USING RECURSION :**

```c  
#include<stdio.h>  
int factorial(int n);  
int main()  
{  
printf("enter a number: \n");      int fact;
scanf("%d",&fact);  printf("%d\n",factorial(fact));  return 0;  
}  
int factorial(int n)  
{ 
int a;  
if(n==0)  
{  
a=1;  
}  
else  
a=n*factorial(n-1);  
return a;  
} 
``` 



**Output:**
enter a number:
6
720





**
 8.) • WRITE A PROGRAM TO CONVERT TEMPERATURE IN°C TO °F :
** 
 
```c 
#include<stdio.h>  
int main()  
{ 
float c,f; 
printf("enter temperature in fahrenheit \n"); 
scanf("%f",&f);  
c=((f-32)*5)/9;  
printf("the temperature in celcius is %f\n",c);  
}  
``` 



**Output:**
enter temperature in fahrenheit
45
the temperature in celcius is 7.222222








** 9.) •WRITE A PROGRAM TO WRITE TABLE OF A EVEN NUMBER : 
 **
```c  
#include<stdio.h>  
int main()  
{  
int i,n; 
printf("enter any number = \n");   scanf("%d",&n); if(n%2==0)  {  for(i=0;i<=10;i++)  
{  
printf("%d×%d=%d\n",n,i,n*i);  
}
}  
else  
printf("the number is not even \n");
return (0);  
}  
```



**Output:**
enter any number =
14
14×0=0
14×1=14
14×2=28
14×3=42
14×4=56
14×5=70                                                                                 14×6=84
14×7=98
14×8=112
14×9=126
14×10=140





**10.) • WRITE A PROGRAM FOR ADDITION OF TWO MATRICES :  **
```c 
#include <stdio.h>  
int main()  
{
int m,n,c,d,first[10][10], second[10][10], sum[10][10]; 
printf("Enter the number of rows and columns of matrix\n");
scanf("%d%d", &m, &n);  printf("Enter the elements of first matrix\n"); 
for ( c = 0 ; c < m ; c++ )  
for ( d = 0 ; d < n ; d++ )  scanf("%d", &first[c][d]); 
printf("Enter the elements of second matrix\n");  
for ( c = 0 ; c < m ; c++ )  
for ( d = 0 ; d < n ; d++ )  scanf("%d", &second[c][d]);  
for ( c = 0 ; c < m ; c++ )  
for ( d = 0 ; d < n ; d++ )  sum[c][d] = first[c][d] + second[c][d];  
/* Matrix addition */  printf("Sum of entered matrices:-\n");  
for ( c = 0 ; c < m ; c++ )  
{  
for ( d = 0 ; d < n ; d++ )  printf("%d\t", sum[c][d]);  printf("\n");  
}  
return 0;  
} 
```


**Output:**
the number of rows and columns of matrix
2
2
Enter the elements of first matrix
3
1
3
3
Enter the elements of second matrix
4
5
6
43
Sum of entered matrices:-
7       6
9       46







**11.) • WRITE A PROGRAM TO SHOW A PYRAMID OF * BY ENTERING THE NO. OF ROWS : **

```c  
#include<stdio.h>  
int main()  
{  
int i,j,n;  
printf("\nEnter number of Rows: ");  scanf("%d",&n);  
printf("\n");  
for(i=1; i<=n; i++)  
{  
for(j=1; j<=2*n-1; j++)  
{  
if(j>=n-(i-1) && j<=n+(i-1))  
printf("*");  
else  
printf(" ");  
}  
printf("\n");  
}  
return 0;  
} 
```



**Output:**
Enter number of Rows: 5                                                                
      * 
     ***
   ***** 
 ********
**********
                                                                                                                            
 
 
 


 **  12.) • WRITE A PROGRAM TO REVERSE NUMBERS :**
```c  
 
#include<stdio.h> 
intt main()
{ 
 int n,reversedValue=0,remainder;     printf(" enter any value of n:\n"); 
scanf("%d",&n);  
while(n!=0)  
{  
remainder =n%10;  reversedValue=reversedValue*10+remainder;  n/=10;  
}  printf("reversed Value=%d\n",reversedValue);  
return 0;  
}  
``` 



**Output:**
enter any value of n:
27
reversedValue=72






**13.). WRITE A PROGRAM TO FIND THE GREATER AMONG ARRAY :**


```c  
#include<stdio.h> 
int main() 
{  
int array[50],i,size,largest;  printf("enter the size of array \n");  
scanf("%d",&size);  
printf(" enter %d element of array : ",size);  for(i=1;i<=size;i++)  scanf("%d",&array[i]);  largest=array[0];  for(i=1;i<=size;i++)  
{  
if(largest<array[i])  largest =array[i];  
}  
printf("\n largest number is %d",largest);  
return 0;  
}
```


**Output:**
enter the size of array
4
 enter 4 element of array : 2
7
5
77

 largest number is 77





**14.) WRITE A PROGRAM TO MAKE A PATTERN : **

```c 
#include<stdio.h>  
int main()  
{  
int i,j,n;  
printf("\nEnter number of Rows: ");  
scanf("%d",&n); 
for(i=1; i<=n; i++) 
{ 
for(j=1; j<=i; j++) 
{  printf("*"); 
}  
printf("\n");  
}  
return 0;  
}  
```  



**Output:**
Enter number of Rows: 6
  *
  **
  ***
  ****
  *****
  ******





**15.) WRITE A PROGRAM FOR TOTAL EXPERIENCE OF EMPLOYEES :  **

```c 
#include<stdio.h> 
int main()  
{  
int n,exp,sum=0;  
printf("enter the no. of         employees :\n");  
scanf("%d",&n);  
for(int i=1;i<=n;i++)  
{  
printf(" enter the experience (in years):\n"); 
scanf("%d",&exp); 
sum=sum+exp;  
}  
printf("%d\n",sum);  
return 0;  
} 
```  



**Output:**
enter the no. of employees :
4
  enter the experience (in years):
2
  enter the experience (in years):                                                      5
  enter the experience (in years):
3
  enter the experience (in years):
4
 14






**16.) • WRITE A PROGRAM FOR MULTIPLICATION OF TWO MATRICES: **
 
 ```c
 
 #include<stdio.h> 
 int main()
 {  
 int sum=0,m,n,p,q,matrix ; 
 //for matrix 1  
 printf("please enter the number of    rows of 1st matrix:\n");  scanf("%d",&m);  
 printf("please enter the number of columns of 1st matrix:\n");
 scanf("%d",&n);  
 printf("please enter the number of rows of 2nd matrix:\n");   scanf("%d",&p);  
printf("please enter the number of columns of 2nd matrix:\n");  
scanf("%d",&q); 
 if(n==p)
 {  
 int matrix1[m][n]; 
  int matrix2[p][q];  
  printf("for matrix 1\n");  
  for(int  i=1;i<=m;i++)
  {
 for(int j=1;j<=n;j++)
 {  
 printf("please enter the value of matrix 1 at %d th row and %d th col$  ");
 scanf("%d",&matrix1[i][j]);  
 }
 }  
 printf("matrix 1 is :\n");  
 for(int i=1;i<=m;i++)
 {  
 for(int j=1;j<=n;j++)
 {  
 printf("%d\t",matrix1[i][j]);  
 if(j==m)  
 printf("\n");  
 }
 } 
  //for matrix 2  
  printf("for matrix 2 \n");  
  for(int k=1;k<=p;k++)
  {  
  for(int l=1;l<=q;l++)
  {  printf("please enter the value of matrix 1 at %d th row and %d th col$  scanf("%d",&matrix2[k][l]);  }
  }  
 printf("matrix 2 is :\n");  
 for(int k=1;k<=p;k++)
 {  
 for(int l=1;l<=q;l++)
 {  
 printf("%d\t",matrix2[k][l]);  
 if(l==p)  
 printf("\n"); 
  }
 }
   //for multiplication 
    int martix[m][q];  
    for(int a=1;a<=m;a++)
    {  
    for(int b=1;b<=q;b++)
    {  for(int c=1;c<=p;c++)
    {  
    sum=sum+matrix1[a][c]
    *matrix2[c][b];
    }  
    matrix1[a][b]=sum;  
    sum=0;}
    }  
    printf("product of matrices is:\n");       
    for(int a=1;a<=m;a++)
    {  
    for(int b=1;b<=q;b++)
    {  
    printf("%d\t",matrix1[a][b]);  
    if(b==m)  
    printf("\n");
    }
    }  
    }  
    else  
    printf("for multiplication of 2 
    matrices the matrices the number of 
    columns of first matrix should be 
    equal to the number of rows of 
    second matrix.");  
    return 0;  
   }
   '''  
   
   
 
  **Output:**
    please enter the number of rows of 1st matrix:
2
please enter the number of columns of 1st matrix:
2
please enter the number of rows of 2nd matrix:
2
please enter the number of columns of 2nd matrix:
2
for matrix 1
please enter the value of matrix 1 at 1 th row and 1 th column1
please enter the value of matrix 1 at 1 th row and 2 th column4
please enter the value of matrix 1 at 2 th row and 1 th column2
please enter the value of matrix 1 at 2 th row and 2 th column1
matrix 1 is :
1       4
2       1
for matrix 2
please enter the value of matrix 1 at 1 th row and 1 th column3
please enter the value of matrix 1 at 1 th row and 2 th column1
please enter the value of matrix 1 at 2 th row and 1 th column21
please enter the value of matrix 1 at 2 th row and 2 th column2
matrix 2 is :                                                                           3       1                                                                               21      2
product of matrices is:
87      95
27      29
     
     
     


**17.) • WRITE A PROGRAM TO FIND TABLE OF NUMBER IN A RANGE:**


```c
#include<stdio.h>                              
int main()
{
int a,b,i,j;
printf("enter starting no. :\n");
scanf("%d",&a);
printf("enter last no. :  \n");
scanf("%d",&b);
for(i=a;i<=b;i++)
{
for(j=1;j<=10;j++)                                                                      printf(" %d*%d=%d\n",i,j,i*j);                                                          }
return 0;
}
```



**Output:**
enter starting no. :
2
enter last no. :
4                                                                                        2*1=2                                                                                   2*2=4
 2*3=6
 2*4=8
 2*5=10
 2*6=12
 2*7=14
 2*8=16
 2*9=18
 2*10=20
 3*1=3
 3*2=6
 3*3=9
 3*4=12
 3*5=15
 3*6=18
 3*7=21
 3*8=24
 3*9=27
 3*10=30
 4*1=4
 4*2=8
 4*3=12
 4*4=16
 4*5=20
 4*6=24
 4*7=28
 4*8=32
 4*9=36
 4*10=40
 
 
 
 
 
 **  18.)  WRITE A PROGRAM TO DRAW A JOKER FACE:**
 

 ```c
#include<stdio.h>
int main()
{
puts("_______________");
puts("|  XXXXXXXXX  |");
puts("|  ( ^   ^ )  |");
puts("|  ( 0   0 )  |");
puts("|   \\  |  /   |");
puts("|    \\ = /    |");
puts("|     \\_/     |");
puts("|      |      |");
puts("|______|______|");
return 0;
}
```

**Output:**

_______________
|  XXXXXXXXX  |
|        ( ^   ^ )       |
|        ( 0   0 )       |
|         \  |  /         |
|         \ = /         |
|          \_/            |
|             |              |
|_______|_______|





** 19.) WRITE A PROGRAM TO DRAW A CALCULATOR : **



```c

#include<stdio.h>
void main()                                              
{
puts("  ____________________\n\
      |_______________|____||\n\
      |   1   |   2   |  3 ||\n\
     |____|_____|____|____|   \n\                 |  4  |  5  |  6  |   +  | \n\
    |_____|____|_____|____|\n\
   |   7   |   8   |   9   |   -   |  \n\
           |_____|____|_____|_ ___| \n\
           |     0                    |   *   |\n\
           |_______________|_____|\n"\
            
 ```
     
   ** Output:**
      ________________
      |_______________|
      |  1   |  2  |  3  |     |
      |____|____|___|      |
       |  4    |   5  |   6  | +  |
       |____|____|___|___|
     |  7   |  8   | 9  |   - |
     |____|____|___|___|
     |     0              |  *  |
     |____________|___|
   
   
   
 
 



** 20.)  WRITE A PROGRAM TO  SWAP A NUMBER :**
 
 
 #include<stdio.h>
int swap(int a,int b);
int main()
{
int a,b;
printf(" enter any two digit value a and b :\n");
scanf("%d"%d",&a,&b);
swap(a,b);
}
int swap(int a,int b);
{
a=a+b;
b=a-b;!
{
}
b=a-b;
printf("the value of a:%d\n",a);
printf("the value of b:%d\n",b);
}
```


**Output:**
Enter any two digit value a and b :
8
2
the value of a:2
the value of b:8



