fizz-buzz
written in visual basic 2015



Auther   Matthew Hunter
Date     2/15/2016
Purpose  To print out numbers from 1 to 100. If the number
          is divisible 3 print "fizz" or if the number is 
	  divisible by 5 print "buzz" or if the number is 
	  both divisible by 3 and 5 print "fizz buzz" else
	  just print the number.


include <iostream>
using namespace std;

void print();

int main()
{	
	print();           

	system("pause");   
	return 0;
}

void print()
{
	for (int i = 1; i <= 100; i++)
	{

		if (i % 3 == 0 && i % 5 == 0)
		{
			cout << "fizz buzz " << endl;
		}
		else if (i % 5 == 0)
		{
			cout << "buzz " << endl;
		}
		else if (i % 3 == 0)
		{
			cout << "fizz " << endl;
		} 
		else
			cout << i << endl;
	}
}
