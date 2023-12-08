
# Commandes gcc

### -c

Compile le fichier passé en paramètre. Par défaut, le fichier de sortie s'appellera : **filename.o**

```bash

gcc  -c  filename.c

```

### -o

Change le nom de sortie du fichier compilé.

```bash

gcc  -c  filename.c  -o  filerename.o

```

### -lm

L'option **-lm** indique au compilateur de lier la bibliothèque mathématique

```bash

gcc  -c  filename.c  -o  filerename.o  -lm

```

  

# Explications globales c

### C est compilé, Pourquoi ?

Le c est compilé pour transformer le code source en langage machine.

  

C'est utile de compiler pour plusieurs raisons :

  

-  **Performance** : Un langage compilé est souvent très performant.

-  **Indépendance** : L'exécutable d'un programme peut être distribué sans que le code source ne soit livré avec.

-  **Compilation séparée** : Vous pouvez compiler plusieurs fichier .c en .o. Ces derniers peuvent ensuite être liés pour créer l'exécutable final.

  

### Quel code dans les fichiers .h

Les fichiers **h** sont des fichiers **header**. Ils contiennent généralement des déclarations de fonctions, des définitions de types de données, des constantes, des prototypes de fonctions...

```c

#ifndef EXEMPLE_H

#define EXEMPLE_H

// Déclaration d'une fonction
int additionner(int a, int b);

// Définition d'une constante
#define PI 3.14159

// Déclaration d'un type de données
typedef struct {
int x;
int y;
} Point;
  

#endif

```

### ifndef, define et endif

`#ifndef`, `#define`, et `#endif` sont des directives de préprocesseur qui évitent l'inclusion multiple du fichier d'en-tête.

  

### Quel code dans les fichiers .c

Les fichiers **c** sont des fichiers source. Ils contiennent généralement l'implémentation d'un **header**, des fonctions, des variables et des autres éléments déclarés dans les fichiers d'en-tête correspondants.

```c

// exemple.c
#include  "exemple.h"

// Implémentation de la fonction additionner
int  additionner(int  a, int  b) {
return a + b;
}

  

int  main() {
// Utilisation de la fonction additionner
int resultat = additionner(5, 3);

// Utilisation de la constante PI
double circonference = 2 * PI;

// Utilisation du type de données Point
Point point1;
point1.x = 10;
point1.y = 20;

return  0;
}

// Le reste de votre programme pourrait inclure d'autres fonctions, variables, etc.
// qui sont déclarées dans le fichier d'en-tête exemple.h.

```

# Réponses questions annales 2019-2020

### Question 2
Vous êtes sur une machine de 64 bits et vous utilisez également un système d’exploitation 64bits. Considérez les variables suivantes :
```c

#include  <string.h>
#include  <stdio.h>


int  main(int  argc, char **argv){
	char  message1[10] = "Bonjour";
	char *message2 = "Bonjour";

	printf("sizeof(char) : %li\n",sizeof(char));
	printf("sizeof(char *) : %li\n",sizeof(char *));
	printf("sizeof(char **) : %li\n",sizeof(char **));
	printf("sizeof(int **) : %li\n",sizeof(int **));
	printf("sizeof(message1) : %li\n",sizeof(message1));
	printf("strlen(message1) : %li\n",strlen(message1));
	printf("sizeof(message2) : %li\n",sizeof(message2));
	printf("strlen(message2) : %li\n",strlen(message2));
	
	return  1;
}
```
Sortie :
```
sizeof(char) : 1
sizeof(char *) : 8
sizeof(char **) : 8
sizeof(int **) : 8
sizeof(message1) : 10
strlen(message1) : 7
sizeof(message2) : 8
strlen(message2) : 7
```
  

### Question 4
Ecrivez un code complet en C dans le but de permuter les valeurs de deux variables. Votre code doit contenir les fichiers d'en-tête nécessaires, une fonction échange (…) et une fonction main. Le but de la fonction échange (…) est d’assurer la permutation des valeurs de deux variables. La fonction main doit appeler la fonction échange (…) et doit afficher les valeurs avant et après l'appel de la fonction
```c

#include  <string.h>
#include  <stdio.h>

int  main(){
	int variable1 = 46;
	int variable2 = 56;
	printf("%i\n%i\n",variable1,variable2);
	echange(&variable1,&variable2)
	printf("%i\n%i\n",variable1,variable2);
	return  1;
}

int  echange(int *variable1, int *variable2){
	int temp = *variable1;
	*variable1 = *variable2;
	*variable2 = temp;
	return  1;
}
```

### Question 5
Coder en C une structure de données Capteur qui comporte les éléments suivants : identifiant, temps, luminosité, pression, température, bâtiment. Les trois valeurs des mesures (luminosité, pression, température) doivent être des nombres flottants. L’élément bâtiment est la localisation de capteur, c’est-à-dire, le nom du bâtiment et son adresse. temps correspond à l'heure à laquelle les valeurs du capteur ont été obtenues. Instanciez une variable de cette structure.
fichier `test.h`

