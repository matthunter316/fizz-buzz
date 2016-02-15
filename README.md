# fizz-buzz
written in visual basic 2015

/*
Auther  : Matthew Hunter
Date    : 2/15/2016
Purpose : To print out numbers from 1 to 100. If the number
          is divisible 3 print "fizz" or if the number is 
		  divisible by 5 print "buzz" or if the number is 
		  both divisible by 3 and 5 print "fizz buzz" else
		  just print the number.
*/
#include <iostream>

using namespace std;

// Function prototypes
void print();

int main()
{	
	print();          // function call

	system("pause");  // pauses the screen for vb users
	return 0;
}

void print()
{
	// loop to print all the numbers
	for (int i = 1; i <= 100; i++)
	{
		// if the number is divisible by 3 and 5 
		// output "fizz buzz "
		if (i % 3 == 0 && i % 5 == 0)
		{
			cout << "fizz buzz " << endl;
		}

		// if the number is divisible by 5 
		// output "buzz "
		else if (i % 5 == 0)
		{
			cout << "buzz " << endl;
		}

		// if the number is divisible by 3  
		// output "fizz "
		else if (i % 3 == 0)
		{
			cout << "fizz " << endl;
		}

		// if the number is neither divisible by 3 of 5
		// output the number 
		else
			cout << i << endl;
	}
}
