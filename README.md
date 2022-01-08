#include<windows.h>
#include<stdio.h>
#include<stdlib.h>
#include<string.h>
#include<string>
#include<conio.h>
#include<ctype.h>
struct passager {
	char name[100];  //nom de passager
	char sexe[100]; //son sexe
	int dd, mm, yy;  //sa date de naissance
	char cin[10], code[10]; //son numero de CIN et son code passport
	int vol = 0; //numero de vol            
	int num = 5; //nombre max de passagers;; tabpassager[0].num est utilisé dans le compteur à l'affichage (le max des passagers)   
};
struct vol {
	int nv; //numero de vol
	char dep[10]; //pays depart
	char ar[20];  //pays d'arrvée/destination
	int  jdep; //jours de depart 
	int mdep;//mois de depart
	int adep; // Année de depart
	int  jar; //jours d'arrivée
	int mar;//mois d'arrivée
	int aar; // Année d'arrivée
	int np;  //nombre de place valable
	int num; //nombre max des vols;; tabvol[1].num est utilisé dans le compteur à l'affichage (le max des vols)
	char a[100] = { "" };
};

void color(int t, int f)
{
	HANDLE H = GetStdHandle(STD_OUTPUT_HANDLE); //fonction predefinie appartenant a la biblio windows.h permettant la modification des couleurs (pris online)
	SetConsoleTextAttribute(H, f * 16 + t);
}

void delay(int a)
{
	int add = 0;
	int time;
	int i;
	time = a * 10000000;
	for (i = 0; i < time; i++)
	{
		add += i;
		add++;
		add++;

	}
}
void anim1()
{
	color(3, 0);                    //START OF SMALL LOGO ANIMATION
	printf("\n**       ");
	printf("\n* ****** ");
	printf("\n*       *");
	printf("\n******** ");
	printf("\n   * *   ");
	printf("\n   **    ");
	delay(10);
	system("cls");
	color(4, 0);
	printf("\n  **       ");
	printf("\n  * ****** ");
	printf("\n  *       *");
	printf("\n  ******** ");
	printf("\n     * *   ");
	printf("\n     **    ");
	delay(10);

	system("cls");
	color(6, 0);
	printf("\n    **       ");
	printf("\n    * ****** ");
	printf("\n    *       *");
	printf("\n    ******** ");
	printf("\n       * *   ");
	printf("\n       **    ");
	delay(10);
	system("cls");
	color(7, 0);
	printf("\n      **       ");
	printf("\n      * ****** ");
	printf("\n      *       *");
	printf("\n      ******** ");
	printf("\n         * *   ");
	printf("\n         **    ");
	delay(10);
	system("cls");
	color(8, 0);
	printf("\n        **       ");
	printf("\n        * ****** ");
	printf("\n        *       *");
	printf("\n        ******** ");
	printf("\n           * *   ");
	printf("\n           **    ");
	delay(10);
	system("cls");
	color(9, 0);
	printf("\n          **       ");
	printf("\n          * ****** ");
	printf("\n          *       *");
	printf("\n          ******** ");
	printf("\n             * *   ");
	printf("\n             **    ");
	delay(10);
	system("cls");
	color(10, 0);
	printf("\n            **       ");
	printf("\n            * ****** ");
	printf("\n            *       *");
	printf("\n            ******** ");
	printf("\n               * *   ");
	printf("\n               **    ");
	delay(10);
	system("cls");
	color(11, 0);
	printf("\n              **       ");
	printf("\n              * ****** ");
	printf("\n              *       *");
	printf("\n              ******** ");
	printf("\n                 * *   ");
	printf("\n                 **    ");
	delay(10);
	system("cls");
	color(12, 0);
	printf("\n                **       ");
	printf("\n                * ****** ");
	printf("\n                *       *");
	printf("\n                ******** ");
	printf("\n                   * *   ");
	printf("\n                   **    ");
	delay(10);
	system("cls");
	color(13, 0);
	printf("\n                  **       ");
	printf("\n                  * ****** ");
	printf("\n                  *       *");
	printf("\n                  ******** ");
	printf("\n                     * *   ");
	printf("\n                     **    ");
	delay(10);
	system("cls");
	color(14, 0);
	printf("\n                    **       ");
	printf("\n                    * ****** ");
	printf("\n                    *       *");
	printf("\n                    ******** ");
	printf("\n                       * *   ");
	printf("\n                       **    ");
	delay(10);
	system("cls");
	color(5, 0);
	printf("\n                      **       ");
	printf("\n                      * ****** ");
	printf("\n                      *       *");
	printf("\n                      ******** ");
	printf("\n                         * *   ");
	printf("\n                         **    ");
	delay(10);
	system("cls");
	color(3, 0);
	printf("\n                        **       ");
	printf("\n                        * ****** ");
	printf("\n                        *       *");
	printf("\n                        ******** ");
	printf("\n                           * *   ");
	printf("\n                           **    ");
	delay(10);
	system("cls");
	color(3, 0);
	printf("\n                          **       ");
	printf("\n                          * ****** ");
	printf("\n                          *       *");
	printf("\n                          ******** ");
	printf("\n                             * *   ");
	printf("\n                             **    ");
	delay(10);
	system("cls");
	printf("\n                            **       ");
	printf("\n                            * ****** ");
	printf("\n                            *       *");
	printf("\n                            ******** ");
	printf("\n                               * *   ");
	printf("\n                               **    ");
	delay(10);
	system("cls");
	printf("\n                              **       ");
	printf("\n                              * ****** ");
	printf("\n                              *       *");
	printf("\n                              ******** ");
	printf("\n                                 * *   ");
	printf("\n                                 **    ");
	delay(10);
	system("cls");
	printf("\n                               **       ");
	printf("\n                               * ****** ");
	printf("\n                               *       *");
	printf("\n                               ******** ");
	printf("\n                                  * *   ");
	printf("\n                                  **    ");
	delay(10);
	system("cls");
	printf("\n                                 **       ");
	printf("\n                                 * ****** ");
	printf("\n                                 *       *");
	printf("\n                                 ******** ");
	printf("\n                                    * *   ");
	printf("\n                                    **    ");
	delay(10);
	system("cls");
	printf("\n                                   **       ");
	printf("\n                                   * ****** ");
	printf("\n                                   *       *");
	printf("\n                                   ******** ");
	printf("\n                                      * *   ");
	printf("\n                                      **    ");
	delay(10);
	color(3, 0);
	system("cls");
	printf("\n                                     **       ");
	printf("\n                                     * ****** ");
	printf("\n                                     *       *");
	printf("\n                                     ******** ");
	printf("\n                                        * *   ");
	printf("\n                                        **    ");
	delay(10);
	system("cls");

}                                  //END OF SMALL LOGO ANIMATION
void logo1anim()
{                                  //START OF BIG LOGO ANIMATION (DELAY)
	color(1, 0);
	printf("\n      *******                                                      "); delay(30);
	color(2, 0);
	printf("\n       *      *                                                    "); delay(10);
	color(3, 0);
	printf("\n        *       *                                                  "); delay(10);
	color(4, 0);
	printf("\n      ***        ******************************************        "); delay(20);
	color(5, 0);
	printf("\n       *         A                          A    I RRRR   *****    "); delay(10);

	color(6, 0);
	printf("\n        *       A A  v   v i  aaa   n      A A   I R   R  ******   "); delay(10);
	color(7, 0);
	printf("\n         *     AAAAA  v v  i a   a  nnnn  AAAAA  I RRRR         *  "); delay(20);
	color(8, 0);
	printf("\n          *   A     A  v   i  aaaaa n  n A     A I R   R        *  "); delay(10);
	printf("\n           *****      *************           *****************    "); delay(20);
	color(9, 0);
	printf("\n              *      *           *          *                      "); delay(20);
	printf("\n             *     *            *         *                        "); delay(15);
	color(10, 0);
	printf("\n            *******            *        *                          "); delay(10);
	printf("\n                              *       *                            "); delay(17);
	color(11, 0);
	printf("\n                             *      *                              "); delay(20);
	printf("\n                            *******                                "); delay(30);

}                                  //END OF BIG LOGO ANIMATION (DELAY)

							   //END OF PRINTING BIG LOGO

