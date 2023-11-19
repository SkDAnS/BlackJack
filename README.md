# BlackJack


En-têtes


#include <stdlib.h> // Pour pouvoir utiliser exit()
#include <stdio.h>	// Pour pouvoir utiliser printf()
#include <math.h>	// Pour pouvoir utiliser sin() et cos()
#include "GfxLib.h" // Seul cet include est necessaire pour faire du graphique
#include "BmpLib.h" // Cet include permet de manipuler des fichiers BMP
#include "ESLib.h"	// Pour utiliser valeurAleatoire()
#include <string.h>
#include <time.h>
#include <unistd.h>

#include "moteur.h"
#include "fonctions.h"
#include "settings.h"
Ces directives #include permettent d'inclure des fichiers d'en-tête nécessaires au programme, tels que des bibliothèques standard (stdlib, stdio, math, etc.) et des fichiers d'en-tête locaux (GfxLib.h, BmpLib.h, ESLib.h, moteur.h, fonctions.h, settings.h).

Variables globales


static int variableboutonf2unef = 0;
Déclaration d'une variable globale statique variableboutonf2unef.

Fonction gestionEvenement


void gestionEvenement(EvenementGfx evenement);
Définition de la fonction gestionEvenement qui gère les événements graphiques.

Fonction main


int main(int argc, char **argv) {
    // ...
    initialiseGfx(argc, argv);
    // ...
    lanceBoucleEvenements();
    return 0;
}
Fonction principale main du programme. Elle initialise la bibliothèque graphique GfxLib, prépare la fenêtre graphique, puis lance la boucle principale d'événements.

Variables globales externes
c

extern int nbr;
extern int nbrInitial;
// ... (d'autres variables externes)
Déclarations d'un ensemble de variables globales externes, probablement définies dans d'autres fichiers source.


Cela concerne seulement le main

