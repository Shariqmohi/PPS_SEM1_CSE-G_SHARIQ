# For Loop in C

![Difficulty](https://img.shields.io/badge/Difficulty-Medium-yellow)

## Problem

**Objective** 

The modulo operator, `%`, returns the remainder of a division.  For example, `4 % 3 = 1` and `12 % 10 = 2`.  The ordinary division operator, `/`, returns a truncated integer value when performed on integers.  For example, `5 / 3 = 1`.  To get the last digit of a number in base 10, use $10$ as the modulo divisor.  

**Task**

Given a five digit integer, print the sum of its digits.  


**Input Format**

The input contains a single five digit number, $n$.

**Constraints**

$ 10000 \le n \le 99999$  

**Output Format**

Print the sum of the digits of the five digit number.

## Solution

**Language:** C  
**Runtime:** N/A  
**Memory:** N/A  
**Submitted:** 2026-10-02T11:14:56.609Z  

```c
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>



int main() 
{
    int a, b,i,r;
    scanf("%d\n%d", &a, &b);
  	// Complete the code.
for(i=a;i<=b;i++)
{  
   if(i<=9) 
   {
    switch(i)
    {
        case 1:printf("one\n");break;
        case 2:printf("two\n");break;
        case 3:printf("three\n");break;
        case 4:printf("four\n");break;
        case 5:printf("five\n");break;
        case 6:printf("six\n");break;
        case 7:printf("seven\n");break;
        case 8:printf("eight\n");break;
        case 9:printf("nine\n");break;
    }
    
   }
   else 
   {
    r=i%2;
    if(r==0)
      printf("even\n");
    else 
      printf("odd\n");
    
   } 
}

return 0;
}


```

---

[View on HackerRank](https://www.hackerrank.com/challenges/sum-of-digits-of-a-five-digit-number/problem)