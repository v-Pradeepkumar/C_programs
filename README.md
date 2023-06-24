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





