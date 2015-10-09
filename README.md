/*# Mi-Ejemplo1
Aprendiendo a usar github*/

#include<stdio.h>
#include<conio.h>
void intercambia(int *,int *);//Prototipo de la funcion PUNTERO

int main(void){
	int x=2,y=3;
	printf("x= %d, y= %d\n",x,y);
	intercambia(&x,&y);  //Llamada a la funcion Le paso direccion de memoria
	printf("x= %d, y= %d\n",x,y);
}

void intercambia(int *x, int *y){ //Declaracion de la funcion * aqui es para decirle al programa que x and y son punteros que apuntan a un entero
	int aux;
	
	aux= *x;  //Los * aqui representan CONTENIDO de la dirreccion de memoria a la que apuntan los punteros
	*x=*y;    // "     "        "         "    
	*y=aux;   // "     "        "         "
}