```c
#ifndef __TEST_H__
#define __TEST_H__
  
typedef struct {
	char *nom;
	char *adresse;
} Batiment;
 
typedef struct {
	int identifiant;
	int temps;
	float luminosite;
	float pression;
	float temperature;
	Batiment batiment;
} Capteur;
#endif
```

fichier `test.c`
```c
#include  "test.h"
#include  <string.h>
#include  <stdio.h>

int  main(){
	Batiment batiment;
	batiment.adresse = "une adresse";
	batiment.nom = "un nom";

	Capteur capteur;
	capteur.batiment = batiment;
	capteur.identifiant = 1;
	capteur.luminosite = 25.3;
	capteur.pression = 18.7;
	capteur.temperature = 27.8;
	capteur.temps = 18;
	return  1;
}

```

  

### Question 6

`10 % 3 = 1`

**%** représente le modulo (reste de la division entière). Ici 10 / 3 = 3 avec un reste de **1**.


`10 & 3 = 2`

**&** opération **AND** bit à bit. Ici 10 = 1010b et 3 = 0011b le AND donne donc **0010 = 2**.

`10 | 3 = 11`

**|** opération **OR** bit à bit. Ici 10 = 1010b et 3 = 0011b le OR donne donc **1011 = 11**.

`10 && 3 = 1`

**&&** opération **AND** logique. Deux nombre non nuls donne vrai donc **1**.

  

`10 || 3 = 1`

**||** opération **OR** logique. Un des deux nombres est non nul et donne vrai donc **1**.

  

`10 << 3 = 80`

**<<** "shift left" : Décale les bits vers la gauche.

10 en binaire = 1010 On ajoute 3 **0** à droite ce qui donne **1010000 = 80**

  

`10 / 3 = 3`

**/** opération de la division, ici entre deux entiers donc résulte une division entière. 10 / 3 = **3**

  

`10 ** 3`

L'opération **\*\*** n'existe pas en C, pour élever une valeur à une puissance, il faut utiliser **pow()** après avoir inclus la bibliothèque **<math.h>**.

  

### Question 7
Codez en C un programme qui prend des numéros (un ou plusieurs) passés par la ligne de commande. L’objectif de code est de :
- a) Trier les nombres par ordre croissant 
- b) Trier les nombres par ordre décroissant
  

```c

#include  <stdio.h>
#include  <stdlib.h>

int  comp (const  void * elem1, const  void * elem2)
{
	int f = *((int*)elem1);
	int s = *((int*)elem2);
	if (f > s) return  1;
	if (f < s) return -1;
	return  0;
}
int  main(int  argc, char* argv[])
{
	if(argc>1){
		int size = argc-1;
		int  x[size];
		for(int i = 1; i<argc; i++){
			x[i-1] = atoi(argv[i]);
		}
		qsort (x, sizeof(x)/sizeof(*x), sizeof(*x), comp);
		for (int i = 0 ; i < size ; i++)
			printf ("%d ", x[i]);
	}
	return  0;
}

```

  

### Question 8
Coder en C la fonction qui permet d’afficher les n premières et les n dernières lignes d’un fichier dont le nom de fichier et la valeur n sont passés par l’utilisateur en utilisant la ligne de commande. Pensez aux commandes head et tail en Linux dont l’objectif est d’afficher les n premières et les n dernières lignes d’un fichier. 
```c
#include  <stdio.h>
#include  <stdlib.h>
#include  <string.h>
int  main(char* argv[])
{
	char  head[1024];
	printf("%s premières lignes du fichier.\n",argv[2]);
	strcat(head, "head ");
	strcat(head, argv[1]);
	strcat(head, " -n ");
	strcat(head, argv[2]);
	system(head);
	printf("%s dernières lignes du fichier.\n",argv[2]);
	char  tail[1024];
	strcat(tail, "tail ");
	strcat(tail, argv[1]);
	strcat(tail, " -n ");
	strcat(tail, argv[2]);
	system(tail);
	printf("\n");
	return  0;
}
```


### Question 9

1. Fonction pour calculer le nombre de caractères dans une chaîne de caractères

```c
int compter_caracteres(const char *chaine) {
    int compte = 0;
    while (chaine[compte] != '\0') {
        compte++;
    }
    return compte;
}
```
2. Trouve la première occurrence d'une phrase dans une chaîne de caractères
```c
const char *trouver_premiere_occurrence(const char *chaine, const char *phrase) {
    const char *p1, *p2, *p3;
    if (*phrase == '\0') {
        return chaine;
    }

    for (p1 = chaine; *p1 != '\0'; p1++) {
        p2 = p1;
        p3 = phrase;
        while (*p2 == *p3 && *p3 != '\0') {
            p2++;
            p3++;
        }
        if (*p3 == '\0') {
            return p1;
        }
    }
    return NULL;
}

```
3. Trouve toutes les occurrences d'une phrase dans une chaîne de caractères.
```c
void trouver_toutes_occurrences(const char *chaine, const char *phrase) {
    const char *p = chaine;
    while (*p != '\0') {
        p = trouver_premiere_occurrence(p, phrase);
        if (p == NULL) {
            break;
        }
        printf("Trouvé à l'indice : %ld\n", (long)(p - chaine));
        p++; // Incrémenter p pour continuer la recherche
    }
}

```