void logo2()
{		 //START OF SECOND LOGO
	printf("\n                                                                                  |              ");
	printf("\n                                                                    \\____TUNISFAX_(_)_AIR______/ ");
	printf("\n                                                                               o'   'o           ");
	printf("\n");
	printf("\n\n                                           ");

	printf("\n\n                         << NOUS REND LE CIEL PLUS PETIT QUE LA TERRE >>                    ");
	delay(100);
	printf("\ :)");
	color(8, 0);
	printf("\n");
	printf("\n");

	printf("\n");

	printf("                                   ------------------------------------ Veuillez appuyer sur entrer pour continuer :> !-----------------------------------\n");
	getchar();
}
void bienvenue() {
	int getchar(); color(13, 0);
	delay(20);
	puts(" ");
	puts(" ");
	delay(30);
	puts(" ");
	printf("                   bbbbbbbb                                                                                                                                                              \n");
	printf("                   b::::::b              iiii                                                                                                                                        !!!\n");
	printf("                   b::::::b             i::::i                                                                                                                                      !!:!!\n");
	delay(35);
	printf("                   b::::::b              iiii                                                                                                                                       !:::!\n");
	printf("                   b:::::b                                                                                                                                                         !:::!\n");
	printf("                   b:::::bbbbbbbbb    iiiiiii     eeeeeeeeeeee    nnnn  nnnnnnnn vvvvvvv           vvvvvvv eeeeeeeeeeee    nnnn  nnnnnnnn    uuuuuu    uuuuuu      eeeeeeeeeeee    !:::!\n");
	delay(45);
	printf("                   b::::::::::::::bb  i:::::i   ee::::::::::::ee  n:::nn::::::::nnv:::::v         v:::::vee::::::::::::ee  n:::nn::::::::nn  u::::u    u::::u    ee::::::::::::ee  !:::!\n");
	printf("                   b::::::::::::::::b  i::::i  e::::::eeeee:::::een::::::::::::::nnv:::::v       v:::::ve::::::eeeee:::::een::::::::::::::nn u::::u    u::::u   e::::::eeeee:::::ee!:::!\n");
	printf("                   b:::::bbbbb:::::::b i::::i e::::::e     e:::::enn:::::::::::::::nv:::::v     v:::::ve::::::e     e:::::enn:::::::::::::::nu::::u    u::::u  e::::::e     e:::::e!:::!\n");
	delay(40);
	printf("                   b:::::b    b::::::b i::::i e:::::::eeeee::::::e  n:::::nnnn:::::n v:::::v   v:::::v e:::::::eeeee::::::e  n:::::nnnn:::::nu::::u    u::::u  e:::::::eeeee::::::e!:::!\n");
	printf("                   b :::::b     b:::::b i::::i e:::::::::::::::::e   n::::n    n::::n  v:::::v v:::::v  e:::::::::::::::::e   n::::n    n::::nu::::u    u::::u  e:::::::::::::::::e !:::!\n");
	delay(30);
	printf("                   b:::::b     b:::::b i::::i e::::::eeeeeeeeeee    n::::n    n::::n   v:::::v:::::v   e::::::eeeeeeeeeee    n::::n    n::::nu::::u    u::::u  e::::::eeeeeeeeeee  !!:!!\n");
	printf("                   b:::::b     b:::::b i::::i e:::::::e             n::::n    n::::n    v:::::::::v    e:::::::e             n::::n    n::::nu:::::uuuu:::::u  e:::::::e            !!! \n");
	printf("                   b:::::bbbbbb::::::bi::::::ie::::::::e            n::::n    n::::n     v:::::::v     e::::::::e            n::::n    n::::nu:::::::::::::::uue::::::::e               \n");
	delay(35);
	printf("                   b::::::::::::::::b i::::::i e::::::::eeeeeeee    n::::n    n::::n      v:::::v       e::::::::eeeeeeee    n::::n    n::::n u:::::::::::::::u e::::::::eeeeeeee   !!! \n");
	printf("                   b:::::::::::::::b  i::::::i  ee:::::::::::::e    n::::n    n::::n       v:::v         ee:::::::::::::e    n::::n    n::::n  uu::::::::uu:::u  ee:::::::::::::e  !!:!!\n");
	delay(30);
	printf("                   bbbbbbbbbbbbbbbb   iiiiiiii    eeeeeeeeeeeeee    nnnnnn    nnnnnn        vvv            eeeeeeeeeeeeee    nnnnnn    nnnnnn    uuuuuuuu  uuuu    eeeeeeeeeeeeee   !!! \n");

}
//affichage de la liste de vol non valables/annulés
int affiche1nval(struct passager tabpassager[10], struct vol tabvol[10])

