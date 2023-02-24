# PROGRAMACION_1
tareas programacion 
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
											  
											.
	 //WHILE en githut

//Declaramos librerias
#include <iostream>

//Incluimos el espacio de nombres
int main() {
	
	//Declaramos la funcion principal Main
    int num, suma = 0, i = 0;
    
    std::cout << "Ingrese un número entero positivo: ";
    std::cin >> num;
    
    while (i <= num) {
        if (i % 2 == 0) {
            suma += i;
        }
        
        i++;
    }
    
    std::cout << "La suma de los números pares menores que " << num << " es: " << suma << std::endl;
    
    return 0;
}
												   .
												   //Do while ejercicio No.1

//Declaramos Libreria
#include <iostream>

//Incluimos el espacio de nombres
using namespace std;

//Declaramos la funcion principal Main
int main() {
    int num;
    int suma = 0;
    do {
        cout << "Ingresa un número (ingresa 0 para terminar): ";
        cin >> num;
        suma += num;
    } while (num != 0);
    cout << "La suma de los números ingresados es: " << suma << endl;
    return 0;
}

	.
	
	//Ejercicio no.1 de vectores

//Declaramos librerias
#include <iostream>
#include <vector>
//Incluimos el espacio de nombres
using namespace std;

//creamos nuestra funcion princpal main
int main() {
    vector<int> numeros; // Creamos un vector de enteros vacío
    int num;

    // Pedimos al usuario que ingrese 5 números enteros y los agregamos al vector
    for (int i = 1; i <= 5; i++) {
        cout << "Ingrese el número " << i << ": ";
        cin >> num;
        numeros.push_back(num);
    }

    // Mostramos los números ingresados por pantalla
    cout << "Los números ingresados son: ";
    for (int i = 0; i < numeros.size(); i++) {
        cout << numeros[i] << " ";
    }
    cout << endl;

    return 0;
}
		
		.
		
		//Ejercicio de Matriz 

//Declaramos las libreria necesarias 
#include <iostream>
#include <conio.h>

//Incluimos el espacio de nombres 
using namespace std;
//Creamos nuestra funcion principal Main 
int main(){
/*vamos a declarar una matriz de tipo entero pero como ejemplo vamos a 
asignarle 
tamanio maximo de [100][100] es decir 100 filas y 100 columnas*/
int dripCake[100][100];
/*Declarar 2 variables de tipo entero para poder guardar los valores de filas
y de columnas*/
int filas, columnas;
cout<<"Bienvenido al creador de Matriz"<<endl<<endl;
cout<<"Puede ingresar un maximo de 100 filas"<<endl;
cout<<"Y un maximo de 100 columnas"<<endl<<endl;
/*Debemos mostrarle al usuario un mensaje en el que se le indique que debe 
ingresar 
una cantidad de filas*/
cout<<"Ingresa la cantidad de filas que deseas:  ";
//Necesitamos almacenar el valor que el usuario ingrese en una variable
cin>>filas;
/*Debemos mostrarle al usuario un mensaje en el que se le indique que debe 
ingresar 
una cantidad de columnas*/
cout<<"Ingresa la cantidad de coumnas que deseas:  ";
//Necesitamos almacenar el valor que el usuario ingrese en una variable
cin>>columnas;
/*Necesitamos poder recorrer la matriz
y lo haremos haciendo uso de 2 Ciclos FOR uno para filas y otro para 
columnas*/
for(int i=0; i<filas; i++){
for(int j=0; j<columnas; j++){
/*Le pedimos al usuario que ingrese cada uno de los valores de la
matriz*/
cout<<"Digita por favor un numero:   ["<<i<<"],["<<j<<"]:  ";
cin>> dripCake[i][j];
}
}
/*Hacemos un recorrido con el ciclo FOR para poder traer los valores de la 
matriz
y poder de esta forma mostrarlos en pantalla */
for(int i=0; i<filas; i++){
for(int j=0; j<columnas; j++){
cout<<dripCake[i][j];
}
/*podemos agregar un salto de linea*/
cout<<"\n";
}
return 0;
}
