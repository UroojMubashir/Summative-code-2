#include<iostream>
#include<math.h>
#include<string>
using namespace std;
int main()
{
	int number, fact = 1, Counter = 10;
	string name;
	cout << "Kindly Enter Your Full Name Here: ";
	getline(cin, name);
	cout << "Kindly Enter a Number Here: ";
	cin >> number;
	while (cin.fail())
	{
		cin.clear();
		cin.ignore(1000, '\n');
		cout << "Invalid Number\n Sorry! Try again: ";
		cin >> number;
	}
	for (int a = number; a > 0; a--)
	{
		fact *= a;
	}
	cout << "Factorial Of The Number You Choose Is: " << fact << endl;
	do
	{
		cout << number << " b " << Counter << " = " << number * Counter << endl;
		Counter--;
	} while (Counter > 0);
	for (int a = 10; a > 4; a--)
	{
		cout << number << " With The  Exponent Of " << a << " = " << pow(number, a) << endl;
	}
	return 0;
}
