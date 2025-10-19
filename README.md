#include <stdio.h>
#include <string.h>
#include <ctype.h>

int main(){
    printf("Welcome to MathsQuize BY Aloo Bhujiya!\n");

    int score = 0;
    char userAnswer;

    printf("Question 1: What is the capital of India?\n");
    printf("a) Mumbai\nb) New Delhi\nc) Kolkata\nd) Chennai\n");

    char answer1 = 'b';

    do {
        printf("Enter your option: ");
        scanf(" %c", &userAnswer);
        userAnswer = tolower(userAnswer);
        
        if (userAnswer < 'a' || userAnswer > 'd'){
            printf("Invalid input. Please enter a, b, c or d.\n");
        }
} while (userAnswer < 'a'|| userAnswer > 'd');
        if(userAnswer == answer1) {
            printf("Correct!\n");
            score++;
        } else {
            printf("Wrong! The correct answer is b) New Delhi.\n");
        }
 while(userAnswer != answer1);

    return 0;
}
