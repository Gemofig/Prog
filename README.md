#include <iostream>
using namespace std;

int main()
{
int a;
int *b;
	cout << "Rasmer massiva : ";
	cin>>a;
	b = new int [a];
for(int i=0; i<a; i++)
	{
	cout<<"b["<<i<<"] = ";
	cin >> b[i];
	}
for(int i=0; i<a; i++)
	cout <<b[i]<<" ";
	delete[] b;
return 0;
}
