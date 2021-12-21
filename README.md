#include<windows.h>
#include<stdio.h>
#include<stdlib.h>
#include<string.h>
#include<string>
#include<conio.h>
#include<ctype.h>

struct vol {
	int nv; //numero de vol
	char dep[10]; //pays depart
	char ar[20];  //pays arrnivée
	char ddep[20]; //date depart
	char dar[20];  //date arrivée
	int np;  //nombre de place valable
};
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
	int c; 
	struct vol vol1, vol2, vol3, vol4, vol5; 
	int affiche1(struct vol vol1, struct vol vol2, struct vol vol3, struct vol vol4, struct vol vol5);
	int annuler(struct vol vol1, struct vol vol2, struct vol vol3, struct vol vol4, struct vol vol5);
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
		affiche1();
		break;
	case 2:
		annuler(); break;
	case 4:
		_getch();
		system("cls");
		mainmenu();
		break;


	}
	return 0;
}

int affiche1(struct vol vol1, struct vol vol2, struct vol vol3, struct vol vol4, struct vol vol5)
{
	int  getch(), rep;//why getch is definied here
	system("cls");
	color(9, 0);

	puts("            |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||");
	puts("            ||||||||||||||||||||||||||||||||||||||||||||                                                                              |||||||||||||||||||||||||||||||||||");
	puts("            |||||||||||||||||||||||||||||||||                                                                                              ||||||||||||||||||||||||||||||");
	puts("            ||||||||||||||||||||||||||||                                                                                                             ||||||||||||||||||||");
	puts("            ||||||||||||||||||||||                                  * * * *   L I S T E    D E S    V O L S  * * * *                                     ||||||||||||||||");
	puts("            |||||||||||||||||||||||||                                                                                                                ||||||||||||||||||||");
	puts("            |||||||||||||||||||||||||||||||||                                                                                              ||||||||||||||||||||||||||||||");
	puts("            |||||||||||||||||||||||||||||||||||||||||||                                                                               |||||||||||||||||||||||||||||||||||");
	puts("            |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||");
	puts(" ");
	puts(" ");
	puts(" ");
	puts(" ");
	color(2, 0); 
	printf("                             DE                    A                       DEPART                    RETOUR                                     Nombre de place valable( CLASSE DE CABINE( 1 ADULTE,ECONOMIQUE) )            \n");
	printf("\n");
	printf("\n");
	vol1 = { 1,"Tunisie","Canada", "10/1/2021","20/1/2022",3};
	if (vol1.np == 0)
	{
		printf("     vol : %d               %s                   %s                        %s                        %s                                                no more available seats             \t",vol1.nv,vol1.dep,vol1.ar,vol1.ddep,vol1.dar);
	}
	else
		printf("      vol : %d              %s                   %s                        %s                        %s                                                %d                                 \t",vol1.nv ,vol1.dep, vol1.ar, vol1.ddep, vol1.dar,vol1.np);

	printf("\n");
	vol2 = {2,"Tunisie","Egypt", "11/1/2021","21/1/2022",90 };
	if (vol2.np == 0)
	{
		printf("     vol : %d               %s                    %s                        %s                       %s                                               no more available seats             \t",vol2.nv ,vol2.dep, vol2.ar, vol2.ddep, vol2.dar);
	}
	else
		printf("     vol : %d               %s                   %s                         %s                        %s                                                %d                                 \t",vol2.nv ,vol2.dep, vol2.ar, vol2.ddep, vol2.dar, vol2.np);

	printf("\n");
	vol3 = {3,"Tunisie","greece", "12/1/2021","22/1/2022",100 };
	if (vol3.np == 0)
	{
		printf("    vol : %d                %s                   %s                        %s                         %s                                               no more available seats             \t",vol3.nv ,vol3.dep, vol3.ar, vol3.ddep, vol3.dar);
	}
	else
		printf("     vol : %d               %s                   %s                        %s                         %s                                                %d                                 \t", vol3.nv,vol3.dep, vol3.ar, vol3.ddep, vol3.dar, vol3.np);

	printf("\n");
	vol4 = { 4, "Tunisie","France", "20/1/2021","30/1/2022",3 };
	if (vol4.np == 0)
	{
		printf("      vol : %d              %s			         %s					      %s					      %s                                               no more available seats             \t", vol4.nv,vol4.dep, vol4.ar, vol4.ddep, vol4.dar);
	}
	else
		printf("      vol : %d              %s                   %s                       %s                          %s                                                 %d                                 \t", vol4.nv,vol4.dep, vol4.ar, vol4.ddep, vol4.dar, vol4.np);

	printf("\n");
	vol5 = {5,"Tunisie","Allemagne", "30/1/2021","9/2/2022",3 };
	if (vol1.np == 0)
	{
		printf("      vol : %d             %s                    %s                       %s                          %s                                               no more available seats             \t", vol5.nv,vol5.dep, vol5.ar, vol5.ddep, vol5.dar);
	}
	else
		printf("      vol : %d             %s                    %s                       %s                          %s                                                %d                                 \t", vol5.nv,vol5.dep, vol5.ar, vol5.ddep, vol5.dar, vol5.np);

	

	printf("\n");

	printf("\n");
	printf("\n");
	printf("\n");
	printf("                                                                             -----------------------------------------------\n");
	color(6, 0);

	printf("                                                                                  voulez vous retourner au menu precedent? ");
	printf(" \n");
	printf("                                                                        *veuillez entrer oui sinon tapper entrer pour quitter le programme*");
	scanf_s("%d", &rep);
	if (rep == 1)
	{
		system("cls");
	}
	//problem when the rep is not 1 the program should be closed by typing enter, didn't work find a way xDD
	return 0;
}




