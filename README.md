#include<stdio.h>
int sum_given_number(int n);
int main()
{
	int a,n;
	printf(" enter the number:");
	scanf("%d",&n);
	a=sum_given_number(n);
	printf(" sum of given number is %d \n",a);
}
int sum_given_number(int n)
{
	int r,sum=0;

	while(n>0)
	{
		r=n%10;
		sum=sum+r;
			n=n/10;
	}
	return sum;
}
