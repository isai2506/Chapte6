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

##  Exercise 6.2

#include<stdio.h> 

int main()

{

int number;

printf("Enter a number betwen 0 and 100: "); 

scanf("%d", &number);

if (number>-1 && number<61)

printf("F", number);

    else if(number>60 && number<71)
    
    printf("D", number);
    
      else if(number>70 && number<81)
      
      printf("C", number);
      
        else if(number>80 && number<91)
        
        printf("B", number);
        
           else if(number>90 && number<101)
           
           printf("A", number);
 
 return(0);
 
 }

## Exercise 6.3 

    #include <stdio.h>

char line[100];             
int score;
char plusminus;

int main() {
    printf("Enter a number between 0 and 100: ");     
    fgets(line, sizeof(line), stdin);
    sscanf(line, "%d", &score);


    if (score <= 60) 
        printf("F");
    
    if (score <= 70 && score >60) {
        printf("D");
    }
    if (score <= 80 && score >70) {
        printf("C");
    }
    if (score <= 90 && score >80) {
        printf("B");
    }
    if (score <= 100 && score >90) {
        printf("A");
    }

    plusminus = line[1];
    if (plusminus < "3") {
        printf("-");
    }
    if (plusminus > "8") {
        printf("+");
    }
}