{
	int mainmenu(struct passager tabpassager[10], struct vol tabvol[10]);
	int option1(struct passager tabpassager[10], struct vol tabvol[10]);
	int rep, i;
	system("cls");
	color(9, 0);

	system("cls");
	puts("            |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||");
	puts("            ||||||||||||||||||||||||||||||||||||||||||||                                                                              |||||||||||||||||||||||||||||||||||");
	puts("            |||||||||||||||||||||||||||||||||                                                                                              ||||||||||||||||||||||||||||||");
	puts("            ||||||||||||||||||||||||||||                                                                                                             ||||||||||||||||||||");
	puts("            ||||||||||||||||||||||                                  * * * *   L I S T E    D E S    V O L S * * * *                                      ||||||||||||||||");
	puts("            |||||||||||||||||||||||                                                                                                                    ||||||||||||||||||");
	puts("            |||||||||||||||||||||||||                                            N O N     V A L A B L E S                                           ||||||||||||||||||||");
	puts("            |||||||||||||||||||||||||||||||||                                                                                              ||||||||||||||||||||||||||||||");
	puts("            |||||||||||||||||||||||||||||||||||||||||||                                                                               |||||||||||||||||||||||||||||||||||");
	puts("            |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||");
	printf("\n");
	printf("\n");
	color(15, 0);
	printf("              NUMERO DE VOL        DE                                  A              DATE DEPART            DATE DE RETOUR             Nombre de place valable                      \n");
	printf("\n");
	printf("\n");
	color(4, 0);
	for (i = 1; i < tabvol[1].num + 1; i++)
	{
		if (strcmp(tabvol[i].a, "ANNULER") == 0)
		{
			printf("              %d    \t ", tabvol[i].nv);
			printf("        %s\t", tabvol[i].dep);
			printf("             %s\t", tabvol[i].ar);
			printf("              %d/", tabvol[i].jdep);
			printf("%d/", tabvol[i].mdep);
			printf("%d     \t", tabvol[i].adep);
			printf("            %d/", tabvol[i].jar);
			printf("%d/", tabvol[i].mar);
			printf("%d\t", tabvol[i].aar);
			printf("             %d  ", tabvol[i].np);
			printf("%s", tabvol[i].a);
			printf(" \n");
		}
	}
	printf("                                                                             -----------------------------------------------\n");

	printf("                                                                                  voulez vous retourner au menu precedent? ");
	printf(" \n");
	printf("                                                                        *veuillez entrer 1 pour retourner au menu precedent ou bien tapper 2 pour retourner au menu principal*");
	scanf_s("%d", &rep);
	if (rep == 1)
	{
		system("cls");
		option1(tabpassager, tabvol);
	}
	else if (rep == 2)
	{
		system("cls");
		mainmenu(tabpassager, tabvol);
	}

	return 0;

}
//verification de la date de depart et d'arrivée
int verifdate2(int jj, int mm, int aa)
{

	//verifions l'annee
	if (aa == 2022)
	{
		//verifions le mois 
		if (mm >= 1 && mm <= 12)
		{
			//verifions le jour
			if ((jj >= 1 && jj <= 31) && (mm == 1 || mm == 3 || mm == 5 || mm == 7 || mm == 8 || mm == 10 || mm == 12))
			{
				printf("date valide :} \n");
				return 1;
			}
			else if ((jj >= 1 && jj <= 30) && (mm == 4 || mm == 6 || mm == 9 || mm == 11))
			{
				printf("date valide :} \n"); return 1;
			}
			else if ((jj >= 1 && jj <= 28) && (mm == 2))
			{
				printf("date valide :}  \n");
				return 1;
			}
			else
			{
				printf("Le Jour est invalide. :< \n"); return 0;
			}
		}
		else
		{
			printf("le Mois est invalide :< \n"); return 0;
		}
	}
	else
	{
		printf("l'annee est invalide :< \n");

	}

	return 0;
}
//fonction d'ajout de vol 
int ajoutvol(struct passager tabpassager[10], struct vol tabvol[10])
{
	int affiche1(struct passager tabpassager[10], struct vol tabvol[10]);
	int test, i, d, m, y;
	int n;
	printf("bienvenue\t");
	do
	{
		printf("combient de vol voulez vous ajouter (3 max)");
		scanf_s("%d", &n);
	} while (n > 3);
	for (i = tabvol[1].num + 1; i <= (tabvol[1].num) + n; i++)
	{
		getchar();
		//tunisie par default
		strcpy_s(tabvol[i].dep, "tunisie");

		do

		{

			printf(" le pays de depart est %s veuillez donner le pays d'arrivee \n", tabvol[i].dep);
			gets_s(tabvol[i].ar);
			test = atoi(tabvol[i].ar); // atoi retourne 0 si la chaine et alphabetique/alphanumerique et retourne la valeur si la chaine est numerisque :}
		} while ((test != 0) && (strlen(tabvol[i].ar) < 1));

		do
		{
			printf("donner le jours de depart ");
			scanf_s("%d", &tabvol[i].jdep);
			printf("donner le mois de depart ");
			scanf_s("%d", &tabvol[i].mdep);
			printf("donner l'annee de depart ( doit etre 2022) ");
			scanf_s("%d", &tabvol[i].adep);



		} while (verifdate2(tabvol[i].jdep, tabvol[i].mdep, tabvol[i].adep) == 0);
		do
		{

			//verification si le mois de depart est inferieur au moins d'arrivée 
			do
			{
				printf("donner le mois d'arrivee (doit etres superieur ou egale au moins de depart) ");
				scanf_s("%d", &tabvol[i].mar);
			} while (tabvol[i].mar < tabvol[i].mdep);
			//verification si le mois de depart est egale au moins d'arrivee donc le jours de depart doit etre inferieur au jours d'arrivée
			if (tabvol[i].mar == tabvol[i].mdep)
			{
				do
				{
					printf("donner le jours d'arrivee (doit etre superieur au jours de depart )  ");
					scanf_s("%d", &tabvol[i].jar);
				} while (tabvol[i].jar <= tabvol[i].jdep);

			}
			else
			{
				printf("donner le jours d'arrivee  ");
				scanf_s("%d", &tabvol[i].jar);
			}
			printf("donner l'annee d'arrivee ");
			scanf_s("%d", &tabvol[i].aar);



		} while (verifdate2(tabvol[i].jar, tabvol[i].mar, tabvol[i].aar) == 0);

		do
		{
			printf("donner le nombre de place (entre 1 et 120)");
			scanf_s("%d", &tabvol[i].np);
		} while (tabvol[i].np < 0 || tabvol[i].np>120);
		printf("le %d vol est ajoutee avec succes\n", tabvol[i].nv);
		tabvol[i].nv = i;
	}
	tabvol[1].num += n;

	affiche1(tabpassager, tabvol);

	return 0;

}
//gestionnaire de vols
int option1(struct passager tabpassager[10], struct vol tabvol[10])
{
	int c;
	//des prototypes
	int affiche1(struct passager tabpassager[10], struct vol tabvol[10]);
	int mainmenu(struct passager tabpassager[10], struct vol tabvol[10]);
	int annuler(struct passager tabpassager[10], struct vol tabvol[10]);
	system("cls");

	color(9, 0);

	puts("  ");
	puts("  ");
	puts("  ");
	puts("=================================================  G  E  S  T  I  O  N  N  A  I  R  E        D  E      V  O  L  S  ! ============================================================================");
	color(2, 0);
	printf("                                       =                                                                                         =\n");
	printf("                                       =                                                                                         =\n");
	printf("                                       =                                                                                         =\n");
	printf("                                       =   V E U I L L E Z    C H O I S I R   U N E   O P T I O N :                              =\n");
	printf("                                       =                                                                                         =\n");
	printf("                                       =                                                                                         =\n");
	printf("                                       =                                                                                         =\n");
	printf("                                       =        1)AFFICHER LA LISTE DES VOLS                                                     =\n");
	printf("                                       =                                                                                         =\n");
	printf("                                       =                                                                                         =\n");
	printf("                                       =        2)AFFICHER LA LISTE DES VOLS NON VALABLES                                        =\n");
	printf("                                       =                                                                                         =\n");
	printf("                                       =                                                                                         =\n");
	printf("                                       =        3)AJOUTER UN VOL                                                                 =\n");
	printf("                                       =                                                                                         =\n");
	printf("                                       =                                                                                         =\n");
	printf("                                       =        4)ANNULER UN VOL                                                                 =\n");//LA LISTE DES VOLS VALABLES ET NON VALABLES 
	printf("                                       =                                                                                         =\n");
	printf("                                       =                                                                                         =\n");
	printf("                                       =        5)RETOUR AU MENU PRINCIPAL                                                       =\n");
	printf("                                       =                                                                                         =\n");
	printf("                                       =                                                                                         =\n");
	printf("                                       ===========================================================================================\n");
	printf(" \n");
	color(6, 0);
	printf("                                                                      Veuillez donner votre choix ===> \t");
	scanf_s("%d", &c);
	switch (c) {
	case 1:
		affiche1(tabpassager, tabvol);
		break;
	case 2:
		affiche1nval(tabpassager, tabvol);
		break;
	case 3:
		ajoutvol(tabpassager, tabvol); ;
		break;
	case 4:
		annuler(tabpassager, tabvol);
	case 5:

		system("cls");
		mainmenu(tabpassager, tabvol);
		break;


	}
	return 0;
}
//affichage de la liste des vols
int affiche1(struct passager tabpassager[10], struct vol tabvol[10])
{
	int option1(struct passager tabpassager[10], struct vol tabvol[10]);
	int mainmenu(struct passager tabpassager[10], struct vol tabvol[10]);
	int i;
	int rep;
	color(9, 0);

	system("cls");
	puts("            |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||");
	puts("            ||||||||||||||||||||||||||||||||||||||||||||                                                                              |||||||||||||||||||||||||||||||||||");
	puts("            |||||||||||||||||||||||||||||||||                                                                                              ||||||||||||||||||||||||||||||");
	puts("            ||||||||||||||||||||||||||||                                                                                                             ||||||||||||||||||||");
	puts("            ||||||||||||||||||||||                                  * * * *   L I S T E    D E S    V O L S* * * *                                     ||||||||||||||||");
	puts("            |||||||||||||||||||||||||                                                                                                                ||||||||||||||||||||");
	puts("            |||||||||||||||||||||||||||||||||                                                                                              ||||||||||||||||||||||||||||||");
	puts("            |||||||||||||||||||||||||||||||||||||||||||                                                                               |||||||||||||||||||||||||||||||||||");
	puts("            |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||");
	printf("\n");
	color(15, 0);

	printf("              NUMERO DE VOL        DE                                  A              DATE DEPART            DATE DE RETOUR             Nombre de place valable                      \n");
	printf("\n");
	color(5, 0);

	printf("\n");
	for (i = 1; i < tabvol[1].num + 1; i++)
	{
		printf("\n");
		printf("\n");

		printf("              %d    \t ", tabvol[i].nv);
		printf("        %s\t", tabvol[i].dep);
		printf("             %s\t", tabvol[i].ar);
		printf("              %d/", tabvol[i].jdep);
		printf("%d/", tabvol[i].mdep);
		printf("%d     \t", tabvol[i].adep);
		printf("            %d/", tabvol[i].jar);
		printf("%d/", tabvol[i].mar);
		printf("%d\t", tabvol[i].aar);
		printf("             %d  ", tabvol[i].np);
		printf("%s", tabvol[i].a);
		printf(" \n");

	}
	printf("\n");

	printf("\n");

	printf("                                                                             -----------------------------------------------\n");

	printf("                                                                                  voulez vous retourner au menu precedent? ");
	printf(" \n");
	printf("                                                                        *veuillez entrer 1 pour retourner au menu precedent ou bien tapper 2 pour retourner au menu principal*");
	scanf_s("%d", &rep);
	if (rep == 1)
	{
		system("cls");
		option1(tabpassager, tabvol);
	}
	else if (rep == 2)
	{
		system("cls");
		mainmenu(tabpassager, tabvol);
	}

	return 0;

}
//fonction d'annulation de vol
int annuler(struct passager tabpassager[10], struct vol tabvol[10])
{
	int i, choix, c, option1(struct passager tabpassager[10], struct vol tabvol[10]);
	int affiche1(struct passager tabpassager[10], struct vol tabvol[10]);
	system("cls");

	printf("=============================================================  A  N  N  U  L  A  T  I  O  N       D  E  S       V  O  L  S ! ============================================================================");

	printf("                                                                                        \n");

	printf("                                                                                        X\n");
	printf("                                                                                        X\n");
	printf("                                                                                        X\n");
	printf("                                                                                        X\n");
	printf("                                                                                        X\n");
	printf("                                                                                        X\n");
	printf("                                                                                        X\n");
	printf("                                                                                        X\n");
	printf("                                                                                        X\n");
	printf("                                                                                        X\n");

	printf("                                                          QUELLE EST LE VOL QUE VOUS VOULEZ ANNULER ?");
	puts("");
	puts("");
	printf("              NUMERO DE VOL        DE                                      A              DATE DEPART            DATE DE RETOUR             Nombre de place valable            \n");
	printf("\n");
	printf("\n");
	for (i = 1; i < tabvol[1].num + 1; i++)
	{

		printf("              %d    \t ", tabvol[i].nv);
		printf("        %s\t", tabvol[i].dep);
		printf("                   %s\t", tabvol[i].ar);
		printf("              %d/", tabvol[i].jdep);
		printf("%d/", tabvol[i].mdep);
		printf("%d     \t", tabvol[i].adep);
		printf("            %d/", tabvol[i].jar);
		printf("%d/", tabvol[i].mar);
		printf("%d\t", tabvol[i].aar);
		printf("             %d  ", tabvol[i].np);
		printf(" \n");
	}


	printf("donner le numero de vol que vous voulez annuler");
	scanf_s("%d", &choix);



	system("cls");
	if ((tabvol[choix].nv) && (strcmp(tabvol[choix].a, "")) != 0)
	{
		printf("le vol numero %d est deja annulee", choix);

	}
	else
		if (choix<1 || choix >tabvol[1].num)
		{
			printf("vol numero %d n'existe pas", choix);
		}
		else
		{
			system("cls");


			printf("                                                                      !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!\n");
			printf("                                                                      !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!\n");
			printf("      !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!   A   T   T   E   N   T   I   O   N   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!\n ");
			printf("                                                                      !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!\n");
			printf("                                                                      !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!\n");
			printf("                                                                                            . \n");
			printf("                                                                                            .\n");
			printf("                                                                                            .\n");
			printf("                                                                                            .\n");
			printf("                                                                                            .\n");
			printf("                                                                                            .\n");
			printf("                                                                                            .\n");
			printf("    \n");
			printf("    \n");

			printf("                                                                   VOULEZ VOUS VRAIMENT ANNULER LE VOL NUMERO   %d ? ", choix);
			printf("    \n");
			printf("    \n");

			printf("                                                                                  1 pour oui / 0 pour retourner au menu precedent            ");
			scanf_s("%d", &c);
			if (c == 1)
			{
				strcpy_s(tabvol[choix].a, "ANNULER");

				affiche1(tabpassager, tabvol);
			}
			else
			{
				option1(tabpassager, tabvol);
			}
		}


	return 0;
}



