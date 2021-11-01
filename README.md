# SUMMATIVE ASSESSMENT 1 

    #include <iostream>
    #include <string>
    using namespace std;
    int main()
    {
	int age;
	int loc;
	string name;
	string yn;
	bool confirm;

	cout << "Thank you for using our service! \n";
	cout << "Please enter the name of the student and age. \n";

	getline(cin, name);
	cout << "Please enter your age \n";
	cin >> age;

	if (std::cin.fail())
	{
		std::cin.clear();
		std::cin.ignore(std::numeric_limits<std::streamsize>::max(), '\n');
		std::cout << "Incorrect command\n: ";
	}
	if (age >= 1)
	{
		cout << "Welcome to the school transportation service. \n";
		cout << "Would you like to avail your student for transporation? (Y/N)\n";
		cin >> yn;

		if (yn == "y" || yn == "Y")
		{
			confirm = true;
			if (confirm == true)
			{

				cout << " \n Where are you located? Prices are charged monthly \n";
				cout << "[1] Abu Dhabi (1000 AED) \n";
				cout << "[2] Sharjah (500 AED) \n";
				cout << "[3] Ajman (390 AED) \n";
				cout << "[4] Dubai (650 AED) \n";
				cout << "[5] Ras Al Khaiman (250 AED) \n";
				cout << "[6] Umm Al Quwain (300 AED) \n";
				cout << "[7] Fujairah (300 AED) \n";
				cout << "[8] Al Ain (1000 AED) \n";

				cin >> loc;

				switch (loc) {
				case 1:
					cout << name << ". Location: Abu Dhabi. 1000 AED/Month \n";
					cout << "Thank you for using our service! \n";
					break;
				case 2:
					cout << name << ". Location: Sharjah. 500 AED/Month \n";
					cout << "Thank you for using our service! \n";
					break;
				case 3:
					cout << name << ". Location: Ajman. 390 AED/Month \n";
					cout << "Thank you for using our service! \n";
					break;
				case 4:
					cout << name << ". Location: Dubai. 650 AED/Month \n";
					cout << "Thank you for using our service! \n";
					break;
				case 5:
					cout << name << ". Location: Ras Al Khaimah. 250 AED/Month \n";
					cout << "Thank you for using our service! \n";
					break;
				case 6:
					cout << name << ". Location: Umm Al Quwain 300 AED/Month \n";
					cout << "Thank you for using our service! \n";
					break;
				case 7:
					cout << name << ". Location: Fujairah. 300 AED/Month \n";
					cout << "Thank you for using our service! \n";
					break;
				case 8:
					cout << name << ". Location: Al Ain. 1000 AED/Month \n";
					cout << "Thank you for using our service! \n";
					break;
				default:
					cout << "Please select only the given selection \n";
				}


			}
		}
		else if (yn == "N" || yn == "n")
			confirm = false;
		{

			cout << "Thank you for using our service!\n";
		}

		return 0;
	}
}
