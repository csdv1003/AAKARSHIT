AAKARSHIT



#include <iostream>
using namespace std;

// swap by using References in C++
void swap(int &x, int &y)
{
	// return if both variables data is same as we can't check for 
	// address of a reference
	if (x == y) 
		return;
	 
	x = x + y;	// Note - overflow might happen
	y = x - y;
	x = x - y;
}

// main function
int main()
{
	int x = 3, y = 4;
	swap(x, y);

	cout << x << " " << y;

	return 0;
}

