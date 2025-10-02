//C program
/*
Name: Wamagata Lynn Njeri
Reg no:CT101/G/26423/25
Description:Water_bill
*/
#include <stdio.h>
int main ( ) {
    int units;
    float bill;

  printf("Enter the number of water units_ consumed: ");
    scanf("%d", &units);
    
    if (units >= 0 && units <= 30) {
        bill = units * 20;
    } 
    else if (units > 30 && units <= 60) {
        bill = (30 * 20) + ((units - 30) * 25);
    } 
    else if(units > 60) {
        bill = (30 * 20) + (30 * 25) + ((units - 60) * 30);
    } 
    printf("The total water bill is KES %.2f\n", bill);

    return 0; 
}
