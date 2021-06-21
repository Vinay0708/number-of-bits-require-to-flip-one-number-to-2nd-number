# number-of-bits-require-to-flip-one-number-to-2nd-number
#include<stdio.h>
#include<math.h>
int main()
{   
    int n,x,y,r,count;
    printf("Please provide two number:\n");
    scanf("%d%d",&n,&x);
    y=n^x;
    count=0;
    while(y>0)
   {
    y=y&(y-1);
    count++;
   }
   printf("number of bits require to flip:%d",count);
    return 0;
}