//fonction de confirmation de réservation
void confirmer(char nom[100], int dd, int mm, int  yy, char sexe[100], char cin[100], char code[10], struct passager tabpassager[10], struct vol tabvol[10], int numvol) {
	void retour1(struct passager tabpassager[10], struct vol tabvol[10]);


	int c, n = 0;
	system("cls");
	printf("                 |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||\n");
	printf("\t\t\t           ||||                     veuillez confirmer la reservation?                              ||||\n ");
	printf("\t\t\t           ||||                 1)oui, confirmer                                                    ||||\n");
	printf("\t\t\t           ||||                 2)non, annuler                                                      ||||\n");
	printf("\t\t\t           |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||\n");
	printf("========>votre choix : ");
	scanf_s("%d", &c);
	switch (c) {
	case 1: //en confirmant, les données sont conservées
		tabpassager[0].num += 1; //le max des passagers +1
		strcpy_s(tabpassager[tabpassager[0].num].name, nom);
		tabpassager[tabpassager[0].num].dd = dd;
		tabpassager[tabpassager[0].num].mm = mm;
		tabpassager[tabpassager[0].num].yy = yy;
		strcpy_s(tabpassager[tabpassager[0].num].sexe, (sexe));
		strcpy_s(tabpassager[tabpassager[0].num].cin, cin);
		strcpy_s(tabpassager[tabpassager[0].num].code, code);
		tabpassager[tabpassager[0].num].vol = numvol;
		tabvol[numvol].np--;	//nombre de place valable -1 




		printf("\n");
		printf("\n");
		printf("            ==============================================================================================================================================\n");
		printf("            =                                       Votre Reservation est realisee avec succes!                                                          =\n ");
		printf("            ==============================================================================================================================================\n");
		printf("\n");
		printf("\n");
		retour1(tabpassager, tabvol);

		break;

	case 2:  system("cls"); retour1(tabpassager, tabvol); break;
	default: system("cls"); confirmer(nom, dd, mm, yy, sexe, cin, code, tabpassager, tabvol, numvol); break;

	}


}
//affichage d'un menu de retour (au menu de gestionnaire de passagers ou mainmenu)
void retour2(struct passager tabpassager[10], struct vol tabvol[10]) {
	int option2(struct passager tabpassager[10], struct vol tabvol[10]);
	int mainmenu(struct passager tabpassager[10], struct vol tabvol[10]);
	int c;
	puts("");
	puts("");
	puts("");
	color(7, 0);

	puts("                |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||");
	puts("                ||||||||||||||||||||||||||||||||||||||||||||                                                                              |||||||||||||||||||||||||||||||||||");
	puts("                |||||||||||||||||||||||||||||||||                       VEUILLEZ RETOURNER AU                                                  ||||||||||||||||||||||||||||||");
	puts("                ||||||||||||||||||||||||||||                                                                                                             ||||||||||||||||||||");
	puts("                ||||||||||||||||||||||                                1) MENU PRECEDENT                                                                      ||||||||||||||||");
	puts("                |||||||||||||||||||||||||                                                                                                                ||||||||||||||||||||");
	puts("                |||||||||||||||||||||||||||||||||                     2) MENU PRINCIPAL                                                        ||||||||||||||||||||||||||||||");
	puts("                |||||||||||||||||||||||||||||||||||||||||||                                                                               |||||||||||||||||||||||||||||||||||");
	puts("                |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||");
	color(15, 0);


	printf("                          ========>votre choix : ");
	scanf_s("%d", &c);
	switch (c) {
	case 1: system("cls"); option2(tabpassager, tabvol); break;
	case 2: system("cls"); mainmenu(tabpassager, tabvol); break;
	default:getchar(); system("cls"); retour2(tabpassager, tabvol); break;
	}


}

