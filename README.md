#include<stdio.h>
int digitsum(int num);
int main()
{
int n1,sum;
printf("\nRecursion:Find the sum of digits of a number:\n");
printf("input any number to find sum of digits");
scanf("%d",&n1);
sum=Digitssum(n1);
printf("the sum of digits of %d=%d\n",n1,sum);
return 0;
}
int Digitsum(int n1)
{
if(n1==0)
return 0;
return((n1%10)+Digitsum(n1/10));
}
