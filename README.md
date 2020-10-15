#include <iostream>
using namespace std;

int main()
{
	float change = 0.00;
	int amount;
	char Products;

        cout << "\t\t\t-------------------------------------------------------------------" << endl;
        cout << "\t\t\tWELCOME TO THE STORE, WE HAVE VARIETY OF PRODUCTS TO CHOOSE FROM..." << endl;
        cout << "\t\t\t-------------------------------------------------------------------" << endl;
        cout << "\t\t\t[1] Noodles" << endl;
        cout << "\t\t\t[2] Corned Beef" << endl;
        cout << "\t\t\t[3] Ice Cream" << endl;
        cout << "\t\t\t[4] Soda" << endl;
        cout << "\t\t\t-------------------------------------------------------------------";
        cout << "\n\nWhat would you like to buy? ";
        cin >> Products;


	switch(Products)
	{
    case '1':
			cout << "------------------------------" << endl;
			cout << "Noodles is priced at PHP 10.00" << endl;
			cout << "------------------------------" << endl;
			cout << "Enter payment to proceed: ";
			cin >> amount;
				if (amount >= 10)
				{
					float change = amount - 10;
					cout << "\nTransaction Successful!";
					cout << "\nChange: " << change;
				}
				else
					cout << "\nPayment not sufficient...";
			break;

    case '2':
			cout << "----------------------------------" << endl;
			cout << "Corned Beef is priced at PHP 33.00" << endl;
			cout << "----------------------------------" << endl;
			cout << "Enter payment to proceed: ";
			cin >> amount;
				if (amount >= 33)
				{
					change = amount - 33;
					cout << "\nTransaction Successful!";
					cout << "\nChange: " << change;
				}
				else
					cout << "\nPayment not sufficient...";
			break;

    case '3':
			cout << "------------------------------" << endl;
			cout << "Ice Cream is priced at PHP 50.00" << endl;
			cout << "------------------------------" << endl;
			cout << "Enter payment to proceed: ";
			cin >> amount;
				if (amount >= 50)
				{
					change = amount - 50;
					cout << "\nTransaction Successful!";
					cout << "\nChange: " << change;
				}
				else
					cout << "\nPayment not sufficient...";
			break;

    case '4':
			cout << "------------------------------" << endl;
			cout << "Soda is priced at PHP 15.00" << endl;
			cout << "------------------------------" << endl;
			cout << "Enter payment to proceed: ";
			cin >> amount;
				if (amount >= 15)
				{
					change = amount - 15;
					cout << "\nTransaction Successful!";
					cout << "\nChange: " << change;
				}
				else
					cout << "\nPayment not sufficient...";
			break;

		default:
			cout << "\n\nERROR....";

	}
}