//affichage de la liste des passagers
int affichepassager(struct passager tabpassager[10], struct vol tabvol[10]) {
	void retour1(struct passager tabpassager[10], struct vol tabvol[10]);
	int i = 0;
	color(9, 0);

	puts("            |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||");
	puts("            ||||||||||||||||||||||||||||||||||||||||||||                                                                              |||||||||||||||||||||||||||||||||||");
	puts("            |||||||||||||||||||||||||||||||||                                                                                              ||||||||||||||||||||||||||||||");
	puts("            ||||||||||||||||||||||||||||                                                                                                             ||||||||||||||||||||");
	puts("            ||||||||||||||||||||||                                  * * * *   L I S T E    D E S    PASSAGERS* * * *                                     ||||||||||||||||");
	puts("            |||||||||||||||||||||||||                                                                                                                ||||||||||||||||||||");
	puts("            |||||||||||||||||||||||||||||||||                                                                                              ||||||||||||||||||||||||||||||");
	puts("            |||||||||||||||||||||||||||||||||||||||||||                                                                               |||||||||||||||||||||||||||||||||||");
	puts("            |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||");
	printf("\n");
	printf("\n");
	color(15, 0);
	printf("                             NUMERO DE VOL          NOM ET PRENON            GENRE         DATE DE NAISSANCE         CIN             CODE    ");
	printf("\n");
	printf("\n");
	printf("\n");
	printf("\n");
	color(5, 0);

	for (i = 1; i <= tabpassager[0].num; i++)
	{
		printf("\n");

		printf("      passager numero =>%d   \t", i);
		printf(" vol : %i       \t", tabpassager[i].vol);

		printf("  %s\t         ", tabpassager[i].name);

		printf(" \t%s   \t", tabpassager[i].sexe);

		printf("  %d/%d/%d\t         ", tabpassager[i].dd, tabpassager[i].mm, tabpassager[i].yy);

		printf(" %s\t    ", tabpassager[i].cin);
		printf(" %s\n  ", tabpassager[i].code);
	}
	retour2(tabpassager, tabvol);

	return 0;

}
//fonction de recherche selon la premiere lettre du nom
void searchLettre(struct passager tabpassager[10], struct vol tabvol[10]) {
	void retour2(passager tabpassager[10], vol tabvol[10]);
	int i, cond1 = 0, cond2 = 0;
	char choix[100]; char test[100];
	getchar();
	puts("");
	printf("                        Veuillez donner Une lettre ===>\t");

	do {
		cond2 = 0;
		gets_s(choix);
		if (choix[0] >= 'a' && choix[0] <= 'z')choix[0] = choix[0] - 32; //convertion du miniscule au majuscule par code ascii
		for (i = 1; i <= tabpassager[0].num; i++) {
			strncpy_s(test, tabpassager[i].name, 1); //on prend la premiere lettre de chaque case passager pour la copmarer
			if (test[0] >= 'a' && test[0] <= 'z') test[0] = test[0] - 32;

			if (strcmp(choix, test) == 0) {


				printf("\n");
				printf("                         passager numero %d\t", i);
				printf(" vol     \t\t %i \t", tabpassager[i].vol);

				printf("         \t%s\t", tabpassager[i].name);

				printf("         \t\t%s\t", tabpassager[i].sexe);

				printf("  %d %d %d\t  ", tabpassager[i].dd, tabpassager[i].mm, tabpassager[i].yy);

				printf(" %s\t                     ", tabpassager[i].cin);
				printf(" %s\n                     ", tabpassager[i].code);

			}
			else  cond2 += 1;

		}
		if (atoi(choix) == 0 && strlen(choix) == 1) { cond1 = 1; } //choix doit etre une lettre uniquement de taille 1 (n'accepte pas des chiffres ou une chaine)

		else {
			cond1 = 0;
			printf("         choix invalide :(              Veuillez donner Une lettre ===>\t");

		}

	} while (cond1 == 0);

	if (cond2 == tabpassager[0].num) {
		color(7, 0);
		printf(" \t\t\t               il y a Aucun passagers dont le nom commence par %s\n", choix);
		printf("\n"); retour2(tabpassager, tabvol);
	}


	else { retour2(tabpassager, tabvol); }
}
//recherche selon une date de naissance
void searchdate(struct passager tabpassager[10]) {
	int verifdate(int dd, int mm, int yy);
	int dd = 0, mm = 0, yy = 0, i = 0, cond = 0;
	do {
		printf(" => Veuillez Donner une date de naissance à rechercher (sous la forme DD/MM/YYYY): ");
		scanf_s("%d/%d/%d", &dd, &mm, &yy);

	} while (verifdate(dd, mm, yy) == 0);

	for (i = 1; i <= tabpassager[0].num; i++) {
		if ((dd == tabpassager[i].dd) && (mm == tabpassager[i].mm) && (yy == tabpassager[i].yy)) {


			printf("\n");
			printf("                         passager numero %d\t", i);
			printf(" vol     \t\t %i \t", tabpassager[i].vol);

			printf("         \t%s\t", tabpassager[i].name);

			printf("         \t\t%s\t", tabpassager[i].sexe);

			printf("  %d %d %d\t  ", tabpassager[i].dd, tabpassager[i].mm, tabpassager[i].yy);

			printf(" %s\t                     ", tabpassager[i].cin);
			printf(" %s\n                     ", tabpassager[i].code);


		}

		else (cond += 1);

	}if (cond == tabpassager[0].num) printf("Aucun passagers possedant ce date de naissance\t");

}
//recherche selon le nom complet
void searchname(struct passager tabpassager[10], struct vol tabvol[10]) {
	int verifnom2(char a[100]);
	char nom[100];
	int i, cond = 0;
	do {
		getchar();
		printf("      => Veuillez donner le Nom et le prenom du passager: \n");
		gets_s(nom);
	} while (verifnom2(nom) == 0);
	for (i = 1; i <= tabpassager[0].num; i++) {
		if (strcmp(nom, tabpassager[i].name) == 0) {

			printf("\n");
			printf("                         passager numero %d\t", i);
			printf(" vol     \t\t %i \t", tabpassager[i].vol);

			printf("         \t%s\t", tabpassager[i].name);

			printf("         \t\t%s\t", tabpassager[i].sexe);

			printf("  %d %d %d\t  ", tabpassager[i].dd, tabpassager[i].mm, tabpassager[i].yy);

			printf(" %s\t                     ", tabpassager[i].cin);
			printf(" %s\n                     ", tabpassager[i].code);


		}
		else cond += 1;
	}
	if (cond == tabpassager[0].num) {
		printf("Aucun passagers dont le nom est  %s\t", nom);
		retour2(tabpassager, tabvol);
	}
	else { retour2(tabpassager, tabvol); }
}
void searchcode(struct passager tabpassager[10]) {
	int verifcode(char a[8]); int i = 0, cond = 0;

	char code[18];

	do {
		printf("=>Veuillez donner votre numero de passport\n");
		gets_s(code);
	} while (verifcode(code) == 0);
	for (i = 1; i <= tabpassager[0].num; i++) {
		if (strcmp(code, tabpassager[i].code) == 0) {

			printf("\n");
			printf("                         passager numero %d\t", i);
			printf(" vol     \t\t %i \t", tabpassager[i].vol);

			printf("         \t%s\t", tabpassager[i].name);

			printf("         \t\t%s\t", tabpassager[i].sexe);

			printf("  %d %d %d\t  ", tabpassager[i].dd, tabpassager[i].mm, tabpassager[i].yy);

			printf(" %s\t                     ", tabpassager[i].cin);
			printf(" %s\n                     ", tabpassager[i].code);


		}
		else cond += 1;
	}

	if (cond == tabpassager[0].num) printf("Aucun passagers possedant ce Code de Passport %s\t", code);

}
//recherche selon le genre et affichage de tous les passagers de ce genre
void searchsexe(struct passager tabpassager[10]) {
	char sexe[10]; int i, j, cond = 0;
	int verifsexe(char a[100]);
	getchar();
	do {
		printf("=>Veuillez Entrer H (pour Homme) ou F (pour femme):  \n");
		gets_s(sexe);
		for (j = 0; sexe[j] != '\0'; j++) {
			if (sexe[j] >= 'a' && sexe[j] <= 'z') {
				sexe[j] = sexe[j] - 32;
			}
		}
	} while (verifsexe(sexe) == 0);

	for (i = 1; i <= tabpassager[0].num; i++) {
		if (strcmp((sexe), (tabpassager[i].sexe)) == 0) {

			printf("\n");
			printf("                         passager numero %d\t", i);
			printf(" vol     \t\t %i \t", tabpassager[i].vol);

			printf("         \t%s\t", tabpassager[i].name);

			printf("         \t\t%s\t", tabpassager[i].sexe);

			printf("  %d %d %d\t  ", tabpassager[i].dd, tabpassager[i].mm, tabpassager[i].yy);

			printf(" %s\t                     ", tabpassager[i].cin);
			printf(" %s\n                     ", tabpassager[i].code);


		}
		else cond += 1;
	}

	if (cond == tabpassager[0].num) printf("pas de passagers de type %s \t", sexe);

}
//recherche selon numero CIN
void searchcin(struct passager tabpassager[10]) {
	int i = 0, cond = 0;
	int verifcin(char a[100]);
	char cin[100];
	do {
		printf("=>Veuillez donner le numero de CIN : \n");
		gets_s(cin);
	} while (verifcin(cin) == 0);
	for (i = 1; i <= tabpassager[0].num; i++) {
		if (strcmp(cin, tabpassager[i].cin) == 0) {

			printf("\n");
			printf("                         passager numero %d\t", i);
			printf(" vol     \t\t %i \t", tabpassager[i].vol);

			printf("         \t%s\t", tabpassager[i].name);

			printf("         \t\t%s\t", tabpassager[i].sexe);

			printf("  %d %d %d\t  ", tabpassager[i].dd, tabpassager[i].mm, tabpassager[i].yy);

			printf(" %s\t                     ", tabpassager[i].cin);
			printf(" %s\n                     ", tabpassager[i].code);


		}
		else cond += 1;
	}
	if (cond == tabpassager[0].num) printf("Aucun passagers possedant ce Numero de CIN\t");

} void searchvol(struct passager tabpassager[10], struct vol tabvol[10]) {
	int numvol, i;


	printf("=>Veuillez donner le numero de vol: \n");
	scanf_s("%d", &numvol);
	if (numvol == 0 || numvol > tabvol[1].num) printf(" Le Vol que vous etes entrain de chercher  n'existe pas");
	if (strcmp(tabvol[numvol].a, "ANNULER") == 0)printf(" Le Vol que vous etes entrain de chercher  a ete annule :(");
	else {
		for (i = 1; i <= tabpassager[0].num; i++) 
{
			if (tabpassager[i].vol == numvol) {

				printf("\n");
				printf("                         passager numero %d\t", i);
				printf(" vol     \t\t %i \t", tabpassager[i].vol);

				printf("         \t%s\t", tabpassager[i].name);

				printf("         \t\t%s\t", tabpassager[i].sexe);

				printf("  %d %d %d\t  ", tabpassager[i].dd, tabpassager[i].mm, tabpassager[i].yy);

				printf(" %s\t                     ", tabpassager[i].cin);
				printf(" %s\n                     ", tabpassager[i].code);


			}


		}





	}


}
//fonction de recherche principal (menu reliant les fonctions de recherche)
int chercherpassager(struct passager tabpassager[10], struct vol tabvol[10]) {
	int c, i;
	int option2(struct passager tabpassager[10], struct vol tabvol[10]);
	char choix[1];
	color(15, 0);


	puts("         |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||");
	puts("         ||||||||||||||||||||||||||||||||||||||||||||                                                                              |||||||||||||||||||||||||||||||||||");
	puts("         |||||||||||||||||||||||||||||||||              R E C H E R C H E   P A S S A G E R E   S E L O N                               ||||||||||||||||||||||||||||||");
	puts("         ||||||||||||||||||||||||||||                                                                                                             ||||||||||||||||||||");
	puts("         ||||||||||||||||||||||                                      L E S   C R I T E R E S   C I   D E S S O U S                                    ||||||||||||||||");
	puts("         |||||||||||||||||||||||||                                                                                                                ||||||||||||||||||||");
	puts("         |||||||||||||||||||||||||||||||||||||||||||                                                                               |||||||||||||||||||||||||||||||||||");
	puts("         |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||");
	printf("\n");
	printf("\n");
	printf("\n");
	printf("\n");

	color(1, 0);
	printf("                                                                                 1)Premiere Lettre du Nom                  \n");
	color(15, 0);
	printf("                                                                      ===============================================\n");
	color(2, 0);
	printf("                                                                                 2)Date de Naissance                       \n");
	color(15, 0);
	printf("                                                                      ===============================================\n");
	color(3, 0);
	printf("                                                                                 3)Nom du passager                          \n");
	color(15, 0);
	printf("                                                                      ===============================================\n");
	color(4, 0);
	printf("                                                                                  4)numero du vol                              \n");
	color(15, 0);
	printf("                                                                      ===============================================\n");
	color(5, 0);
	printf("                                                                                  5)CIN                                         \n");
	color(15, 0);
	printf("                                                                      ===============================================\n");
	color(6, 0);
	printf("                                                                                  6)Code Passport                              \n");
	color(15, 0);
	printf("                                                                      ===============================================\n");
	color(7, 0);
	printf("                                                                                  7)Affichage selon Le sexe                    \n");
	color(15, 0);
	printf("                                                                      ===============================================\n");
	color(13, 0);
	printf("                                                                                  8)Retour au Menu precedente                        \n");
	printf(" \n");
	color(11, 0);
	printf("                                                                      Veuillez donner votre choix ===> \t");

	scanf_s("%d", &c);
	color(3, 0);
	switch (c) {
	case 1:
		searchLettre(tabpassager, tabvol); retour2(tabpassager, tabvol); break;
	case 2:   searchdate(tabpassager); break;
	case 3:  searchname(tabpassager, tabvol); retour2(tabpassager, tabvol); break;
	case 4: searchvol(tabpassager, tabvol); retour2(tabpassager, tabvol); break;
	case 5:getchar(); searchcin(tabpassager); retour2(tabpassager, tabvol); break;
	case 6:getchar(); searchcode(tabpassager); retour2(tabpassager, tabvol); break;
	case 7: searchsexe(tabpassager); retour2(tabpassager, tabvol); break;

	case 8: system("cls"); option2(tabpassager, tabvol); break;


	default: system("cls"); chercherpassager(tabpassager, tabvol);

		break;
	}


	return 0;

}
//fonction permettant la modification du nom et du genre
void modifynameetsexe(struct passager tabpassager[10], char nom[100], int n) {
	int verifsexe(char a[100]);
	char sexe[10]; int i;
	strcpy_s(tabpassager[n].name, nom);
	do {
		printf("=>Veuillez Entrer H (pour Homme) ou F (pour femme):  \n");
		gets_s(sexe);
		for (i = 0; sexe[i] != '\0'; i++) {   //conversion en majuscule f=>F & h=>H
			if (sexe[i] >= 'a' && sexe[i] <= 'z') {
				sexe[i] = sexe[i] - 32;
			}
		}
	} while (verifsexe(sexe) == 0);
	strcpy_s(tabpassager[n].sexe, sexe);

} //modification du date de naissance
void modifydate(struct passager tabpassager[10], int dd, int mm, int yy, int n) {
	tabpassager[n].dd = dd;
	tabpassager[n].mm = mm;
	tabpassager[n].yy = yy;

} //modification de numero de CIN
void modifycin(struct passager tabpassager[10], char cin[100], int n) {
	strcpy_s(tabpassager[n].cin, cin);

}
//modification du code passport
void modifycode(struct passager tabpassager[10], char code[100], int n) {
	strcpy_s(tabpassager[n].code, code);

}
//fonction de suppression d'un passager
int supprimerpassager(struct passager tabpassager[10], struct vol tabvol[10]) {
	int verifnom2(char a[100]);
	int cond = 0, i, n = 0; char nom[100];
	color(1, 0);


	puts("                        |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||");
	puts("                        ||||||||||||||||||||||||||||||||||||||||||||                                                                              |||||||||||||||||||||||||||||||||||");
	puts("                        |||||||||||||||||||||||||||||||||                                                                                              ||||||||||||||||||||||||||||||");
	puts("                        ||||||||||||||||||||||||||||                                                                                                             ||||||||||||||||||||");
	puts("                        ||||||||||||||||||||||                                  * * * *   L I S T E    D E S    P A S S A G E R S* * * *                             ||||||||||||||||");
	puts("                        |||||||||||||||||||||||||                                                                                                                ||||||||||||||||||||");
	puts("                        |||||||||||||||||||||||||||||||||                                                                                              ||||||||||||||||||||||||||||||");
	puts("                        |||||||||||||||||||||||||||||||||||||||||||                                                                               |||||||||||||||||||||||||||||||||||");
	puts("                        |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||");
	printf("\n");
	printf("\n");
	color(5, 0);

	for (i = 1; i <= tabpassager[0].num; i++)
	{
		for (i = 1; i <= tabpassager[0].num; i++)
		{
			printf("\n");
			printf("                         passager numero %d\t", i);
			printf("         \t%s\t", tabpassager[i].name);

			printf("         \t\t%s\t", tabpassager[i].sexe);

			printf("  %d %d %d\t  ", tabpassager[i].dd, tabpassager[i].mm, tabpassager[i].yy);

			printf(" %s\t                     ", tabpassager[i].cin);
			printf(" %s\n                     ", tabpassager[i].code);
		}
	} getchar();
	do {

		printf("      Veuillez choisir le nom du passager a supprimer===> \t");
		gets_s(nom);
	} while (verifnom2(nom) == 0);
	for (i = 1; i <= tabpassager[0].num; i++) {
		if (strcmp(nom, tabpassager[i].name) == 0) {

			printf("\n");
			printf("                         passager numero %d\t", i);

			printf("         \t%s\t", tabpassager[i].name);

			printf("         \t\t%s\t", tabpassager[i].sexe);

			printf("  %d %d %d\t  ", tabpassager[i].dd, tabpassager[i].mm, tabpassager[i].yy);

			printf(" %s\t                     ", tabpassager[i].cin);
			printf(" %s\n                     ", tabpassager[i].code);
			n = i;

		}
		else { cond += 1; }
	}

	if (cond == tabpassager[0].num) {
		printf("Aucun passagers possedant ce Nom\t\n");

	}
	else {



		strcpy_s(tabpassager[n].name, "[Deleted]");
		strcpy_s(tabpassager[n].sexe, "");
		strcpy_s(tabpassager[n].cin, "[Deleted]");
		strcpy_s(tabpassager[n].code, "[Deleted]");
		tabpassager[n].dd = 00;
		tabpassager[n].mm = 00;
		tabpassager[n].yy = 0000;
		tabvol[tabpassager[n].vol].np++;
		tabpassager[n].vol = 0;



	}
	retour2(tabpassager, tabvol);
	return 0;
}
//gestionnaire de passagers (menu)
int option2(struct passager tabpassager[10], struct vol tabvol[10]) {
	int mainmenu(struct passager tabpassager[10], struct vol tabvol[10]);    //prototypes
	int modifypassager(struct passager tabpassager[10], struct vol tabvol[10]);
	int c;
	int getch();
	system("cls");
	color(9, 0);
	puts("  ");
	puts("  ");
	puts("  ");
	puts("=================================================  G  E  S  T  I  O  N  N  A  I  R  E      D  E     P  A  S  S  A  G  E  R  S    ! =================================================================");
	color(2, 0);
	printf("                                       =                                                                                                   =\n");
	printf("                                       =                                                                                                   =\n");
	printf("                                       =                                                                                                   =\n");
	printf("                                       =                    V E U I L L E Z    C H O I S I R   U N E   O P T I O N :                       =\n");
	printf("                                       =                                                                                                   =\n");
	printf("                                       =                                                                                                   =\n");
	printf("                                       =                                                                                                   =\n");
	printf("                                       =        1)LISTE DES PASSAGERS                                                                      =\n");
	printf("                                       =                                                                                                   =\n");
	printf("                                       =                                                                                                   =\n");
	printf("                                       =        2)CHERCHER UN PASSAGER                                                                     =\n");
	printf("                                       =                                                                                                   =\n");
	printf("                                       =                                                                                                   =\n");
	printf("                                       =        3)MODIFIER LES DONNEES DU PASSAGER                                                         =\n");
	printf("                                       =                                                                                                   =\n");
	printf("                                       =                                                                                                   =\n");
	printf("                                       =        4)SUPPRIMER UN PASSAGER                                                                    =\n");
	printf("                                       =                                                                                                   =\n");
	printf("                                       =                                                                                                   =\n");
	printf("                                       =        5)RETOUNRER AU MENU PRINCIPAL                                                              =\n");
	printf("                                       =                                                                                                   =\n");
	printf("                                       =====================================================================================================\n");
	printf(" \n");
	color(6, 0);
	printf("                                                                       donner votre choix ===> \t");
	scanf_s("%d", &c);
	switch (c)
	{


	case 1:int getch(); system("cls"); affichepassager(tabpassager, tabvol); break;
	case 2: int getch(); system("cls"); chercherpassager(tabpassager, tabvol); break;
	case 3: int getch(); system("cls"); modifypassager(tabpassager, tabvol); break;
	case 4: int getch(); system("cls"); supprimerpassager(tabpassager, tabvol); break;
	case 5:int getch(); system("cls"); mainmenu(tabpassager, tabvol); break;
	default:
		int getch(); system("cls");
		puts("\t\t\t<Choix invalide! veuillez donner un autre choix>\n");
		option2(tabpassager, tabvol);
		break;
	} return 0;
}
//gestionnaire de reservation (menu)
int option3(struct passager tabpassager[10], struct vol tabvol[10])
{
	int mainmenu(struct passager tabpassager[10], struct vol tabvol[10]);
	int reserver(passager tabpassager[10], struct vol tabvol[10]);
	int getch();
	system("cls");

	int c;
	color(9, 0);
	puts("  ");
	puts("  ");
	puts("  ");
	puts("=================================================  G  E  S  T  I  O  N  N  A  I  R  E        D  E      R  E  S  E  R  V  A  T  I  O  N  ! =========================================================================");
	color(2, 0);
	printf("                                       =                                                                                                        =\n");
	printf("                                       =                                                                                                        =\n");
	printf("                                       =                                                                                                        =\n");
	printf("                                       =                                                                                                        =\n");
	printf("                                       =                                                                                                        =\n");
	printf("                                       =                                    1)RESERVER UNE PLACE                                                =\n");
	printf("                                       =                                                                                                        =\n");
	printf("                                       =                                                                                                        =\n");
	printf("                                       =                                                                                                        =\n");
	printf("                                       =                                                                                                        =\n");
	printf("                                       =                                  2)RETOUR AU MENU PRINCIPAL                                            =\n");
	printf("                                       =                                                                                                        =\n");
	printf("                                       =                                                                                                        =\n");
	printf("                                       ==========================================================================================================\n");
	printf(" \n");
	color(6, 0);
	printf("                                                                      Veuillez donner votre choix ===> \t");

	scanf_s("%d", &c);
	switch (c) {
	case 1: reserver(tabpassager, tabvol); break;
	case 2: int getch(); system("cls"); mainmenu(tabpassager, tabvol); break;
	}
	return 0;
}
//menu principal
int mainmenu(struct passager tabpassager[10], struct vol tabvol[10])
{
	int quitter(struct passager tabpassager[10], struct vol tabvol[10]);
	int c;
	color(6, 0);
	puts(" ");

	puts(" ");
	puts(" ");
	printf("                          ********************************************************************************************************************************************                               \n");
	printf("                          *                                                                                                                                          *\n");
	printf("                          *                                                                                                                                          *\n");
	printf("                          *    S  Y  S  T  E  M  E       D  E      G  E  S  T  I  O  N     D  E  S     C  O  M  P  A  G  N  I  E  S      A  E  R  I  E  N  N  E  S   *\n");
	printf("                          *                                                                                                                                          * \n");
	printf("                          *                                                                                                                                          * \n");
	printf("                          *************************************************************             ******************************************************************\n");
	printf("                                                                                      *             *   \n");
	printf("                                                                                      *             *    \n");
	printf("                                                                                      *             *    \n");
	printf("                                                                                      *             *    \n");
	printf("                                                                                         *       *    \n");
	printf("                                                                                           *   * \n");
	printf("                                                                                             *     \n");
	puts(" ");
	color(9, 0);
	printf("=====================================================================   M   E  N  U        P  R  I  N  C  I  P  A  L      =======================================================================================\n");
	color(2, 0);
	printf("                                       =                                                                                                                    =\n");
	printf("                                       =                                                                                                                    =\n");
	printf("                                       =                                                                                                                    =\n");
	printf("                                       =                              V E U I L L E Z    C H O I S I R   U N E   O P T I O N :                              =\n");
	printf("                                       =                                                                                                                    =\n");
	printf("                                       =                                                                                                                    =\n");
	printf("                                       =                                                                                                                    =\n");
	printf("                                       =                                            1)GESTIONNAIRE DES VOLS                                                 =\n");
	printf("                                       =                                                                                                                    =\n");
	printf("                                       =                                                                                                                    =\n");
	printf("                                       =                                            2)GESTIONNAIRE DES PASSAGERS                                            =\n");
	printf("                                       =                                                                                                                    =\n");
	printf("                                       =                                                                                                                    =\n");
	printf("                                       =                                            3)GESTIONNAIRE DES RESERVATION                                          =\n");
	printf("                                       =                                                                                                                    =\n");
	printf("                                       =                                                                                                                    =\n");
	printf("                                       =                                            4) Quitter                                                              =\n");
	printf("                                       =                                                                                                                    =\n");
	printf("                                       =                                                                                                                    =\n");
	printf("                                       ======================================================================================================================\n");
	color(6, 0);

	printf(" \n");
	printf("                                                                      Veuillez donner votre choix ===> \t");
	scanf_s("%d", &c);


	switch (c) {
	case 1:
		option1(tabpassager, tabvol);
		break;

	case 2:
		option2(tabpassager, tabvol);
		break;

	case 3:
		option3(tabpassager, tabvol);
		break;
	case 4:
		quitter(tabpassager, tabvol);

		break;

	default:
		int getch(); system("cls");
		mainmenu(tabpassager, tabvol);
		break;
	};



	return 0;


}
//fonction d'arret final
int quitter(struct passager tabpassager[10], struct vol tabvol[10]) {

	int c;
	int getch();
	color(3, 0);
	system("cls");
	printf("Est-ce-que vous etes sure de quitter le programme?");
	printf("\t\t\t1)oui\t\t\t2)non\n");
	printf("=>");
	scanf_s("%d", &c);
	switch (c) {
	case 1:  exit(0);
		; break;
	case 2: int getch();
		system("cls");
		mainmenu(tabpassager, tabvol);
		break;
	default:
		int getch(); system("cls");
		printf("\t\t\t<Choix invalide! veuillez donner un autre choix>\n");
		mainmenu(tabpassager, tabvol);
		break;
	}
}

