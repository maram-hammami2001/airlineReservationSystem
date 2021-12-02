# airlineReservationSystem
a computer reservation system 
#include<stdio.h>
#include<windows.h>
#include <stdlib.h>
void color(int t, int f)
{
	HANDLE H = GetStdHandle(STD_OUTPUT_HANDLE);
	SetConsoleTextAttribute(H, f * 16 + t);
}

int main_menu()
{
	
	system("COLOR 0B");


	printf("                          *************************************************************\n");
	printf("                          ***************                                **************\n");
	printf("                          ********                                           **********\n");
	printf("                                  SYSTEME DE GESTION DES COMPAGNIES AERIENNES             \n");
	printf("                          *********                                          *********\n");
	printf("                          **************                                 **************\n");
	printf("                          *************************************************************\n");
	printf("                               ***************        BIENVENUE AU       *************\n");
	printf("                                  **************  MENU PRINCIPALE :> ! ***********\n");

	printf("\n");
	printf("\n");
	printf("\n");

	printf("                                           veuillez choisir une option\n ");
	printf("\n");
	printf("                                      1-VOIR VOL\n");
	printf("\n");
	printf("                                      2-RESERVER UN BILLET");
	printf("\n");
	printf("\n");

	printf("                                      3-VOIR PASSAGER\n");
	printf("\n");
	printf("                                      4-RECHERCHE PASSAGERS \n");
	printf("\n");
	printf("                                      5-BILLET RESERVER \n");
	printf("\n");
	printf("                                      6-ANNULER  VOL \n");
	printf("\n");
	printf("                                      7-ANNULER VOYAGE\n");
	printf("                     --------------------------------------------------------------------------\n");
	printf("\n");
	printf("\n");

	printf("                                                                 ***TAP A ENTER-KEY TO LEAVE !***\n");
	return 0;
	
}
int voir_vol()
{
	printf("\n");
	printf("\n");

	printf("                             |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||\n       ");
	printf("\n");

	printf("                                                VOTRE VOYAGE COMMENCE MAINTENANT\n                   ");
	printf("\n");

	printf("                             |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||\n       ");
	printf("\n");
	printf("\n");

	printf("         DE              A                DEPART               RETOUR                   CLASSE DE CABINE      \n");
	printf("\n");
	printf("\n");

	printf("      TUNISIE         DJERBA             05/12/2021          12/12/2021                 1 ADULTE,ECONOMIQUE    \n");
	printf("      TUNISIE         EGYPT              06/12/2021          13/12/2021                 1 ADULTE,ECONOMIQUE    \n");
	printf("      TUNISIE         FRANCE             07/12/2021          14/12/2021                 1 ADULTE,ECONOMIQUE    \n");
	printf("      TUNISIE         MALTA              08/12/2021          15/12/2021                 1 ADULTE,ECONOMIQUE    \n");
	printf("      TUNISIE         GREECE             10/12/2021          16/12/2021                 1 ADULTE,ECONOMIQUE    \n");
	printf("      TUNISIE         ALGERIE            11/12/2021          17/12/2021                 1 ADULTE,ECONOMIQUE    \n");
	printf("      TUNISIE         MAROC              12/12/2021          18/12/2021                 1 ADULTE,ECONOMIQUE    \n");
	printf("      TUNISIE         LIBIE              13/12/2021          19/12/2021                 1 ADULTE,ECONOMIQUE    \n");
	printf("      TUNISIE         TURQUIE            14/12/2021          20/12/2021                 1 ADULTE,ECONOMIQUE    \n");
	printf("      TUNISIE         ESPAGNE            15/12/2021          21/12/2021                 1 ADULTE,ECONOMIQUE    \n");
	printf("\n");


	return 0;
}

int lol()
{
	printf("hello");
		return 0; 
}


int main()
{
	int choix, R;
	main_menu() ; 
	printf("choisir un sub menu\n");
	scanf_s("%d", &choix);
	system("cls");
	
	switch (choix)
	{
	case 1:
		color(1,0);
	{printf("'veuillez attendez s'il vous plait...");
	voir_vol();
	printf("retour au menu principal tapper R \n");
	scanf_s("%d", &R);
	if(R)
	{
		system("cls");
		main_menu();
	}
	break;
	}
	case 2: 
	 printf("'veuillez attendez s'il vous plait..."); lol(); break;
	

	default: puts("Oups! entrée invalide"); voir_vol();
	}
		return 0;
	




}
