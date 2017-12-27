
/*
 * NAME: Alana Ruth
 *
 * Accepts two decimal integers, the first being nonnegative and the second being
 * between 2 and 16. Converts the first decimal integer into its representation
 * in radix of the second integer and prints the result.
 *
 */

#include <stdio.h>

main(void){

  //Declare two integer variables
  int d, r;


  //Prompt the user for two integers and read in the two integers
  printf("\nEnter two integers: "); fflush(stdout);
  scanf("%d%d", &d, &r);


  //Array to store the digits of a radix representation up to base 16
  char radixDigits[16] = {'0', '1', '2', '3', '4', '5', '6', '7', '8', '9', 'A', 'B', 'C', 'D', 'E', 'F'};


  //Array to store answer of radix representation
  char radixRepresentation[100];
  int i = 0;


  //Declare integer to store the remainder and the temporary quotient
  int remainder;
  int temp = d;


  //While loop to determine the representation in the radix specified
  while (temp !=  0){
    remainder = temp % r;
    temp = temp / r;

    //Stores answer in the array radixRepresentation
    radixRepresentation[i] = radixDigits[remainder];
    i++;
  }


  i--;

  printf("Answer = "); fflush(stdout);

  //If the integer entered is 0, the answer is 0
  if (d == 0){
    printf("0"); fflush(stdout);
  }
  //Otherwise, go through the array and print each char (this will be the answer)
  else{
    while (i >= 0){
      printf("%c", radixRepresentation[i]); fflush(stdout);
      i--;
    }
  }
}
