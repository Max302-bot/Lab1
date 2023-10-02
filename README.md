#include <stdio.h>
#include <stdlib.h>
#include<windows.h>
#include <stdlib.h>

#define Name "Max"
#define LastName "Bilous"
#define GroupName "PC-31"
#define Faculty "RTF"
#define University "Igor Sikorsky KPI"

int main()

{
unsigned int age; // вік
unsigned int semestr; // номер семестру
float admissionScore; //  вступ бал
int grade1; //  предмет №1
int grade2; // предмет №2
int grade3; // предмет №3
double averageGrade; //  середнє значення
SetConsoleCP (1251);
SetConsoleOutputCP(1251);






printf("%s%s Виконайте наступні дії .\n",Name ,LastName);
printf("Введіть намер семестру : ");
scanf("%u", &semestr);

  printf("Введіть свій вступний бал: ");
   scanf("%f", &admissionScore);

  printf("Введіть оцінку за предмет No1: ");
   scanf("%d", &grade1);

  printf("Введіть оцінку за предмет No2: ");
  scanf("%d", &grade2);

  printf("Введіть оцінку за предмет No3: ");
  scanf("%d", &grade3);

  printf("Введіть свій вік: ");
  scanf("%u", &age);
  averageGrade = (double)(grade1 + grade2 + grade3) /3 ; //змінюєм тип данних та рахуєм середній бал

  printf("\n\t average grade = %.3lf", averageGrade);


  averageGrade = (double)(grade1 + grade2 + grade3) / 3;

system("cls"); // Очистити поле для тексту
printf("%s", University); // Університет в якому навчається студент
printf("\n%s", Faculty); // Факульет в якому навчається студент
printf("\n%s", GroupName); // Група студента
printf("\n>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>");
printf("\nstudent: %s %s", Name, LastName ); //Ім'я та прізвище студента
printf("\nage: %u", age);// Вік студента
printf("\nsemestr: %u", semestr); //Номер семемтру
printf("\n>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>");
printf("\nadmission score: %.2f", admissionScore); //Вступний бал
printf("\naverage grade = %.3lf", averageGrade); // Середній бал по трьом предметам
printf("\n");// Відступ рядка

    return 0 ;
}

