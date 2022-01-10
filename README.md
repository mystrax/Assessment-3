	#include <iostream> 
	#include <string>
	using namespace std;
	int change(int money) 
	{

	}
	int main()
	{
		int input;
		int money;
		char typeInput;
		char T, t, C, c;
		cout << "Would you like a tea or a coffee? Press T for tea and C for coffee." << endl;
		cin >> input;
		if (input== C && input == c)
		{
			cout << "What type of coffee would you like?" << endl;
			cout<<	"Press the corresponding initial of the coffee that you like" << endl;
			cout<<	"1 = Iced Coffee for 3 AED  | 2 = Milk Coffee for 2 AED | 3 = Black Coffee for 1 AED " << endl;
			cin >> typeInput;
			switch (typeInput)
			{
				case 1:
					cout << "You chose iced coffee that would be 3 AED, Please input your money." << endl;
					cin >> money;
					change();

			}


		}
		else if
		{
			cout << "What type of tea would you like?" << endl;
			cout << "Press the corresponding initial of the coffee that you like" << endl;
			cout << "I = Iced Tea for 3 AED  | M = Milk Tea for 2 AED | B = Black Tea for 1 AED " << endl;
			cin >> typeInput;
		}
		else {
			cout << "Incorrect command, Please Try Again" << endl;
		}
	}
