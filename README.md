# PROGRAMACION_1
tareas programacion 
/*Programa que solicite al usuario ingresar el tamaño de un array multidimensional. 
El usuario deberá poder ingresar los valores y asignarlos al array. 
Luego el programa deberá mostrar al usuario el resultado de la suma y multiplicación de los 2 arrays.*/

//Declaramos libreria
#include<iostream>
#include<conio.h>

//Incluimos el espacio de nombres
using namespace std;

//Declaramos la funcion principal Main
int main(){
	
	int numeros[100];
	int suma = 0;
	int multiplicacion = 1;
	int f;
	
cout<<" Bievenido al programa de suma y multiplicacion de 2 Arrays!  ";	
cout<<"\n-----------------------------------------------------------  ";	
cout<<"\nIngresa la cantidad de arreglos que desea ingresar -->  ";
cin>>f;
	
	//Sirve para llenar los valore
	for(int i=0;i<f;i++){	
	
	
	//Sirve para llenar los valores de los arrays
		cout<<"Por Favor ingrese los datos del arreglo ["<<i<<"]";
		cin>>numeros[i];
		}
	
	

	for(int i=0;i<f;i++){
		//Declaramos para hacer la suma de los arrays
		suma += numeros[i];
		//Declaramos para hacer la multiplicacion de los arrays
		multiplicacion *= numeros[i];
		
	}
	
	
	
	cout<<"la suma de los arrays ingresados es de:  "<<suma<<endl;
	cout<<"la multiplicacion de los arrays ingresados es de:  "<<multiplicacion<<endl;
}
