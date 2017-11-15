// Funciones
//Id:222946
//Muñoz Serna J. Refugio

#include <stdio.h>
#include <stdlib.h>
#include <time.h>

void bienvenida(){
    printf("Bienvenido al barco! \n");
}

void navegarAlSur(int *x, int *y){
    printf("Navegando al SUR! \n");
    *x = *x+1;
    *y-=10;
}
void navegarAlnorte(int *x, int *y){
    printf("Navegando al NORTE! \n");
    *x = *x+1;
    *y+=10;
}
void navegarAleste(int *x, int *y){
    printf("Navegando al ESTE! \n");
    *x = *x+1;
    *y+=10;
}
void navegarAloeste(int *x, int *y){
    printf("Navegando al OESTE! \n");
    *x = *x-1;
    *y+=10;
}


void imprimirPosicion(int x, int y){
    printf("La posicion actual del barco es: %d, %d \n", x, y);
}

int main() {
    int x = 0;
    int y = 0;

    bienvenida();

    navegarAlSur(&x, &y);
     imprimirPosicion(x, y);
    navegarAlnorte(&x, &y);
     imprimirPosicion(x, y);
    navegarAleste(&x, &y);
     imprimirPosicion(x, y);
    navegarAloeste(&x, &y);
    imprimirPosicion(x, y);

    return EXIT_SUCCESS;
}