int annuler(struct vol vol1, struct vol vol2, struct vol vol3, struct vol vol4, struct vol vol5)
{
	char oui[5] = {"oui"};
	int choix;// numero de vol 
	char on[5]; // on stands for oui non
	char vol1s[20]{};
	char r1[5]{};
	char r2[5] = { "oui" };
	system("cls");
	color(9, 0);
	printf("\n");

	puts("=============================================================  A  N  N  U  L  A  T  I  O  N       D  E  S       V  O  L  S ! ============================================================================");
	color(2, 0);
	printf("                                                                             .\n");
	printf("                                                                             .\n");
	printf("                                                                             .\n");
	printf("                                                          QUELLE EST LE VOL QUE VOUS DEVEZ ANNULER ?");
	puts("");
	puts("");
	printf("                             DE                    A                       DEPART                    RETOUR                                     Nombre de place valable( CLASSE DE CABINE( 1 ADULTE,ECONOMIQUE) )            \n");
	printf("\n");
	printf("\n");
	vol1 = { 1,"Tunisie","Canada", "10/1/2021","20/1/2022",3 };
		printf("      vol : %d              %s                   %s                        %s                        %s                                                %d                                 \t", vol1.nv, vol1.dep, vol1.ar, vol1.ddep, vol1.dar, vol1.np);
	printf("\n");
	vol2 = { 2,"Tunisie","Egypt", "11/1/2021","21/1/2022",90 };
	
		printf("     vol : %d               %s                   %s                         %s                        %s                                                %d                                 \t", vol2.nv, vol2.dep, vol2.ar, vol2.ddep, vol2.dar, vol2.np);
		printf("\n");

		printf("     vol : %d               %s                   %s                        %s                         %s                                                %d                                 \t", vol3.nv, vol3.dep, vol3.ar, vol3.ddep, vol3.dar, vol3.np);
	printf("\n");
	vol4 = { 4, "Tunisie","France", "20/1/2021","30/1/2022",3 };
		printf("      vol : %d              %s                   %s                        %s                          %s                                               %d                                 \t", vol4.nv, vol4.dep, vol4.ar, vol4.ddep, vol4.dar, vol4.np);
	printf("\n");
	vol5 = { 5,"Tunisie","Allemagne", "30/1/2021","9/2/2022",3 };
		printf("      vol : %d             %s                    %s                       %s                          %s                                                %d                                 \t", vol5.nv, vol5.dep, vol5.ar, vol5.ddep, vol5.dar, vol5.np);

		printf("donner le numero de vol que vous voulez annuler");
	scanf_s("%d", &choix);
	system("cls");

	if (choix<6 || choix>0)
	{
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
		printf("    \n");

		printf("                                                                   VOULEZ VOUS VRAIMENT ANNULER LE %d VOL ? ",choix);
		printf("    \n");
		printf("    \n");

		printf("                                                                                   oui / non               ");
	
		gets_s(on); 
		if (strcmp(on,oui ))
		{

		}
		else
		{
			mainmenu();
		}
	}
	
	else
		printf("vol numero %d n'existe pas",choix);
	
	return 0;
}