//fonction de verification de la validité du nom à l'entrée: non espacé, purement alphabétique et de longeur minimum 5
int verifnom(char a[100]) {

	if (strcmp(a, "") != 0 && strstr(a, "1") == 0 && strstr(a, "2") == 0 && strstr(a, "3") == 0 && strstr(a, "4") == 0 && strstr(a, "5") == 0 && strstr(a, "6") == 0 && strstr(a, "7") == 0 && strstr(a, "8") == 0 && strstr(a, "9") == 0 && strstr(a, "0") == 0 && strstr(a, " ") == 0 && strlen(a) <= 20 && strstr(a, "*") == 0 && strstr(a, "-") == 0 && strstr(a, "_") == 0 && strstr(a, "/") == 0 && strstr(a, "_") == 0 && strlen(a) >= 6) {
		color(9, 0);
		printf("\n");
		printf("                                                              NOM VALIDE :D !! \n");
		printf("\n");
		return 1;

	}
	else {
		color(4, 0);
		printf("                                                        OUPS, NOM INVALIDE :( !!   \n");
		printf("\n");
		color(15, 0);

		return 0;
	}

}

//fonction de verification de genre: H ou F
int verifsexe(char a[100]) {
	if (strlen(a) == 1 && ((strcmp(a, "H") == 0 || strcmp(a, "F") == 0 || strcmp(a, "h") == 0 || strcmp(a, "f") == 0)) && (strcmp(a, "") != 0 && strstr(a, "1") == 0 && strstr(a, "2") == 0 && strstr(a, "3") == 0 && strstr(a, "4") == 0 && strstr(a, "5") == 0 && strstr(a, "6") == 0 && strstr(a, "7") == 0 && strstr(a, "8") == 0 && strstr(a, "9") == 0 && strstr(a, "0") == 0 && strstr(a, " ") == 0))
	{
		color(9, 0);
		printf("\n");
		printf("                                                         CHOIX VALIDE :D ! :)\n");
		printf("\n");

		return 1;
	}

	else {
		color(4, 0);
		printf("                                                        OUPS, CHOIX INVALIDE :(  \n");  return 0;
		printf("\n");
		color(15, 0);
	}

}



