# QUIZ-GAME
This Quiz Game in C is a simple interactive program that asks multiple-choice questions and checks the user’s answers. It keeps track of the score and displays the final result at the end. The game is easy to run, beginner-friendly, and demonstrates basic C concepts like input, conditions, and scoring logic.
Quiz Game in C
A simple and interactive quiz game written in C programming language. It asks multiple-choice questions, checks user answers, and displays the final score. This project is perfect for beginners and B.Tech students who want to understand basic C concepts clearly.

 Unique Points
This Quiz Game stands out for its clean and beginner-friendly C code, making it easy for students to understand and modify. It runs on any system without extra libraries and applies core concepts like input handling, conditions, and scoring. Its simplicity makes it ideal for learning and showcasing on GitHub.

 Features

Multiple-choice questions
Score calculation
Simple and clean console interface
Beginner-friendly logic

 Technologies Used

C Programming Language
Standard I/O Library (stdio.h)
 Project Structure
Quiz-Game/
│── quiz.c
│── README.md

 How to Run
Install a C compiler (GCC/MinGW/CodeBlocks).
Open terminal or command prompt in the project folder.
Compile the code:

gcc quiz.c -o quiz
Run the program:
./quiz
📝 Description
This Quiz Game is a simple command-line program that asks a set of multiple-choice questions. The user inputs answers, the program checks correctness, updates the score, and displays the final results. It demonstrates key C concepts such as variables, conditional statements, user input, and logical flow.
#include <stdio.h>

int main() {
    int score = 0;
    char ans;

    printf("===== QUIZ GAME =====\n\n");

    printf("1. What is the capital of India?\n");
    printf("A. Delhi\nB. Mumbai\nC. Kolkata\nD. Chennai\n");
    printf("Your answer: ");
    scanf(" %c", &ans);

    if (ans == 'A' || ans == 'a') score++;

    printf("\n2. Who invented C language?\n");
    printf("A. Bill Gates\nB. Dennis Ritchie\nC. James Gosling\nD. Mark Zuckerberg\n");
    printf("Your answer: ");
    scanf(" %c", &ans);

    if (ans == 'B' || ans == 'b') score++;

    printf("\n3. Which data type is used for characters?\n");
    printf("A. int\nB. char\nC. float\nD. double\n");
    printf("Your answer: ");
    scanf(" %c", &ans);

    if (ans == 'B' || ans == 'b') score++;

    printf("\n===== QUIZ OVER =====\n");
    printf("Your Score: %d / 3\n", score);

    return 0;
}
