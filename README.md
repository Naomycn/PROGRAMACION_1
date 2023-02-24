# PROGRAMACION_1
tareas programacion 
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
