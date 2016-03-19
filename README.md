# Venturesity
//Code for Subset of maximum sum
//This code gets two subsets odd and even subset and prints the sum of each.

#include <stdio.h>

int main() 
{
  int a[10],n,i,sum_odd=0,sum_even=0;
  printf("Enter the size of array \n");
  scanf("%d \n",&n);
  printf("Enter %d elements of array \n",n);
  for(i=0;i<n;i++)
  {
    scanf("%d \n",&a[i]);
  }
  for(i=0;i<n;i++)
  {
    printf("a[%d]=%d \n",i,a[i]);
  }
  for(i=0;i<n;i++)
  {
    if((i%2)==0)
    {
    	sum_even+=a[i];
    }
    else
    {
    	sum_odd+=a[i];
    }
  }
  printf("Sum of elements of odd subset is : %d \n",sum_odd);
 
  printf("Sum of elements of even subset is :%d \n",sum_even );
	return 0;
}
