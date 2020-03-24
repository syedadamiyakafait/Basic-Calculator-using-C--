# Basic Calculator using C++
 It performs 5 basic operations such as add, subtract, divide, multiply and power
#include<iostream>
using namespace std;
class calculator //simple calculator performing 5 basic operations
{
	private:
		int n1,n2;
		public:
			int add(int a, int b) //for addition
			{
				n1=a;
				n2=b;
				cout<<"Enter 2 numbers:"<<endl; //take input from users
				cin>>a>>b;
				cout<<"Answer:"<<endl;
				cout<<a<<"+"<<b<<"="<<a+b<<endl;
			}
			int subtract(int a, int b) // for subtraction
			{
				n1=a;
				n2=b;
				cout<<"Enter 2 numbers:"<<endl; //take input from users
				cin>>a>>b;
				cout<<"Answer:"<<endl;
				cout<<a<<"-"<<b<<"="<<a-b<<endl;
			}
			int multiply(int a, int b) // for multiplication
			{	
		  n1=a;
				n2=b;
				cout<<"Enter 2 numbers:"<<endl; //take input from users
				cin>>a>>b;
				cout<<"Answer:"<<endl;
				cout<<a<<"*"<<b<<"="<<a*b<<endl;
			}
			int divide(int a, int b) //for division
			{	
			 n1=a;
				n2=b;
				cout<<"Enter 2 numbers:"<<endl; //take input from users
				cin>>a>>b;
				cout<<"Answer:"<<endl;
				cout<<a<<"/"<<b<<"="<<a/b<<endl;
			}
			int power(int a, int b) // for power
			{
		  n1=a;
				n2=b;
			 int c=1;
			 cout<<"enter a number whose power is required:"<<endl;
    cin>>a;  //take input from users
    cout<<"enter a number, the number of times you want it to get multiplied:"<<endl;
	   cin>>b;
    for(int i=1;i<=b;i++)
        	{
	        	c=c*a;
        	}
			cout<<"value is:"<<c<<endl;
			}
};
main()
{
	calculator cal;
	int opt,a,b;
	cout<<"Enter number to get desired operation(1-5):"<<endl;
 cout<<"Enter 1 for addition."<<endl;
	cout<<"Enter 2 for subtraction."<<endl;
	cout<<"Enter 3 for multiplication."<<endl;
 cout<<"Enter 4 for division."<<endl;
 cout<<"Enter 5 for power."<<endl;
 cin>>opt;
	switch (opt)
	{
  case 1:
			cal.add(a,b);
		break;
		case 2:
			cal.subtract(a,b);
		break;
		case 3:
			cal.multiply(a,b);
		break;
		case 4:
			cal.divide(a,b);
		break;
		case 5:
		 cal.power(a,b);
		break;
		default:
			cout<<"Invalid operator."<<endl;
	    }
	return 0;
}