void confirmer(char nom[100], int dd, int mm, int  yy, char sexe[100], char cin[100], char code[10]) {
	void retour1();
	char tabpassager[6][6] = {};
	int tabdate[20][3];
	int c, i = 0;
	printf("\t\t\t           |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||\n");
	printf("\t\t\t           ||||                     veuillez confirmer la reservation?                              ||||\n ");
	printf("\t\t\t           ||||                 1)oui, confirmer                                                    ||||\n");
	printf("\t\t\t           ||||                 2)non, annuler                                                      ||||\n");
	printf("\t\t\t           |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||\n");
	printf("========>votre choix : ");
	scanf_s("%d", &c);
	switch (c) {
	case 1:
		tabpassager[i][0] = nom[100];
		tabpassager[i][1] = sexe[100];
		tabpassager[i][2] = cin[100];
		tabpassager[i][3] = code[10];
		tabdate[i][0] = dd;
		tabdate[i][1] = mm;
		tabdate[i][2] = yy;
		i++;
		break;

	case 2:  system("cls"); retour1(); break;
	default: system("cls"); confirmer(nom, dd, mm, yy, sexe, cin, code); break;

	}


}

void option2() {
	//int affichepassager();
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


		//case 1: affichepassager();
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

	if (strcmp(a, "") != 0 && strstr(a, "1") == 0 && strstr(a, "2") == 0 && strstr(a, "3") == 0 && strstr(a, "4") == 0 && strstr(a, "5") == 0 && strstr(a, "6") == 0 && strstr(a, "7") == 0 && strstr(a, "8") == 0 && strstr(a, "9") == 0 && strstr(a, "0") == 0 && strstr(a, " ") == 0 && strlen(a) <= 20 && strstr(a, "*") == 0 && strstr(a, "-") == 0 && strstr(a, "_") == 0 && strstr(a, "/") == 0 && strstr(a, "_") == 0) {
		printf("nom valide :) \n");  return 1;
	}
	else {
		printf("Nom invalide :(   ****Verifiez le Nom (pas d'espace/de chiffre/de caractere speciaux!)*** \n");
		return 0;
	}

}
int verifsexe(char a[100]) {
	if (strlen(a) == 1 && ((strcmp(a, "M") == 0 || strcmp(a, "F") == 0 || strcmp(a, "m") == 0 || strcmp(a, "f") == 0)) && (strcmp(a, "") != 0 && strstr(a, "1") == 0 && strstr(a, "2") == 0 && strstr(a, "3") == 0 && strstr(a, "4") == 0 && strstr(a, "5") == 0 && strstr(a, "6") == 0 && strstr(a, "7") == 0 && strstr(a, "8") == 0 && strstr(a, "9") == 0 && strstr(a, "0") == 0 && strstr(a, " ") == 0))
	{
		printf("choix valide! :)\n");
		return 1;
	}

	else {
		printf("choix invalide! :(\n");  return 0;
	}

}

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
				printf("Date valide.:) \n");
				return 1;
			}
			else if ((dd >= 1 && dd <= 30) && (mm == 4 || mm == 6 || mm == 9 || mm == 11))
			{
				printf("Date valide :) .\n"); return 1;
			}
			else if ((dd >= 1 && dd <= 28) && (mm == 2))
			{
				printf("Date valide. :) \n");
				return 1;
			}
			else if (dd == 29 && mm == 2 && (yy % 400 == 0 || (yy % 4 == 0 && yy % 100 != 0)))
				printf("Date  valide. :) \n");
			else
			{
				printf("Le Jour est invalide. :( \n"); return 0;
			}
		}
		else
		{
			printf("le Mois est invalide :( \n"); return 0;
		}
	}
	else
	{
		printf("l'annee est invalide :( \n");
		return 0;
	}


}
int verifcin(char a[100]) {
	if (strlen(a) == 8 && (atoi(a) != 0))   //atoi(str) fait  la conversion du chaine  en numero
	{                                  //si str n'est pas une chaine numerique, atoi(str) retourne 0
		printf("numero de cin valide :)\n");
		return 1;
	}
	else {
		printf("numero de cin invalide :(   ***Verifier le Numero de CIN (8chiffres) ~ essayez un autre fois*** \n");
		return 0;
	}
}
int verifcode(char a[8]) {


	if (strlen(a) == 7 && isalpha(a[0]) && isdigit(a[1]) && isdigit(a[2]) && isdigit(a[3]) && isdigit(a[4]) && isdigit(a[5]) && isdigit(a[6])) {
		printf("numero du passport valide :)\n");
		return 1;
	}
	else {
		printf("numero du passport invalide :(   ***Verifiez  le Code du passport~ (commence par une lettre alphabetique et le reste du code est une serie de 6 chiffres)***   \n");
		return 0;

	}
}
// FONCTION QUI PERMET DE VERIFIT EST CE QUE LE VOL EST DISPO OU NN
int dispo(int numvol)
{
	
	int vol1, vol2, vol3, vol4, vol5;
	if (numvol==1 && vol1)
	{
		return 0; 
	}

	if (numvol == 2 && vol2)
	{
		return 0;
	}
	if (numvol == 3 && vol3)
	{
		return 0;
	}
	if (numvol == 4 && vol4)
	{
		return 0;
	}
	if (numvol == 5 && vol5)
	{
		return 0;
	}
	
}
// LA FONCTION POUR VERIFIER EST CE QUE LE NUMERO DE VOL EST VALIDE OU NON
int verifnumvol(int numvol)
{
	int dispo() ;
	if ((numvol <= 0 || numvol > 5))
	
		{	
		printf("num de vols n'existe pas"); 
	     }

    	  
	else
		if (dispo() == 0)

		{
			printf("le vol numero %d a ete choisit avec succees", numvol);
		}
		else
	{
		printf("il n'ya plus de places disponibles sur le vol numéro %d", numvol);
	}
		
	
	return 0; 
}
/*void affichepassager(char tabpassager[6][6], int tabdate[20][3]) {

	int	i = 0, j = 0;
	for (i = 0; i < 5; i++) {
		for (j = 0; j < 6; j++) {
			printf("\t\t\tNOM DU PASSAGER    SEXE    NUM CIN   CODE PASSORT   NUM DU VOL \n");
			printf("\t\t\t%s\t", tabpassager[i][j]);*/
			//}
		//}

	//}
