# Sticks-Sticks
#include <stdio.h>
#include <stdlib.h>
#include <conio.h>


int main()
{
float h=0;//высота. 
float w=0;//ширина(ввод)
float d=0;//глубина(ввод)
float a=1.5;//толщина дсп
float b=0.5;//толщина двп
float c=1;//толщина дерева
float f1=0.8;//г/см^3 это плотность дсп
float f2=0.82;//г/см ^3 это плотность двп
float f3=0.52;//г/см^3 это плотность дерева(сосна)
float m1=0;// масса нижних и верхних планок. считаются без вычитаний и удваиваются.дсп
float m2=0;//масса боковых стенок. из высоты вычитается ширина верхней и нижней планок.дсп
float m3=0;//масса задней планки.1.5см -  это нижняя планка, она автоматом должна плюсоваться. двп
float m4=0;//дсп масса полок умноженный на их кол-во.
int k=0;//кол-во полок. из полученного кол ва убирается верхняя планка.
int l=40;//расстояние между полками
float m5=0;//дерево масса дверей, c учетом, что они не везутся по полу во время открывания, т.е. их высота равна высота минус ширина нижней планки. удвоенная.
float FINM=0;//финальный вес шкафа.

printf("You are welcomed by Skilful Hands. Create your closet as you see fit.\nEnter the desired width(80-120 cm) and depth(50-90 cm) of your closet so that we can calculate its weight. Ask why? Of course, so you know how many movers to call for pickup.\n");
system("pause");
printf("width, depth\n");
scanf("%f%f",&w,&d);
if ((w>=80 && w<=120) && (d>=50 && d<=90)) 
{h=h+a;
{do
    { h=h+a+l;
    k=k+1;}
while (h<=220-40);}
k=k-1;
 m1=w*d*a*2*f1;
 m2=(h-a-a)*d*a*f1*2;
 m3=h*w*b*f2;
 m4=f1*(w-a-a)*d*k*a;
 m5=f3*(h-a)*w*c;
 FINM=(m1+m2+m3+m4+m5)/1000;
 printf("\n %f kg", FINM);
}
else
{
if (w>120 || w<80) {
printf("width entered incorrectly\n");}
if (d<50 || d>90){ 
printf("depth entered incorrectly\n");}
}
return 0;
}
