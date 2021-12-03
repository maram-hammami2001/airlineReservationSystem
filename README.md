#include<windows.h>
#include<stdio.h>
#include<stdlib.h>
#include<string.h>
#include<string>
#include<conio.h>
#include<ctype.h>
void color(int t, int f)
{
	HANDLE H = GetStdHandle(STD_OUTPUT_HANDLE); //fonction appartenant a la biblio windows.h permettant la modificationdes couleur
	SetConsoleTextAttribute(H, f * 16 + t);
}

void bienvenue() {
	int getchar();
	color(9, 0);
	puts(" ");
	puts(" ");
	puts(" ");
	puts(" ");
	puts(" ");
	puts(" ");
	puts(" ");
	puts(" ");
	puts(" ");
	puts(" ");
	printf("                   bbbbbbbb                                                                                                                                                              \n");
	printf("                   b::::::b              iiii                                                                                                                                        !!!\n");
	printf("                   b::::::b             i::::i                                                                                                                                      !!:!!\n");
	printf("                   b::::::b              iiii                                                                                                                                       !:::!\n");
	printf("                   b:::::b                                                                                                                                                         !:::!\n");
	printf("                   b:::::bbbbbbbbb    iiiiiii     eeeeeeeeeeee    nnnn  nnnnnnnn vvvvvvv           vvvvvvv eeeeeeeeeeee    nnnn  nnnnnnnn    uuuuuu    uuuuuu      eeeeeeeeeeee    !:::!\n");
	printf("                   b::::::::::::::bb  i:::::i   ee::::::::::::ee  n:::nn::::::::nnv:::::v         v:::::vee::::::::::::ee  n:::nn::::::::nn  u::::u    u::::u    ee::::::::::::ee  !:::!\n");
	printf("                   b::::::::::::::::b  i::::i  e::::::eeeee:::::een::::::::::::::nnv:::::v       v:::::ve::::::eeeee:::::een::::::::::::::nn u::::u    u::::u   e::::::eeeee:::::ee!:::!\n");
	printf("                   b:::::bbbbb:::::::b i::::i e::::::e     e:::::enn:::::::::::::::nv:::::v     v:::::ve::::::e     e:::::enn:::::::::::::::nu::::u    u::::u  e::::::e     e:::::e!:::!\n");
	printf("                   b:::::b    b::::::b i::::i e:::::::eeeee::::::e  n:::::nnnn:::::n v:::::v   v:::::v e:::::::eeeee::::::e  n:::::nnnn:::::nu::::u    u::::u  e:::::::eeeee::::::e!:::!\n");
	printf("                   b :::::b     b:::::b i::::i e:::::::::::::::::e   n::::n    n::::n  v:::::v v:::::v  e:::::::::::::::::e   n::::n    n::::nu::::u    u::::u  e:::::::::::::::::e !:::!\n");
	printf("                   b:::::b     b:::::b i::::i e::::::eeeeeeeeeee    n::::n    n::::n   v:::::v:::::v   e::::::eeeeeeeeeee    n::::n    n::::nu::::u    u::::u  e::::::eeeeeeeeeee  !!:!!\n");
	printf("                   b:::::b     b:::::b i::::i e:::::::e             n::::n    n::::n    v:::::::::v    e:::::::e             n::::n    n::::nu:::::uuuu:::::u  e:::::::e            !!! \n");
	printf("                   b:::::bbbbbb::::::bi::::::ie::::::::e            n::::n    n::::n     v:::::::v     e::::::::e            n::::n    n::::nu:::::::::::::::uue::::::::e               \n");
	printf("                   b::::::::::::::::b i::::::i e::::::::eeeeeeee    n::::n    n::::n      v:::::v       e::::::::eeeeeeee    n::::n    n::::n u:::::::::::::::u e::::::::eeeeeeee   !!! \n");
	printf("                   b:::::::::::::::b  i::::::i  ee:::::::::::::e    n::::n    n::::n       v:::v         ee:::::::::::::e    n::::n    n::::n  uu::::::::uu:::u  ee:::::::::::::e  !!:!!\n");
	printf("                   bbbbbbbbbbbbbbbb   iiiiiiii    eeeeeeeeeeeeee    nnnnnn    nnnnnn        vvv            eeeeeeeeeeeeee    nnnnnn    nnnnnn    uuuuuuuu  uuuu    eeeeeeeeeeeeee   !!! \n");
	color(8, 0);
	printf("\n");
	printf("                                   ------------------------------------ Veuillez appuyer sur entrer pour continuer :> !-----------------------------------\n");
	getchar();
}
int mainmenu()
{
	int  option1();
	void option2();
	void option3();
	void quitter();
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
	printf("=====================================================================   M   E  N  U        P  R  I  N  C  I  P  A  L  E   =======================================================================================\n");
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
		option1();
		break;

	case 2:
		option2();
		break;

	case 3:
		option3();
		break;
	case 4:  
		quitter();

		break;

	default:
		int getch(); system("cls");
		mainmenu();
		break;
	};



	return 0;


}