// FONCTION QUI VERIFIE LA DATE  DE DEPART ET D'ARRIVéE
int verifdate(int dd, int mm, int yy)
{

	//verifions l'annee
	if (yy >= 1900 && yy <= 2021)
	{
		//verifions le mois 
		if (mm >= 1 && mm <= 12)
		{
			//verifions le jour
			if ((dd >= 1 && dd <= 31) && (mm == 1 || mm == 3 || mm == 5 || mm == 7 || mm == 8 || mm == 10 || mm == 12))
			{
				color(9, 0);
				printf("                                                     DATE VALIDE.:) \n");
				return 1;
			}
			else if ((dd >= 1 && dd <= 30) && (mm == 4 || mm == 6 || mm == 9 || mm == 11))
			{
				color(9, 0);
				printf("                                                    DATE VALIDE.:) \n"); return 1;
			}
			else if ((dd >= 1 && dd <= 28) && (mm == 2))
			{
				color(9, 0);
				printf("                                                    DATE VALID.:) \n");
				return 1;
			}
			else if (dd == 29 && mm == 2 && (yy % 400 == 0 || (yy % 4 == 0 && yy % 100 != 0)))
			{
				color(9, 0);
				printf("                                                     DATE VALIDE.:) \n");
			}
			else
			{
				color(4, 0);
				printf("                                                   OUPS, LE JOUR EST INVALIDE :( \n"); return 0;
			}
		}
		else
		{
			color(4, 0);
			printf("                                                        OUPS, LE MOIS EST INVALIDE :( \n"); return 0;
		}
	}
	else
	{
		color(4, 0);
		printf("                                           OUPS, L'ANNEE EST INVALIDE :( \n");
		return 0;
	}


}


//fonction de verification de la validité du numéro CIN

int verifcin(char a[100]) {
	if (strlen(a) == 8 && (atoi(a) != 0))   //atoi(str) fait  la conversion du chaine en valeur; si str n'est pas une chaine  purement numerique, atoi(str) retourne 0
	{
		color(9, 0);

		printf("                                                   CIN EST VALIDE  :)\n");
		return 1;
	}
	else {
		color(4, 0);

		printf("                                                  NUMERO DE CIN EST INVALIDE :< \n");
		return 0;
	}
}
//fonction de verification de la validité du code passport: commence par un caractere alphabetique et fini par 6 chiffres
int verifcode(char a[8]) {


	if (strlen(a) == 7 && isalpha(a[0]) && isdigit(a[1]) && isdigit(a[2]) && isdigit(a[3]) && isdigit(a[4]) && isdigit(a[5]) && isdigit(a[6]))
	{
		color(9, 0);
		printf("\n");
		printf("                                              NUMERO DE PASSEPORT EST VALIDE :)\n");
		return 1;
	}
	else {
		printf("\n");
		color(4, 0);
		printf("                                                 OUPS, NUMERO DE PASSPORT EST INVALIDE :<  \n");
		return 0;

	}
}
//une fonction de verification du nom qui n'exige pas que le nom soit de taille 5, utilisé pour chercher l'existance du nom d'un passager avant sa modification ou avant sa suppression
int verifnom2(char a[100]) {

	if (strcmp(a, "") != 0 && strstr(a, "1") == 0 && strstr(a, "2") == 0 && strstr(a, "3") == 0 && strstr(a, "4") == 0 && strstr(a, "5") == 0 && strstr(a, "6") == 0 && strstr(a, "7") == 0 && strstr(a, "8") == 0 && strstr(a, "9") == 0 && strstr(a, "0") == 0 && strstr(a, " ") == 0 && strlen(a) <= 20 && strstr(a, "*") == 0 && strstr(a, "-") == 0 && strstr(a, "_") == 0 && strstr(a, "/") == 0 && strstr(a, "_") == 0) {
		color(9, 0);

		return 1;

	}
	else {

		return 0;
	}

}

