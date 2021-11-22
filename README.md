# Table-till-10-for-loop
for loop
#include<iostream>
using namespace std;
int main()
{
	int table;   //declaring variables of datatype integer
	cout << "Table of : ";    
	cin >> table;

	while (cin.fail()!=0)  //if the users input is not an integer value then it will clear the input and will prompt the user to enter a valid number 
	{
		cin.clear();
		cin.ignore(1000, '\n');
		cout << "Invalid. Please enter a valid number : ";  //this message will display if the users input is not a number
		cin >> table;  //the users input will  be stored in variable table 
	}
	for (int k=1; k <= 10; k++)    //using for loop
	{
		cout << "\n" << table << " X " << k << " = " << table * k << endl;   //displaying the table on the console screen
		
	}
	return 0;
}
