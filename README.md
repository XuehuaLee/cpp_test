# cpp_test

`#include <iostream>

using namespace std;

int main()

{

	double x;
  
	cout << "Enter Value:";
  
	while( !(cin >> x))
  
	{
  
		cout << "Bad input. Please enter a number:";
    
		cin.clear();
    
		while(cin.get() != '\n')
    
			continue;
      
	}
  
	cout << "Value =" << x << endl;
  
	return 0;
  
}`

* 不使用using编译指令和using声明
`#include <iostream>

//using namespace std;

int main()

{

	double x;
  
	std::cout << "Enter Value:";
  
	while( !(std::cin >> x))
  
	{
  
		std::cout << "Bad input. Please enter a number:";
    
		std::cin.clear();
    
		while(std::cin.get() != '\n')
    
			continue;
      
	}
  
	std::cout << "Value =" << x << std::endl;
  
	return 0;
  
}`

* 不使用using编译指令，使用using声明
`#include <iostream>

//using namespace std;

int main()

{  

	using std::cout;
  
	using std::cin;
  
	using std::endl;
  
	double x;
  
	cout << "Enter Value:";
  
	while( !(cin >> x))
  
	{
  
		cout << "Bad input. Please enter a number:";
    
		cin.clear();
    
		while(cin.get() != '\n')
    
			continue;
      
	}
  
	cout << "Value =" << x << endl;
  
	return 0;
  
}
`
