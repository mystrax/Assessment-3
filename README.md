	#include <iostream> 
	#include <string>
	#include<cmath> 
	using namespace std;
	void menu() {
		string menu[4][1] =
		{
		{"Tea		Prices |Coffee		Prices(AED)"},
		{"Iced Tea	3      |Iced coffee		3	"},
		{"Milk Tea	2      |Milk coffee		2	"},
		{"Black Tea	1      |Black coffee		1	"},
		};
		for (int i = 0;i < 4;i++) 
		{
			for (int j = 0;j < 1;j++)
				cout << menu[i][j] << endl;
		}
	}
	int main()
	{
		char input;
		int money;
		char typeInput;
		menu();
		cout << "Would you like a tea or a coffee? Press T for tea and C for coffee." << endl;
		cin >> input;
		while (cin.fail())
		cin.ignore(1000, '|n');
		cin.clear();
		cout << "Enter an input: " << endl;
			if (input == 'C' || input == 'c')
			{
				cout << "What type of coffee would you like?" << endl;
				cout << "Press the corresponding initial of the coffee that you like" << endl;
				cout << "I = Iced Coffee for 3 AED  | M = Milk Coffee for 2 AED | 3 = Black Coffee for 1 AED " << endl;
				cin >> typeInput;
				switch (typeInput)
				{
				case 'I':
					cout << "You chose iced coffee that would be 3 AED, Please input your money." << endl;
					cin >> money;
					cout << "Your change is: " << money - 3 << endl;
					cout << "Thank you for buying" << endl;
					break;
				case 'M':
					cout << "You chose milk coffee that would be 2 AED, Please input your money." << endl;
					cin >> money;
					cout << "Your change is: " << money - 2 << endl;
					cout << "Thank you for buying" << endl;
					break;
				case 'B':
					cout << "You chose black coffee that would be 1 AED, Please input your money." << endl;
					cin >> money;
					cout << "Your change is: " << money - 1 << endl;
					cout << "Thank you for buying" << endl;
					break;
				}
			}
			else if (input == 'T' || input == 't')
			{

				cout << "What type of tea would you like?" << endl;
				cout << "Press the corresponding initial of the coffee that you like" << endl;
				cout << "I = Iced Tea for 3 AED  | M = Milk Tea for 2 AED | B = Black Tea for 1 AED " << endl;
				cin >> typeInput;
				switch (typeInput)
				{
				case 'I':
				case 'i':
					cout << "You chose iced tea that would be 3 AED, Please input your money." << endl;
					cin >> money;
					cout << "Your change is: " << money - 3 << endl;
					cout << "Thank you for buying" << endl;
					break;
				case 'M':
				case 'm':
					cout << "You chose milk tea that would be 2 AED, Please input your money." << endl;
					cin >> money;
					cout << "Your change is: " << money - 2 << endl;
					cout << "Thank you for buying" << endl;
					break;
				case 'B':
				case 'b':
					cout << "You chose black tea that would be 1 AED, Please input your money." << endl;
					cin >> money;
					cout << "Your change is: " << money - 1 << endl;
					cout << "Thank you for buying" << endl;
					break;
				}
			}
			else {
				cout << "Please try again." << endl;
			}
		return 0;
	}