//
int reserver()
{
	int getch(); system("cls");
	char nom[100]{};
	char sexe[100]{};
	int dd = 0, mm = 0, yy = 0,numvol;
	char cin[10]{};
	char code[10]{};
	int verifnumvol() ; 
	;
	color(12, 0);
	puts("==========================================Bienvenue au Fomulaire du reservation!========================================");
	getchar(); //getchar() empeche le programme de considerer l'appuie sur ENTREE comme un donnée à executer dans la boucle /HUH??
	//VERIF NOM
	do {
		printf("      => Veuillez donner le Nom et le prenom du passager: \n");
		gets_s(nom);
	} while (verifnom(nom) == 0);
	//VERIF DATE DE NAISSANCE
	do {
		printf(" => Veuiller Enter la date de naissance (sous la forme DD/MM/YYYY): ");
		scanf_s("%d/%d/%d", &dd, &mm, &yy);

	} while (verifdate(dd, mm, yy) == 0);
	getchar();
	//VERIF SEXE
	do {
		printf("=>Veuillez Entrer H (pour Homme) ou F (pour femme):  \n");
		gets_s(sexe);
		 
	} while (verifsexe(sexe) == 0);
	//VERIF NUMERO DE VOLS
	printf("entrer le numero de vol ");
	scanf_s("%d", &numvol);
	
    // VERIF CIN
	do {
		printf("=>Veuillez donner le numero de CIN : \n");
		gets_s(cin);
	} while (verifcin(cin) == 0);

	do {
		printf("=>Veuillez donner votre numero de passport\n");
		gets_s(code);
	} while (verifcode(code) == 0);
	if (verifnom(nom) == 1 && verifdate(dd, mm, yy) == 1 && verifsexe(sexe) == 1 && verifcin(cin) == 1 && verifcode(code) == 1)
		confirmer(nom, dd, mm, yy, sexe, cin, code);
	return 0;
}

void retour1() {
	int c;
	printf("\t\t\t              |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||\n");
	printf("\t\t\t              ||||                     veuillez retourner au ?                                         ||||\n ");
	printf("\t\t\t              ||||                 1)menu precedente                                                   ||||\n");
	printf("\t\t\t              ||||                 2)menu principale                                                   ||||\n");
	printf("\t\t\t              |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||\n");
	printf("========>votre choix : ");
	scanf_s("%d", &c);
	switch (c) {
	case 1: system("cls"); option3(); break;
	case 2: system("cls"); mainmenu(); break;
	default:system("cls"); retour1; break;
	}


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