int option1() {
	int vol1 = 0, vol2 = 3, vol3 = 3, vol4 = 3, vol5 = 3, c, getch();
	int affiche1(int vol1, int vol2, int vol3, int vol4, int vol5);
	int annuler(int vol1, int vol2, int vol3, int vol4, int vol5);
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
	printf("                                       =        2)ANNULATION DE VOL                                                              =\n");
	printf("                                       =                                                                                         =\n");
	printf("                                       =                                                                                         =\n");
	printf("                                       =        3)LA LISTE DES VOLS VALABLES ET NON VALABLES                                     =\n");
	printf("                                       =                                                                                         =\n");
	printf("                                       =                                                                                         =\n");
	printf("                                       =        4)RETOUR AU MENU PRINCIPAL                                                       =\n");
	printf("                                       =                                                                                         =\n");
	printf("                                       =                                                                                         =\n");
	printf("                                       ===========================================================================================\n");
	printf(" \n");
	color(6, 0);
	printf("                                                                      Veuillez donner votre choix ===> \t");

	scanf_s("%d", &c);
	switch (c) {
	case 1:
		affiche1(vol1, vol2, vol3, vol4, vol5);
		break;
	case 2:
		annuler(vol1, vol2, vol3, vol4, vol5); break;
	case 4:
		getch();
		system("cls");
		mainmenu();
		break;


	}
	return 0;
}

int affiche1(int vol1, int vol2, int vol3, int vol4, int vol5)
{
	int  getch(), rep;//why getch is definied here
	system("cls");
	color(9, 0);

	puts("|||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||");
	puts("|                                                                                                                                                           |");
	puts("|                                                                                                                                                           |");
	puts("|                                                    * * * *   L I S T E    D E S    V O L S  * * * *                                                       |");
	puts("|                                                                                                                                                           |");
	puts("|                                                                                                                                                           |");
	puts("|||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||");
	puts(" ");
	puts(" ");
	puts(" ");
	puts(" ");
	color(2, 0);
	printf("              DE              A                DEPART               RETOUR                   CLASSE DE CABINE            Nombre de place valable            \n");
	printf("\n");
	printf("\n");

	printf("\n");

	printf("           TUNISIE         DJERBA             05/12/2021          12/12/2021                 1 ADULTE,ECONOMIQUE     \t");
	if (vol1 == 0)
	{
		printf("no more available seats\n");
	}
	else
	{
		printf("     %d\n    ", vol1);
	};
	printf("\n");
	printf("\n");
	printf("\n");

	printf("           TUNISIE         EGYPT              06/12/2021          13/12/2021                 1 ADULTE,ECONOMIQUE     \t");
	if (vol2 == 0)
	{
		printf("no more available seats\n");
	}
	else
	{
		printf("     %d\n    ", vol2);
	};
	printf("\n");
	printf("\n");
	printf("\n");

	printf("          TUNISIE         FRANCE             07/12/2021          14/12/2021                 1 ADULTE,ECONOMIQUE     \t");
	if (vol3 == 0)
	{
		printf("no more available seats\n");
	}
	else
	{
		printf("     %d\n    ", vol3);
	};
	printf("\n");
	printf("\n");
	printf("\n");

	printf("          TUNISIE         MALTA              08/12/2021          15/12/2021                 1 ADULTE,ECONOMIQUE     \t");
	if (vol4 == 0)
	{
		printf("no more available seats\n");
	}
	else
	{
		printf("     %d\n    ", vol4);
	};
	printf("\n");
	printf("\n");
	printf("\n");

	printf("          TUNISIE         GREECE             10/12/2021          16/12/2021                 1 ADULTE,ECONOMIQUE     \t");
	if (vol5 == 0)
	{
		printf("no more available seats\n");
	}
	else
	{
		printf("     %d\n    ", vol5);
	};
	printf("\n");
	printf("\n");
	printf("\n");
	printf("                                                                             -----------------------------------------------\n");
	color(6, 0);

	printf("                                                                                  voulez vous retourner au menu precedant? ");
	printf(" \n");
	printf("                                                                        *veuillez entrer oui sinon tapper entrer pour quitter le programme*");
	scanf_s("%d", &rep);
	if (rep == 1)
	{
		system("cls");
		option1();
	}
	//problem when the rep is not 1 the program should be closed by typing enter, didn't work find a way xDD
	return 0;
}




