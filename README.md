# PROGRAMACION_1
tareas programacion 

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
