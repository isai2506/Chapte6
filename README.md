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

## Exercise 6.4

     #include <stdio.h>

    char line[100];/* line of input data */
    int amount;
    int quarters; /* the height of the rectangle */
    int dimes; /* the width of the rectangle */
    int nickels; /* perimeter of the rectangle (computed) */
    int pennies;
    int main()
    
    {
    printf("Give an amount of money less than $1.00 (in cents) ");
    fgets(line, sizeof(line), stdin);

    sscanf(line, "%d", &amount);
   
    quarters = (amount/25);
    printf("Quarters: %d\n", quarters);

    dimes = (amount-25*quarters)/10;
    printf("Dimes: %d\n", dimes);

    nickels = (amount-25*quarters-10*dimes)/5;
    printf("nickels: %d\n", nickels);

     pennies = (amount-25*quarters-10*dimes-5*nickels);
     printf("Penniess: %d\n", pennies);
     
    return (0);
 
     }
     
 ## Exercise 6.5

    #include <stdio.h>
    int main() {
    int year;
    printf("Enter a year: ");
    scanf("%d", &year);

  
    if (year % 400 == 0) {
       printf("%d is a leap year.", year);
     }
    else if (year % 100 == 0) {
      printf("%d is not a leap year.", year);
     }
       else if (year % 4 == 0) {
      printf("%d is a leap year.", year);
    }
    else {
      printf("%d is not a leap year.", year);
    }
     return 0;
    }

## Exercise 6.6

    #include <stdio.h>
    int main() {
    int hour;
    int pay;
    int pay2;
    printf("Enter number of hours worked in the week: ");
    scanf("%d", &hour);
    int h; /*For each hour worked the payment is 100 pesos */
    h=100;

    pay=(hour*h);
    pay2=(pay*1.5);

    if (hour<=40)
    printf("Your weekly pay is %d\n pesos", pay);
       else if(hour>=40)
       printf("Your weekly pay is %d\n pesos", pay2);
    
    return 0;
    }



