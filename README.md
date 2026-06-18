# GRADE_CALCULATOR.C


#include <stdio.h>


float getScore(char scoreType[]) {
    float score;
    printf("Enter %s score: ", scoreType);
    scanf("%f", &score);
    return score;
}


float calculateFinalGrade(float quizScore, float examScore) {
    return (quizScore * 0.4) + (examScore * 0.6);
}


char getLetterGrade(float finalGrade) {
    if (finalGrade >= 90)
        return 'A';
    else if (finalGrade >= 80)
        return 'B';
    else if (finalGrade >= 70)
        return 'C';
    else if (finalGrade >= 60)
        return 'D';
    return 'F';
}
