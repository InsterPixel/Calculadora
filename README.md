#include <iostream>
#include <cstdlib>
using namespace std;
void pausa();

int main()
{
	int num1, num2, suma, resta, multiplicacion, division;
	bool bandera = false;
	char tecla;
	do
	{
		system("color 12");
		system("cls");
		cin.clear();
		cout << "Calculadora" << endl;
		cout << "----------" << endl;
		cout << "Sumar (1)" << endl;
		cout << "Restar (2)" << endl;
		cout << "Multiplicar (3)" << endl;
		cout << "Dividir (4)" << endl;
		cout << "Salir (5)" << endl;
		cout << "Elije una opcion: ";
		cin >> tecla;
		switch (tecla)
		{
		case '1':
			system("cls");
			cout << "Has elejido Sumar" << endl;
			cout << "Cual es su primer cantidad a sumar?" << endl;
			cin >> num1;
			cout << "Cual es su segunda cantidad a sumar?" << endl;
			cin >> num2;
			suma = num1 + num2;
			cout << "La suma de sus numeros es; " << suma << endl;
			cout << "Pulsa una tecla para regresar... "<< endl;
			pausa();
			break;
		case '2':
			system("cls");
			cout << "Has elejido Restar" << endl;
			cout << "Cual es el numeros a restar?" << endl;
			cin >> num1;
			cout << "Cual es la cantidad a restar?" << endl;
			cin >> num2;
			resta = num1 - num2;
			cout << "La suma de sus numeros es; " << resta << endl;
			cout << "Pulsa una tecla para regresar... " << endl;
			pausa();
			break;
		case '3':
			system("cls");
			cout << "Has elejido Multiplicar" << endl;
			cout << "Cual es su primer cantidad a multiplicar?" << endl;
			cin >> num1;
			cout << "Cual es su segunda cantidad a multiplicar?" << endl;
			cin >> num2;
			multiplicacion = num1 * num2;
			cout << "La suma de sus numeros es; " << multiplicacion << endl;
			cout << "Pulsa una tecla para regresar... " << endl;
			pausa();
			break;
		case '4':
			system("cls");
			cout << "Has elejido Dividir" << endl;
			cout << "Cual es la cantidad a dividir?" << endl;
			cin >> num1;
			cout << "En cuantas cantidades se va a dividir?" << endl;
			cin >> num2;
			division = num1 / num2;
			cout << "La suma de sus numeros es; " << division << endl;
			cout << "Pulsa una tecla para regresar... " << endl;
			pausa();
			break;
		case '5':
			bandera = true;
			break;
		default:
			system("cls");
			cout << "Opcion no valida" << endl;
			cout << "Pulsa una tecla para regresar... " << endl;
			pausa();
			break;
		}
	} while (bandera != true);
	return 0;
}
void pausa()
{
	cout << "Pulsa una tecla para continuar...";
	getwchar();
	getwchar();
}
