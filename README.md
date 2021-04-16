# project-1 cse 
#include<stdio.h>
int isperfect(int n)
{
	int i,sum=0;
	for(i=1; i<n; i++)
	{
	if(n%i==0)
	sum=sum+i;
	}
	if(sum==n)
	return 1;
	else
	return 0;
}
int main()
{
    int n;
    printf("Enter number: ");
    scanf("%d",&n);
    if(isperfect(n))
	printf("%d is perfect number.\n",n);
	else
    printf("%d is not perfect number.",n);
	return 0;
}
