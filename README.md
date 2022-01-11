	#include <iostream> 
	#include <string>
	#include<cmath> 
	using namespace std;
	int menu() {
		cout << "Tea		Prices |Coffee		Prices(AED)" << endl;
		cout << "Iced Tea	3	Iced coffee		3	" << endl;
		cout << "Milk Tea	2	Milk coffee		2	" << endl;
		cout << "Black Tea	1	Black coffee		1	" << endl;

	} 
	int main()
	{
		int input;
		int money;
		float change1;
		char typeInput;
		menu();
		cout << "Would you like a tea or a coffee? Press T for tea and C for coffee." << endl;
		cin >> input;
		while(input!=C)
		if (input == 'C' && input == 'c')
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
				break;
			case 'M':
				cout << "You chose milk coffee that would be 2 AED, Please input your money." << endl;
				cin >> money;
				break;
			case 'B':
				cout << "You chose black coffee that would be 1 AED, Please input your money." << endl;
				cin >> money;
				break;
			}
		}
		else if(input=='T' && input == 't')
		{ 
			int change= money-
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
				break;
			case 'M':
			case 'm':
				cout << "You chose milk tea that would be 2 AED, Please input your money." << endl;
				cin >> money;
				break;
			case 'B':
			case 'b':
				cout << "You chose black tea that would be 1 AED, Please input your money." << endl;
				cin >> money;
				cout << "Your change is " <<change << endl;
				break;
			}
		}
		else {
			cout << "Incorrect command, Please Try Again" << endl;
		}

	}
