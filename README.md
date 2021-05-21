# Coding-interview-preparation

1. Time Complexity Of A Computer Program
2. How To Calculate Running Time?
3. Asymptotic Notations
  * BIG O
  * omega notation
  * Thetha notation



## IO manipulation

```
#include<iostream>
#include<iomanip>
using namespace std;

int main(){
	
	bool a = true;
	cout<<a<<"\n";
	cout<<std::boolalpha;
	cout<<a<<"\n";
	cout<<std::noboolalpha;
	cout<<a<<"\n";
	
	

	int b = 12, c= 33;
	cout<<b <<" "<<c<<"\n";
	
	cout<<std::hex;
	cout<<b <<" "<<c<<"\n";
	
	cout<<std::oct;
	cout<<b <<" "<<c<<"\n";
	
	cout<<std::dec;
	cout<<b <<" "<<c<<"\n\n\n";


	int d = 26;
	cout<<std::showbase;
	cout<<std::oct;
	cout<<d<<"\n";
	
	cout<<std::hex;
	cout<<d<<"\n";
	
	
	cout<<std::showpos;
	cout<<d<<"\n";
	
	cout<<std::uppercase;
	cout<<d<<"\n\n";
	
	
	int e = 12;
	cout<<std::dec;
	cout<<std::setw(5);
	cout<<std::setfill('*');	
	cout <<e<<"\n";
	
	cout<<std::left;
	cout<<std::setw(5);
	cout <<e<<"\n";
	
	

return 0;	
}
```

## C++ Preprocessors

Macros <br>
File Inclusion <br>
Conditional Compilation <br>
Other directives <br>


```
// { Driver Code Starts
//Initial Template for C++
#include <bits/stdc++.h>
#define MULTI(a,b) (a*b) //The multiplication macro function.
/*Whenever MULTI(a,b) is encountered, it is replaced by (a*b) during the preprocessing stage*/
using namespace std;

void macros(int a,int b);


 // } Driver Code Ends
//User function Template for C++

void macros(int a,int b)
{
    std::cout<< a * b;
    
    //See the macro defined at the top of the code. Use that macro to find a*b
    //Use only macro to complete this task
    
    cout<<endl;
}

// { Driver Code Starts.


int main() {
	int t;
	cin>>t;
	while(t--)
	{
	    int a,b;
	    
	    //Input a and b
	    cin>>a>>b; 
	    
	    //function call
	    macros(a,b);
	    
	}
	return 0;
}  // } Driver Code Ends
```

