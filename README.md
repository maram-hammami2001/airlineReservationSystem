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
    printf("        bbbbbbbb                                                                                                                                                              \n");
    printf("        b::::::b              iiii                                                                                                                                        !!!\n");
    printf("        b::::::b             i::::i                                                                                                                                      !!:!!\n");
    printf("        b::::::b              iiii                                                                                                                                       !:::!\n");
    printf("        b:::::b                                                                                                                                                         !:::!\n");
    printf("        b:::::bbbbbbbbb    iiiiiii     eeeeeeeeeeee    nnnn  nnnnnnnn vvvvvvv           vvvvvvv eeeeeeeeeeee    nnnn  nnnnnnnn    uuuuuu    uuuuuu      eeeeeeeeeeee    !:::!\n");
    printf("        b::::::::::::::bb  i:::::i   ee::::::::::::ee  n:::nn::::::::nnv:::::v         v:::::vee::::::::::::ee  n:::nn::::::::nn  u::::u    u::::u    ee::::::::::::ee  !:::!\n");
    printf("        b::::::::::::::::b  i::::i  e::::::eeeee:::::een::::::::::::::nnv:::::v       v:::::ve::::::eeeee:::::een::::::::::::::nn u::::u    u::::u   e::::::eeeee:::::ee!:::!\n");
    printf("        b:::::bbbbb:::::::b i::::i e::::::e     e:::::enn:::::::::::::::nv:::::v     v:::::ve::::::e     e:::::enn:::::::::::::::nu::::u    u::::u  e::::::e     e:::::e!:::!\n");
    printf("        b:::::b    b::::::b i::::i e:::::::eeeee::::::e  n:::::nnnn:::::n v:::::v   v:::::v e:::::::eeeee::::::e  n:::::nnnn:::::nu::::u    u::::u  e:::::::eeeee::::::e!:::!\n");
    printf("        b :::::b     b:::::b i::::i e:::::::::::::::::e   n::::n    n::::n  v:::::v v:::::v  e:::::::::::::::::e   n::::n    n::::nu::::u    u::::u  e:::::::::::::::::e !:::!\n");
    printf("        b:::::b     b:::::b i::::i e::::::eeeeeeeeeee    n::::n    n::::n   v:::::v:::::v   e::::::eeeeeeeeeee    n::::n    n::::nu::::u    u::::u  e::::::eeeeeeeeeee  !!:!!\n");
    printf("        b:::::b     b:::::b i::::i e:::::::e             n::::n    n::::n    v:::::::::v    e:::::::e             n::::n    n::::nu:::::uuuu:::::u  e:::::::e            !!! \n");
    printf("        b:::::bbbbbb::::::bi::::::ie::::::::e            n::::n    n::::n     v:::::::v     e::::::::e            n::::n    n::::nu:::::::::::::::uue::::::::e               \n");
    printf("        b::::::::::::::::b i::::::i e::::::::eeeeeeee    n::::n    n::::n      v:::::v       e::::::::eeeeeeee    n::::n    n::::n u:::::::::::::::u e::::::::eeeeeeee   !!! \n");
    printf("        b:::::::::::::::b  i::::::i  ee:::::::::::::e    n::::n    n::::n       v:::v         ee:::::::::::::e    n::::n    n::::n  uu::::::::uu:::u  ee:::::::::::::e  !!:!!\n");
    printf("        bbbbbbbbbbbbbbbb   iiiiiiii    eeeeeeeeeeeeee    nnnnnn    nnnnnn        vvv            eeeeeeeeeeeeee    nnnnnn    nnnnnn    uuuuuuuu  uuuu    eeeeeeeeeeeeee   !!! \n");
    color(8, 0);
    printf("\n");
    printf("                                 Veuillez appuyer sur entrer pour continuer!\n");
    getchar();
}
int mainmenu()
{
    void option1();
    void option2();
    void option3();
    void quitter();
    int c;
    color(6, 0);
    puts("\t\t\t\t                   *******************************************************************");
    puts("\t\t\t\t                   *                  BIENVENUE DANS NOTRE SYSTEME                   *");
    puts("\t\t\t\t                   *                     DE RESERVATION DE VOL!                      *");
    puts("\t\t\t\t                   *******************************************************************");
    color(4, 0);
    printf("\t\t                     votre options:\n");
    puts("\t\t\t                                ****************************************");
    printf("\t\t\t                              * 1)Gestionnaire des vols     \t         *\n");
    printf("\t\t\t                              * 2)Gestionnaire des passagers\t         *\n ");
    printf("\t\t\t                              * 3)Gestion des reservation   \t         *\n");
    printf("\t\t\t                              * 4) Quitter \t                         *\n");
    puts("\t\t\t                                ****************************************");
    printf("Veuillez donner votre choix:");
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
    case 4:   quitter();

        break;

    default:
        int getch(); system("cls");
        printf("\t\t\t<Choix invalide! veuillez donner un autre choix>\n");
        mainmenu();
        break;
    };



    return 0;


}









