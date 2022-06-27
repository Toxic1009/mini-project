# mini-project

#include <stdio.h>
#include <stdlib.h>

// for sleep() function
#include <math.h>
int main() 
{
float principal_amount, rate, time, emi;
printf("Enter the principal amount: ");
scanf("%f",&principal_amount);
printf("Enter the rate: ");
scanf("%f",&rate);
printf("Enter the time in years: ");
scanf("%f",&time);
// one month interest
rate=rate/(12*100);
// one month period
time=time*12; 
emi= (principal_amount*rate*pow(1+rate,time))/(pow(1+rate,time)-1);
printf("The Monthly EMI is = %f\n",emi);
return 0;
}

TEST CASES (1) :
Enter the principal amount: 1000000
Enter the rate: 10
Enter the time in years: 5
The Monthly EMI is = 21247.062500

TEST CASES(2) :
Enter the principal amount: 56892314
Enter the rate: 44
Enter the time in years: 8
The Monthly EMI is = 2153953.000000