int annuler(int vol1, int vol2, int vol3, int vol4, int vol5)
{
	int choix, value;
	char vol1s[20]{};
	char r1[5]{};
	char r2[5] = { "oui" };
	system("cls");
	color(9, 0);
	printf("\n");

	puts("=================================================  A  N  N  U  L  A  T  I  O  N       D  E  S       V  O  L  S ! ============================================================================");
	color(2, 0);
	printf("                                                                             .\n");
	printf("                                                                             .\n");
	printf("                                                                             .\n");
	printf("                                                          QUELLE EST LE VOL QUE VOUS DEVEZ ANNULER ?");
	puts("");
	puts("");

	puts("");
	printf("                                      1==>TUNISIE         DJERBA             05/12/2021          12/12/2021                 \n");
	puts("");
	puts("");

	printf("                                      2==>TUNISIE         EGYPT              06/12/2021          13/12/2021                 \n");
	puts("");

	puts("");
	printf("                                      3==>TUNISIE         FRANCE             07/12/2021          14/12/2021                 \n");
	puts("");

	puts("");
	printf("                                      4==>TUNISIE         MALTA              08/12/2021          15/12/2021                 \n");
	puts("");

	puts("");
	printf("                                      5==>TUNISIE         GREECE             10/12/2021          16/12/2021                 \n");
	puts("");

	scanf_s("%d", &choix);
	switch (choix)
	{
	case 1:

		system("cls");
		color(12, 0);

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

		printf("                                                                   VOULEZ VOUS VRAIMENT ANNULER LE PREMIER VOL ? ");
		/*scanf_s("%s", &r1);

		value = strcmp(r1, r2);//a predefined function  to compare whether r1 which is the input oui is the same as r2 which is oui by default and thereafter recieves 1 if they are the same
		if (value == 1)
		{
			printf("LA PREMIERE VOL A ETE ANNULER AVEC SUCCEES :>");
		}


		; break;
		   case 2:

			 ;
			 break;
		 case 3:

			 ;
			 break;
		 case 4:

			 ;
			 break;
		 case 5:

			 ;
			 break;*/
	}

	return 0;
}
void affichepassager() {


}


void option2() {
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


	case 1: affichepassager();
	case 5:int getch(); system("cls"); mainmenu(); break;
	default:
		int getch(); system("cls");
		puts("\t\t\t<Choix invalide! veuillez donner un autre choix>\n");
		option2();
		break;
	}
}
 void option3()
    {
	int reserver();
	int getch();
	system("cls");

	int c;
	color(9, 0);
	puts("  ");
	puts("  ");
	puts("  ");
	puts("=================================================  G  E  S  T  I  O  N  N  A  I  R  E        D  E      R  E  S  E  R  V  A  T  I  O  N  ! ============================================================================");
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
	case 1: reserver(); break;
	case 2: int getch(); system("cls"); mainmenu(); break;
	}
	
}
int verifnom(char a[100]) {
	if (strcmp(a, "") == 0 && strcmp(a, "1234567890") == 0 && strcmp(a, " ") == 0 && strlen(a) <= 20) return 1;
	else return 0;

}
int verifdate(int dd, int mm, int yy)
{

	//verifions l'annee
	if (yy >= 1900 && yy <= 9999)
	{
		//verifions le mois
		if (mm >= 1 && mm <= 12)
		{
			//verifions le jour
			if ((dd >= 1 && dd <= 31) && (mm == 1 || mm == 3 || mm == 5 || mm == 7 || mm == 8 || mm == 10 || mm == 12))
			{
				printf("Date is valid.\n");
				return 1;
			}
			else if ((dd >= 1 && dd <= 30) && (mm == 4 || mm == 6 || mm == 9 || mm == 11))
			{
				printf("Date is valid.\n"); return 1;
			}
			else if ((dd >= 1 && dd <= 28) && (mm == 2))
			{
				printf("Date is valid.\n");
				return 1;
			}
			else if (dd == 29 && mm == 2 && (yy % 400 == 0 || (yy % 4 == 0 && yy % 100 != 0)))
				printf("Date is valid.\n");
			else
			{
				printf("Day is invalid.\n"); return 0;
			}
		}
		else
		{
			printf("Month is not valid.\n"); return 0;
		}
	}
	else
	{
		printf("Year is not valid.\n");
		return 0;
	}


}

int reserver()
{
	int getch(); system("cls");
	char nom[100]{};
	int dd = 0, mm = 0, yy = 0;

	color(12, 0);
	puts("==========================================Bienvenue au Fomulaire du reservation!========================================");

	do {
		printf("      => Veuillez donner le Nom du passager: \n");
		gets_s(nom);
	} while (verifnom(nom) == 0);
	do {
		printf(" => Veuiller Enter la date de naissance (sous la forme DD/MM/YYYY): ");
		scanf_s("%d/%d/%d", &dd, &mm, &yy);

	} while (verifdate(dd, mm, yy) == 0);

	return 0;

}





void quitter() {
	int c;
	int getch();
	color(3, 0);
	system("cls");
	printf("Est-ce-que vous etes sure de quitter le programme?");
	printf("\t\t\t1)oui\t\t\t2)non\n");
	printf("=>");
	scanf_s("%d", &c);
	switch (c) {
	case 1: exit(EXIT_SUCCESS); break;
	case 2: int getch();
		system("cls");
		mainmenu();
		break;
	default:
		int getch(); system("cls");
		printf("\t\t\t<Choix invalide! veuillez donner un autre choix>\n");
		mainmenu();
		break;
	}
}


int main()
{
	bienvenue();
	int getch();
	system("cls");
	mainmenu();

	return 0;
}
