# Max-Element-in-Array-using-c

Max Element in Array 
Find the maximum element from the given array of integers.

Input Format:
﻿The first line of input contains N - the size of the array and the second line contains the elements of the array.

Output Format:
Print the maximum element of the given array.

Constraints:
1 <= N <= 10^3
-10^9 <= ar[i] <= 10^9

Example
Input
5
-2 -19 8 15 4

Output
15

#include <stdio.h>
#include <stdlib.h>
int main() {  
   int n,i,max;
   long long a[1000];
   scanf("%d",&n);
   for(i=0;i<n;i++)
   scanf("%lld",&a[i]);
   max=a[0];
   for(i=1;i<n;i++)
   {
       if(a[i]>max)
       max=a[i];
   }
   printf("%d",max);
    return 0;
}