void option1() {
    int getch();
    system("cls");
    int c;
    void affiche1();

    color(14, 0);
    puts("===============================================GESTIONNAIRE DE VOLS!====================================================");
    printf("\t\tvotre options:\n");
    puts("\t\t\t  ///////////////////////////////////////////");
    printf("\t\t\t // 1.Afficher la liste des vols           //\n");
    printf("\t\t\t // 2.Afficher  les places valables        //\n");
    printf("\t\t\t //  et nonvalable dans chaque vol         //\n");
    printf("\t\t\t // 2.Afficher  les places valables        //\n ");
    printf("\t\t\t // et non valable dans chaque vol         //\n ");
    printf("\t\t\t // 4.Retour au menu principale            //\n");
    puts("\t\t\t  /////////////////////////////////////////////");
    printf("\t\t\t\t\t\tVeuillez donner votre choix:");
    scanf_s("%d", &c);
    switch (c) {
    case 1: affiche1(); break;
    case 4: int getch(); system("cls"); mainmenu(); break;


    }
}
void affichepassager() {


}


void option2() {
    int c;
    int getch();
    system("cls");
    color(9, 0);
    puts("===============================================GESTIONNAIRE DE PASSAGERS!===============================================");
    puts("\t\tvotre options:\n");
    puts("\t\t\t  ///////////////////////////////////////////");
    printf("\t\t\t // 1)Liste des passagers                  //\n");
    printf("\t\t\t // 2) chercher un passager                //\n ");
    printf("\t\t\t // 3) modifier les informations           //\n ");
    printf("\t\t\t //  du passager                           //\n ");
    printf("\t\t\t // 4) Supprimer un passager               //\n ");
    printf("\t\t\t // 5) Retour au menu principale           //\n");
    puts("\t\t\t  //////////////////////////////////////////");
    printf("Veuillez donner votre choix:");
    scanf_s("%d", &c);
    switch (c) {


    case 1: affichepassager();
    case 5:int getch(); system("cls"); mainmenu(); break;
    default:
        int getch(); system("cls");
        puts("\t\t\t<Choix invalide! veuillez donner un autre choix>\n");
        option2();
        break;
    }
}
void option3() {
    void reserver();
    int getch();
    system("cls");

    int c;
    color(13, 0);
    puts("==========================================Reservation de vol!====================================================");
    printf("\t\tvotre options:\n");
    puts("\t\t\t  ///////////////////////////////////////////");
    printf("\t\t\t // 1)Veuillez voyager? Reserver votre     //\n");
    printf("\t\t\t //    place maintenant!                   //\n");
    printf("\t\t\t // 2) Retour au menu principale           //\n");
    puts("\t\t\t  //////////////////////////////////////////");
    printf("\tVeuillez donner votre choix:");
    scanf_s("%d", &c);
    switch (c) {
    case 1: reserver(); break;
    case 2: int getch(); system("cls"); mainmenu(); break;
    }
    ;
}

void reserver() {
    int getch(); system("cls");
    char nom[11]{};
    int result = 0;
    color(12, 0);
    puts("==========================================Bienvenue au Fomulaire du reservation!========================================");

    do {
        printf("==>Veuillez donner votre Nom:");
        gets_s(nom);
        result = isspace(*nom);
    } while (!(result == 0 && strlen(nom) >= 10));



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
void affiche1() {
    int getch();
    system("cls");

    color(4, 10);
    puts("\t\t\t||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||");
    puts("\t\t\t|                                     Liste des Vols                                 |");
    puts("\t\t\t||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||");

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

    printf("Apuyer  sur le keyboard pour le retour au menu precedent");

}

int main()
{
    bienvenue();
    int getch();
    system("cls");
    mainmenu();

    return 0;
}
