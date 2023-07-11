// Online C compiler to run C program online
#include <stdio.h>

int main()
{
   int n,i,j;
   printf ("enter the number of columns you want in your Pyramid\n");
   scanf("%d",&n);
   for(i=1;i<=n;i++)
   {
       for(j=1;j<=2*n-1;j++)
       {
           if(j>=n-(i-1)&&j<=n+(i-1))
           {
               printf("*");
           }
           else
           printf(" ");
       }
       printf("\n");
   }
    return 0;
}



// function to find the area of reactangle
#include <stdio.h>
int areaOfRect(int length, int breadth)
{
    int area;
    area = length * breadth;
    return area;
}
int main()
{
 int l=50, b=50;
 int area = areaOfRect(l,b);
    printf("%d\n",area);

    return 0;
}



//function for return a character
#include <stdio.h>

char fun();

int main()
{
 char c = fun();
 printf("character is; %c",c);
}

   char fun()
   {

    return 'a';
}

//function for adding two numbers
#include <stdio.h>

int add(int,int);

int main()
{
 int m =20, n = 30, sum;
 sum = add(m, n);
 printf("sum is; %d",sum);
 return 0;
}

   int add(int a, int b)
   {

    return (a + b);
}

// function to find the area of reactangle
#include <stdio.h>
int areaOfRect(int length, int breadth)
{
    int area;
    area = length * breadth;
    return area;
}
int main()
{
 int l=50, b=50;
 int area = areaOfRect(l,b);
    printf("%d\n",area);

    return 0;
}





//function for return a character
#include <stdio.h>

char fun();

int main()
{
 char c = fun();
 printf("character is; %c",c);
}

   char fun()
   {

    return 'a';
}



//function for adding two numbers
#include <stdio.h>

int add(int,int);

int main()
{
 int m =20, n = 30, sum;
 sum = add(m, n);
 printf("sum is; %d",sum);
 return 0;
}

   int add(int a, int b)
   {

    return (a + b);
}



//palindrome code
include <stdio.h>

int main() {
    int n, result=0,rem,q;
    printf ("please enter the number: ");
    scanf("%d",&n);
    q=n;
    while (q!=0)
    {
        rem =q%10;
        result=result *10+rem;
        q=q/10;
        
    }
    if(result==n)
    printf("it is a palindrome");
    else
    printf("No!its not a palindrome");

    return 0;
}




//code for adding two numbers without + operator
#include <stdio.h>

int main() {
    // Write C code here
int x , y;
printf("enter two numbers:");
scanf("%d, %d",&x , &y);
while (y!= 0)
{
    x++;
    y--;
}
printf("the addition of two number is %d",x );
    return 0;
}





//code for adding two numbers without + operator also for positive and negative numbers
#include <stdio.h>

int main() {
    // Write C code here
int x , y;
printf("enter two numbers:");
scanf("%d, %d",&x , &y);
if (y>0)
{
    while (y!=0)
    {
    x++;
    y--;
        
    }
}
else if (y<0)
{
    while (y!=0)
    {
    x--;
    y++;
}
}
printf("the addition of two number is %d",x );
    return 0;
}




//code for adding two numbers without + operator using half adder
#include <stdio.h>

int main() {
    // Write C code here
int sum,carry,  x , y;
printf("enter two numbers:");
scanf("%d, %d",&x , &y);

    while (y!=0)
    {
    sum = x^y;
    carry = (x&y)<<1;
    x = sum; 
    y= carry;
}
printf("the addition of two number is %d",x );
    return 0;
}




//writing c program for fibonoci series

#include <stdio.h>

int main()
{

int a,b,result,n,i;
printf("enter the number of terms:");
scanf("%d",&n);


a = 0;
b= 1;

for(i=1;i<=n;i++)
{
printf("%d",a );
result = a+b;
a=b; 
b = result;
}

}





//print the format of floyd's triangle
/*
1 
2 3 
4 5 6 
7 8 9 10 
11 12 13 14 15 
16 17 18 19 20 21 
22 23 24 25 26 27 28 
29 30 31 32 33 34 35 36 
37 38 39 40 41 42 43 44 45 
#include <stdio.h>*/ 
// output

int main()
{

int i, j, rows, n=1;
printf("enter the number of rows:");
scanf("%d",&rows);


for(i=0;i<=rows;i++)
{
    for(j=0;j<=i;j++)
    {
        printf("%d ",n);
        n++;
        
    }
    printf("\n");
}
return 0 ;
}





//convert binary to decimal
#include <stdio.h>

int main()
{
int decimal=0,binary ,base=1 ,rem , num;
printf("enter the binary number:");
scanf("%d",&binary);

num = binary;
while(binary!=0)
{
    rem = binary % 10;
    decimal = decimal + rem * base;
    binary = binary / 10;
    base = base * 2;
}
printf("decimal equivalent of the binary number %d is %d",num, decimal);
return 0;
}





//decimal eqivalent for the exponential value and positive power numbers
#include <stdio.h>

int main() {
    int base ,exponent ,expo ,power = 1;
    double power1 = 1.0 ;
    printf("enter the base: ");
    scanf("%d",& base);
     printf("enter the exponent: ");
    scanf("%d",& exponent);
    
    expo=exponent;
    if (exponent > 0)
    {
        while (exponent!= 0)
        {
            power = power * base ;
            exponent--;
        }
        printf("%d to the power of %d is %d",base , expo, power);
        
    }
    else
    {
        while(exponent!= 0)
        {
        power1 = power1 * (1.0/base);
            exponent++;
        }
        printf("%d to the power of %d is %.10f ,base , expo , power");
        }

    return 0;
}






// find the year is leap year or not
#include <stdio.h>

int main() {
    int year;
    printf("entter the year:");
    scanf("%d",&year);
    if (year % 400 == 0)
    printf("%d is leap year",year);
    else  if (year % 100 == 0)
    printf("%d is not a leap year",year);
    else if (year % 4 == 0)
    printf("%d is leap year",year);
    else
    printf("%d is not a leap year",year);
    return 0;
}





// code for perfect number means-all its factors addition is that number eg: 6 =1+2+3=6
#include <stdio.h>

int main() {
    int number;
    printf("enter the number:");
    scanf("%d", &number);
    
    int i,rem,sum=0;
    for(i=1;i<number;i++)
    {
        rem = number%i;
        if(rem==0)
        {
            sum = sum+i ;
        }
    }
if (sum == number)
 {
     printf("%d is a perfect number",number);
 }
 else 
 {
 printf("%d is not a perfect number",number);
 }
    return 0;
}