//fonction de modification de passagers(menu reliant les fonctions de modifications)
int modifypassager(struct passager tabpassager[10], struct vol tabvol[10]) {
	int verifnom(char a[100]);

	int c = 0, i, n, dd, mm, yy, cond = 0; char nom[100], nom2[100];
	char cin[100]; char code[100];
	color(1, 0);


	puts("                        |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||");
	puts("                        ||||||||||||||||||||||||||||||||||||||||||||                                                                              |||||||||||||||||||||||||||||||||||");
	puts("                        |||||||||||||||||||||||||||||||||                                                                                              ||||||||||||||||||||||||||||||");
	puts("                        ||||||||||||||||||||||||||||                                                                                                             ||||||||||||||||||||");
	puts("                        ||||||||||||||||||||||                                  * * * *   L I S T E    D E S    P A S S A G E R S* * * *                             ||||||||||||||||");
	puts("                        |||||||||||||||||||||||||                                                                                                                ||||||||||||||||||||");
	puts("                        |||||||||||||||||||||||||||||||||                                                                                              ||||||||||||||||||||||||||||||");
	puts("                        |||||||||||||||||||||||||||||||||||||||||||                                                                               |||||||||||||||||||||||||||||||||||");
	puts("                        |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||");
	printf("\n");
	printf("\n");
	color(5, 0);

	for (i = 1; i <= tabpassager[0].num; i++)
	{
		for (i = 1; i <= tabpassager[0].num; i++)
		{
			printf("\n");
			printf("                    passager numero %d\t", i);
			printf("         \t%s\t", tabpassager[i].name);

			printf("         \t\t%s\t", tabpassager[i].sexe);

			printf("  %d %d %d\t  ", tabpassager[i].dd, tabpassager[i].mm, tabpassager[i].yy);

			printf(" %s\t    ", tabpassager[i].cin);
			printf(" %s\n    ", tabpassager[i].code);
		}
	} getchar();
	do {
		color(5, 0);

		printf("\n");
		printf("      Veuillez choisir le nom du passager pour modifier ses donnees===> \t");
		gets_s(nom);
	} while (verifnom2(nom) == 0);
	for (i = 1; i <= tabpassager[0].num; i++) {
		if (strcmp(nom, tabpassager[i].name) == 0) {

			printf("\n");
			printf("                         passager numero %d\t", i);

			printf("         \t%s\t", tabpassager[i].name);

			printf("         \t\t%s\t", tabpassager[i].sexe);

			printf("  %d %d %d\t  ", tabpassager[i].dd, tabpassager[i].mm, tabpassager[i].yy);

			printf(" %s\t                     ", tabpassager[i].cin);
			printf(" %s\n                     ", tabpassager[i].code);
			n = i;

		}
		else { cond += 1; }
	}

	if (cond == tabpassager[0].num) {
		printf("Aucun passagers possedant ce Nom\t\n");
		retour2(tabpassager, tabvol);
	}
	else {
		printf("\n");
		printf("                ==========================Quel Donnee voulez-vous Changer============================\n");
		printf("                =                               1)Nom du passager et son sexe                       =\n");
		printf("                =                               2)Date de Naissance                                 =\n");
		printf("                =                               3)CIN                                               =\n");
		printf("                =                               4)Code Passport                                     =\n");
		printf("                =                               5)retour                                            =\n");
		printf("                =====================================================================================\n");

	}
	printf("                                                                      Veuillez donner votre choix ===> \t");
	scanf_s("%d", &c);
	switch (c) {
	case 1:
		do {
			getchar();

			printf("      Veuillez choisir le nouveau nom ===> \n");
			gets_s(nom2);
		} while (verifnom(nom2) == 0);
		modifynameetsexe(tabpassager, nom2, n); retour2(tabpassager, tabvol); break;


	case 2: do {
		getchar();
		printf(" => Veuiller Enter la date de naissance (sous la forme DD/MM/YYYY): ");
		scanf_s("%d/%d/%d", &dd, &mm, &yy);

	} while (verifdate(dd, mm, yy) == 0);
	modifydate(tabpassager, dd, mm, yy, n); retour2(tabpassager, tabvol); break;
	case 3: do {
		getchar();
		printf("=>Veuillez donner le numero de CIN : \n");
		gets_s(cin);
	} while (verifcin(cin) == 0);
	modifycin(tabpassager, cin, n);
	retour2(tabpassager, tabvol); break;
	case 4: do {
		getchar();
		printf("=>Veuillez donner votre numero de passport\n");
		gets_s(code);
	} while (verifcode(code) == 0);
	modifycode(tabpassager, code, n); retour2(tabpassager, tabvol); break;
	case 5: getchar(); retour2(tabpassager, tabvol); break;
	default: system("cls"); modifypassager(tabpassager, tabvol); break;

	}
	return 0;
}
//fonction de verification de la validité du numéro de vol, s'il existe, s'il est anulé ou s'il est valide
int verifnum(struct vol tabvol[10], struct passager tabpassager[10], int a) {
	int option3(struct passager tabpassager[10], struct vol tabvol[10]);
	int i, val = 0, choix = 0;

	if (a == 0 || a > tabvol[1].num) {
		color(4, 0);
		printf("                                                  NUMERO DE VOL N'EXISTE PAS ! ");
		color(7, 0); !
			printf("                                              Veuillez choisir 1 pour continuer ou 2 pour quitter");
		do {
			scanf_s("%d", &choix);
			if (choix == 1) { val = 1; }
			else if (choix == 2) option3(tabpassager, tabvol);
			else if (choix != 1 && choix != 2) { color(4, 0); printf("Vous n'avez pas choisi entre 1 et 2, essayer une autre fois"); }
		} while (choix != 1 && choix != 2);
	}
	else if (strcmp(tabvol[a].a, "ANNULER") == 0)
	{
		color(4, 0);
		printf("                                                CET VOL EST DEJA ANNULEE ! ");
		color(7, 0); !
			printf("                                           Veuillez choisir 1 pour continuer ou 2 pour quitter");
		do {
			scanf_s("%d", &choix);
			if (choix == 1)
			{
				val = 2; //invalide
			}


			else if (choix == 2) { option3(tabpassager, tabvol); }
			else if (choix != 1 && choix != 2) { color(4, 0); printf("Vous n'avez pas choisi entre 1 et 2, essayer une autre fois"); }
		} while (choix != 1 && choix != 2);
	}
	else
		if (tabvol[a].np == 0) {
			color(4, 0);
			printf("                                          NOMBRE DE PLACE EST SATUREE ! ");
			color(7, 0); !
				printf("                                    Veuillez choisir 1 pour continuer ou 2 pour quitter");
			do {
				scanf_s("%d", &choix);
				if (choix == 1) val = 1; //invalide
				else if (choix == 2) { option3(tabpassager, tabvol); }
				else if (choix != 1 && choix != 2) {
					color(4, 0);
					printf("Vous n'avez pas choisi entre 1 et 2, essayer une autre fois");
				}


			} while (choix != 1 && choix != 2);
		}

		else { val = 0; } //valide



	return val;
}
//FONCTION  QUI PERMET DE RESERVER LES PASSAGERS
int reserver(passager tabpassager[10], struct vol tabvol[10])
{
	int getch(); system("cls");
	char nom[100]{};
	char sexe[100]{};
	int dd = 0, mm = 0, yy = 0;
	char cin[10]{};
	char code[10]{};
	int numvol;
	int i;
	color(13, 0);

	puts("            |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||");
	puts("            ||||||||||||||||||||||||||||||||||||||||||||                                                                              |||||||||||||||||||||||||||||||||||");
	puts("            |||||||||||||||||||||||||||||||||                                                                                              ||||||||||||||||||||||||||||||");
	puts("            ||||||||||||||||||||||||||||                B I E N V E N U E                                                                            ||||||||||||||||||||");
	puts("            ||||||||||||||||||||||                                           A U   F O R M U L A I R E                                                   ||||||||||||||||");
	puts("            |||||||||||||||||||||||||                                                                      DE   R S E R V A T I O N                  ||||||||||||||||||||");
	puts("            |||||||||||||||||||||||||||||||||                                                                                              ||||||||||||||||||||||||||||||");
	puts("            |||||||||||||||||||||||||||||||||||||||||||                                                                               |||||||||||||||||||||||||||||||||||");
	puts("            |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||");
	printf("\n");
	printf("\n");
	color(15, 0);
	getchar(); //getchar() empeche le programme de considerer l'appuie sur ENTREE comme un donnée à executer dans la boucle /HUH??
	//VERIF NOM
	do {
		printf("                                                         + Veuillez donner le Nom et le prenom du passager: \n");
		color(11, 0);
		printf("                                                            (pas d'espace/minimun taille : 5 /de chiffre/de caracteres speciaux)\t");
		printf("\n");
		color(2, 0);
		gets_s(nom);
	} while (verifnom(nom) == 0);

	//VERIF DATE DE NAISSANCE
	do {
		color(15, 0);

		printf("                                                        + Veuiller Enter la date de naissance :\n ");
		color(11, 0);
		printf("                                                               (sous la forme DD/MM/YYYY) \n");
		color(2, 0);
		scanf_s("%d/%d/%d", &dd, &mm, &yy);
		printf("\n");
	} while (verifdate(dd, mm, yy) == 0);

	//VERIF SEXE
	getchar();
	do {
		color(15, 0);
		printf("\n");

		printf("                                                        +Veuillez Entrer le sexe :  \n");
		color(11, 0);
		printf("                                                        (H pour Homme ou F pour Femme)\n");
		color(2, 0);
		gets_s(sexe);
		printf("\n");

		for (i = 0; sexe[i] != '\0'; i++)
		{
			if (sexe[i] >= 'a' && sexe[i] <= 'z')
			{
				sexe[i] = sexe[i] - 32;
			}
		}
	} while (verifsexe(sexe) == 0);

	//VERIF NUMERO DE VOLS                                      
	do {
		color(15, 0);
		printf("                                                           + donner le numero de vol: \n");

		color(2, 0);
		scanf_s("%d", &numvol);
	} while (verifnum(tabvol, tabpassager, numvol) != 0);
	color(9, 0);
	printf("                                                                      CHOIX VALIDE :D !!\n");

	// VERIF CIN
	getchar();
	do {

		color(15, 0);
		printf("                                                       +Veuillez donner le numero de CIN : \n");
		color(11, 0);
		printf("                                                    (le numero de cin doit etre compose de 8 chiffres)\n");
		color(2, 0);
		gets_s(cin);
		printf("\n");

	} while (verifcin(cin) == 0);
	//VERIF CODE PASSPORT
	do {
		color(15, 0);
		printf("\n");
		printf("                                                    +Veuillez donner votre numero de passport\n");
		color(11, 0);
		printf("                                                            ( sous la forme -->A123456)\n");

		color(2, 0);
		gets_s(code);
		printf("\n");
	} while (verifcode(code) == 0);
	if (verifnom(nom) == 1 && verifdate(dd, mm, yy) == 1 && verifsexe(sexe) == 1 && verifcin(cin) == 1 && verifcode(code) == 1)

		confirmer(nom, dd, mm, yy, sexe, cin, code, tabpassager, tabvol, numvol);
	return 0;
}
//fonction de retour (menu de reservation ou mainmenu)
void retour1(struct passager tabpassager[10], struct vol tabvol[10]) {

	int c;
	color(7, 0);

	puts("                                 |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||");
	puts("                                 ||||||||||||||||||||||||||||||||||||||||||||                                                                              |||||||||||||||||||||||||||||||||||");
	puts("                                 |||||||||||||||||||||||||||||||||                       VEUILLEZ RETOURNER AU                                                  ||||||||||||||||||||||||||||||");
	puts("                                 ||||||||||||||||||||||||||||                                                                                                             ||||||||||||||||||||");
	puts("                                 ||||||||||||||||||||||                                1) MENU PRECEDENT                                                                      ||||||||||||||||");
	puts("                                 |||||||||||||||||||||||||                                                                                                                ||||||||||||||||||||");
	puts("                                 |||||||||||||||||||||||||||||||||                     2) MENU PRINCIPAL                                                        ||||||||||||||||||||||||||||||");
	puts("                                 |||||||||||||||||||||||||||||||||||||||||||                                                                               |||||||||||||||||||||||||||||||||||");
	puts("                                 |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||");
	color(15, 0);
	printf("                                                            ========> votre choix : ");
	scanf_s("%d", &c);
	switch (c) {
	case 1: system("cls"); option3(tabpassager, tabvol); break;
	case 2: system("cls"); mainmenu(tabpassager, tabvol); break;
	default:system("cls"); retour1(tabpassager, tabvol); break;
	}
}

//et biensur, le main :) 
int main()
{
	struct passager tabpassager[10];
	struct vol tabvol[10];
	//ceci des vols remplis par defaut

	tabvol[1] = { 1,"Tunisie","Canada", 10,1,2021,20,1,2022,20,5 };
	tabvol[2] = { 2,"Tunisie","Egypt", 11,1,2021,21,1,2022,90 };
	tabvol[3] = { 3,"Tunisie","greece", 12,1,2021,22,1,2022,100 };
	tabvol[4] = { 4, "Tunisie","France", 20,1,2021,30,1,2022,3 };
	tabvol[5] = { 5,"Tunisie","Allemagne", 30,1,2021,9,2,2022,0 };




	//ceci quelques passagers remplis par defauts
	tabpassager[1] = { "ahmedkacem", "H" , 15,3,2000 , "11167349" , "q982345", 1 };
	tabpassager[2] = { "mounachaben", "F", 12 , 12 , 2012, "11234691", "e652187", 1 };
	tabpassager[3] = { "azizmezghani", "H", 11, 1, 1999, "12263478", "t652327", 3 };
	tabpassager[4] = { "karimhsairi","H", 5,5,1995,"11248379","n258369", 4 };
	tabpassager[5] = { "azzaslimen", "F", 6,7,2001,"11345983", "d325489",3 };
	anim1();
	bienvenue();

	logo1anim(); logo2();
	delay(10);

	system("cls");
	mainmenu(tabpassager, tabvol);




	return 0;
}
