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
