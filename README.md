// Галимов Арсен 219/3
#include <iostream>
using namespace std;

void main() {
	setlocale(LC_ALL, "ru");

	double x, y;
	cout << "Введите координаты точки: ";
	cin >> x >> y;
	if ((y > 0.5) && (x*x + y * y > 1))
		cout << "Точка принадлежит области";
	else if ((y < 0.5) || (x*x + y * y < 1))
		cout << "Точка не принадлежит области";
	else cout << "Точка лежит на границе области";
}
