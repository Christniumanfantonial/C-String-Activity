#include <stdio.h>
#include <stdlib.h>


//    Create a Program that takes a strings from the user input and converts a the vowels into Uppercase.
//    + Print the Inputted String
//    + Print the length of the string
//    + Print the number of consonant and vowels
/*<==  ==<<<-*/

int main(){

    char str[255];   
    int  i, vowels, consonantCounter;


   printf("Input a sentence: ");  
   gets(str);                     
   
   
   i = 0;                  
   vowels = 0;              
   consonantCounter = 0; 


    while(str[i]!='\0') 
    {
     if(str[i] == 'a' || str[i] == 'e' || str[i] == 'i' || str[i] == 'o' || str[i] == 'u'){
        str[i]=str[i]-32;
        vowels++;
        }
     if(str[i] >= 'a' || str[i] >= 'e' || str[i] >= 'i' || str[i] >= 'o' || str[i] >= 'u'){
        consonantCounter++;
        }

        i++;
    }
    printf("String converted: ");
    puts(str);
    printf("\n");

    printf("String length: %d \n", i);
    printf("Vowels: %d \n", i-consonantCounter);
    printf("Consonant: %d \n", i-vowels);

return 0;

}
