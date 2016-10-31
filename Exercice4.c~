#include <stdio.h>
#include <stdlib.h>

#define TAILLEMAX 10

/*Hello world*/

void transposeMatrice (int a[][TAILLEMAX], int taille);

void affiche_vecteur_int(int[], int);

void affiche_matrice_int(int tab[][TAILLEMAX], int);

int main(void){
  int a[3][TAILLEMAX] = {{1,2,3},{4,5,6},{7,8,9}};
  
  affiche_matrice_int(a, 3);
  
  transposeMatrice (a, 3);
  
  printf("\n\n");
  affiche_matrice_int(a, 3);
  
  printf("\n");
  int b[4][TAILLEMAX] = {{1,2,3,4},{5,6,7,8},{9,10,11,12},{13,14,15,16}};
  
  printf("\n");
  affiche_matrice_int(b, 4);
  
  transposeMatrice (b, 4);
  
  printf("\n");
  affiche_matrice_int(b, 4);
  
  return EXIT_SUCCESS;
}

void transposeMatrice (int a[][TAILLEMAX], int taille){
  int i, j, n;
  for(i = 0; i < taille; i++){
    for(j = i; j < taille; j++){
      n = a[i][j];
      a[i][j] = a[j][i];
      a[j][i] = n;
    }
  }
}

void affiche_vecteur_int(int tab[], int taille){
  int i;
  
  for(i = 0; i < taille; i++){
    printf("%4d", tab[i]);
  }
  
  printf("\n");
}

void affiche_matrice_int(int tab[][TAILLEMAX], int taille){
  int i;
  
  for(i = 0; i < taille; i++){
    affiche_vecteur_int(tab[i], taille);
  }
}
