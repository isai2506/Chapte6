## Chapter6
## Exercise 6.1

#include<stdio.h> 

#include<stdlib.h> 

#include<math.h>

int main()


{

float x1, x2, y1, y2, distance, square;

printf("Enter point 1: "); 

scanf("%f %f",&x1,&y1);

printf("Enter point 2: ");

scanf("%f %f",&x2,&y2);



distance = sqrt(pow((x2-x1),2)+pow((y2-y1),2));

square = pow((distance),2);

 printf("The distance between the two points is %.2f. ", distance);
 
 printf("The square of the distance is %.2f", square);
 
 return(0);
 
 
 }
