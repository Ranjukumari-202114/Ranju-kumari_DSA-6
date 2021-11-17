# Ranju-kumari_DSA-6





/*write a program for swapping two numbers using 'call by value' and 'call by reference' strategies*/

#include <stdio.h>
void swap (int*, int*);

int main()
{
    int num1,num2;
    printf("enter the value of num1 = ");
    scanf("%d",&num1);
    printf("enter the value of num2 = ");
    scanf("%d",&num2);
    swap( &num1, &num2);
    printf(" The value of num1 = %d\nThe value of num2 = %d\n", num1,num2);
    return 0;
}
 
 void swap(int *x, int *y)
 {
     int t;
     t = *x;
     *x = *y;
     *y = t;
 }
