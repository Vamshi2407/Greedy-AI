# Greedy-AI

#include <stdio.h>
/* Greedy Algorithm */
int main() 
{
   int Cash_Owed ; // Cash Owed to Bank Customer
   printf ("How much Cash is owed?\n");
   scanf ("%d", &Cash_Owed );
   printf ("Cash owed to Bank Customer is Rs%d\n",Cash_Owed );
   
	int Tens=0, Twenties=0, Fifties=0, Hundreds=0, Two_Hundreds=0, Five_Hundreds=0, Two_Thousands=0;
	while(Cash_Owed >=2000)
	{
	Cash_Owed =Cash_Owed-2000;
	Two_Thousands++;
	}
	while(Cash_Owed >=500)
	{
	Cash_Owed =Cash_Owed-500;
	Five_Hundreds++;
	}
	while(Cash_Owed >=200)
	{
	Cash_Owed =Cash_Owed-200;
	Two_Hundreds++;
	}
	while(Cash_Owed >=100)
	{
	Cash_Owed =Cash_Owed-100;
	Hundreds++;
	}
	while (Cash_Owed >=50)
	{
		Cash_Owed = Cash_Owed -50;
		Fifties ++;
	}
	while(Cash_Owed >=20)
	{
	Cash_Owed =Cash_Owed-20;
	Twenties++;
	}
	while(Cash_Owed >=10)
	{
	Cash_Owed =Cash_Owed-10;
	Tens++;
	}
	if(Cash_Owed==0)
	{
	printf ("Please Give the Bank Customer following Denomination.\n");
	
	printf ("%d Tens\n", Tens);
	printf ("%d Twenties\n", Twenties );
	printf ("%d Fifties\n", Fifties );
	printf ("%d Hundreds\n", Hundreds );
	printf ("%d Two_Hundreds\n", Two_Hundreds );
	printf ("%d Five_Hundreds\n", Five_Hundreds );
	printf ("%d Two_Thousands\n", Two_Thousands );
	} 
	else
	{
	printf("error..!");
	}
	
}
