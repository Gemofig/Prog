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



http://www.cyberforum.ru/cpp-beginners/thread83916.html
https://code-live.ru/post/cpp-functions/





#include <iostream>
#include <string>

using namespace std;

void check_pass (string password)//Название в скобках можно выставить любое
{
    string valid_pass = "qwerty123";
    if (password == valid_pass) { // Проверка пароля (равны ли valid_pass и password ?)  
        cout << "Dostup" << endl;
    } else {
        cout << "Pschol von" << endl;
    }
}

int main()
{    
    string user_pass;
    cout << "Parol ?: ";
    getline (cin, user_pass);
    check_pass (user_pass);//Вызывает первую функцию void check_pass (string password) (ЕЁ МОЖНО ВЫЗЫВАТЬ БЕССКОНЕЧНО)
    return 0;
}
