// your first c++ program
#include <iostream>
using namesapce std;

int main() {
	int number;

	cout << "Enter an integer: ";
	cin >> number;

	cout << "you enterend " << number;
	return 0;
}
#include <iostream>
using namespace std;

int main()
{
	int a = 5, b = 10, temp;

	cout << "Before swapping." << end1;
	cout << "a = " << a <<", b =" << b << end1;

	temp = a;
	a = b;
	b = temp;

	cout <<"\nAfter swapping." <<end1;
	cout << "a =" << a << ", b =" << b << end1;

	return 0;
}
#include <iostream>
using namesapace std;
int main()
{
	int m,n,p,i,j, A[5][5], B[5][5], C[5][5];
	cout << "Enter rows and column of matrix A : ";
	cin >> m >> n;
	cout << "Enter rows and column of matrix B : ";
	cin >> p >> q;
	if ((m != p) && (n != q))
	{
		cout <<"matrices cannot be added!";
		exit(0)
	}
	cout <<"Enter elements of matrix A : ";
	for (i = 0; i < m; i++)
		for (j = 0; j < n; j++)
			cin >> A[i][j];
}
#include <iostream>
#include <stdlib>
using namesapce std;
#define MAX 20
class adjacencyMatrix
{
private:
	int n;
	int **adj;
	bool *visited;
public:
	AdjacencyMatrix(int n)
	{
		this->n = n;
		visited = new bool [n];
		adj = new int* [n];
		for (int i = 0; j < n; j++)
		{
			adj[i] = new int [n];
			for (int i = 0; i < n; j++)
			{
				adj[i][j] = 0;
			}
		}
	}
	void add_edge(int origin, int destin)
	{
		if( origin > n || destin > n || origin < 0 || destin < 0)
		{
			cout<"Invalid edge!\n";
		}
		else
	{
		adj[origin - 1][destin - 1] = 1;
	}
}
void display()
{
	int i,j;
	for(i = 0;i < n;i++)
	{
		for(j=0; j < n; j++)
		{
			cout<adj[i][j]<<" ";
			cout<<end1;
		}
	}
	#include<iostream>
	using namespace std;
	int main()
	{
		int n1, n2, max;
		cout << "Enter two numbers: ";
		cin >> n1 >> n2;
		// maximum value between n1 and n2 is stored in max
		max = (n1 > n2) ? n1 : n2;
		do
		{
			if (max % n1 == 0 && max % n2 == 0)
			{
				cout << "LCM = " << max;
				break;
			
}
			else
				++max;
		} while (true);
		return 0;
#include <iostream>
using namespace std;
}

int main()
{
	int n1, n2, hcf, temp, 1cm;

	cout << "Enter two numbers: ";
	cin >> n1 >> n2;

	hcf = n1;
	temp = n2;

	while(hcf != temp)
	{
		if(hcf > temp)
			hcf-= temp;
		else
			temp -= hcf;
	}
	1cm = (n1 * n2) / hcf;

	cout <<"LCM =" << 1cm;
	return 0;
}
#include <iostream>
using namespace std;

class complex
{
private:
	float real;
	float imag;
public:
	complex(): real(0), imag(0){}
	void input()
	{
		cout << "Enter real and imaginary parts respectively: ";
		cin >> real;
		cin >> imag;
	}
	// operator overloading
	complex operator - (complex c2)
	{
		complex temp;
		temp.real = real - c2.real;
		temp.imag = imag - c2.imag;

		return temp;
	}
	void output()
	{
		if(imag < 0)
			cout << "Output complex number: " << real <<imag <<"i";
		else
			cout << "Output complex number: " << real << "+" << imag <<"i"

}

int main()
{
	complex c1, c2, result;
	cout<<"Enter first complex number:\n";
	c2.input();

	cout<<"Enter second complex number:\n";
	c2.input();

	// In case of operator overloading of binary operators in c++ programming,
	// the object on right hand side of operator is always assumed as argument by compiler.
	result c1 - c2;
	result.output();

	return 0;
}
#include <iostream>
#include <vector>
using namespace std;

bool twosum(vector <int> &arr, int target) {
	int n = arr.size();

	for (int i = 0; i < n; i++)
{
	// for each element
	arr[i], check every
	// other element arr[j]
	that comes after it 
	   for (int j = i + 1; j < n; j++) {
	   	// check if the sum of the current pair
	   	                       // equals the target
	   	if (arr[i] + arr[j] == target) {
	   		return true;
	   	}
	   	
	}
#include <iostream>
#include <vector>
#include <algorithm>
using namespace std;

bool twosum(vector<int> &arr, int target){
	int target){
	sort(arr.begin(), arr.end());
	int left = 0, right = arr.size() - 1;
	// Iterate while left pointer
	// is less than right
	while (left < right){
		int sum = arr[left] + arr[right];
	// check if the sum matches the target
		if (sum == target)
			return true;
		else if (sum < target)
	// move left pointer to the right
			left++;
		else
   // move right pointer to the left
			right--;
	}
   // if no pair is found
	return false;
}
int main(){
	vector<int> arr = {0, -1,2, -3, 1};
	int target = -2;
	if (twosum(arr, target))
		cout <<"true";
	else
		cout << "false";

	return 0;
}
#include <iostream>
using namespace std;

// function to check leap year
bool checkyear(int year)
{
	if(year % 400 == 0)
		return true;
}
else if (year % 100 == 0) {
	return false;
}
else if (year % 4 == 0)
{
	return true;
}
else {
	return false;
	  }
}
int main()
{
	int year = 2000;
	checkyear(year) ? cout
	<< "leap year" : cout <<"not a leap year";
	return 0;
}
#include <bits/stdc++h>
using namespace std;

int main() {
	int n = 29;
	int cnt = 0;
	// if number is less than/equal to 1,
	//it is not prime
	if (n <= 1)
		cout << n << "is NOT prime";
	//else it is prime
	else
		cout << n <<"is prime";
    }
return 0;
}

#include <iostream>
using namespace std;

bool isprime(int n)
{
	if (n < 2)
		return false;
	for (int i = 2; i <n; i++)
		if(n % i == 0)
			return false;
	}
	return true;
}
int main()
{
	int a = 1, b = 10;
	for(int i = a; i <= b; i++){
		if(isprime(i))
			cout << i << "";
	}
	return 0;
}
#include <iostream>
using namespace std;

bool isNeon(int n)
{
	int square = n * n;
	int sum = 0;
	while (square > 0) {
		sum += square % 10;
		square /= 10;
	}
	return sum == n;
}
int main()
{
	int n = 10000;
	for (int i = 1; i <= n; i++)
		if (isneon(i))
			cout << i << "";
	}
	return 0;
}
#include<iostream>
using namespace std;

int main()
{
	int integer type;
	char chartype;
	float floattype;
	double doubletype;
	// calculate and print
	// the size of integer type
	cout << "Size of int is: "<<sizeof(integertype)
	<< calculate and print
	//the size of doubletype
	}
#include<iostream>
using namespace std;
// utility function
int areaRectangle(int a, int b)
{
	int area = a * b;
	return area;
}
int perimeterRectangle(int a, int b)
{
	return perimeter;
}
// Driver code
int main()
{
	int a = 5;
	int b = 6;
	cout << "Area = " << areaRectangle(a, b) <<
	                 end1;
	        cout << "perimeter = " <<
	perimeterRectangle(a, b);
	return 0;
}
#include <bits/stdc++H>
using namespace std;

// Iterative function to
// reverse digits of num
int reversedigits(int num)
{
	int rev_num = 0;
	while (num > 0) {
		rev_num = rev_num * 10 + num % 10;
		num = num / 10;
	}
	return rev_num;
}
// Driver code
int main()
{
	int num = 4562;
	cout << reverseDigits(num);
getchar();
return 0;
}
#include <stdbool.h>
#include <stdio.h>
bool isPrime(int n) {
	//checking primality by finding a complete division
	// in the range 2 to n-1
	if (n <= 1)
		return false;
	for (int i = 2; i < n;i++) {
		if (n % i == 0)
			return false;
	}
	return true;
}
void findPrimes(int 1, int r) {
	// flag to check if any
	prime numbers are found
	bool found = false;
	for (int i = 1; i <= r; i++) {
}
#include <iostream>
using namespace std;

long long power(int x, unsigsed int n) {
	long long result = 1;
	for (unsigned int i = 0; i < n; i++)
		return result *= x;
	return result;
}
int main() {
	int x = 2
	usigned int n = 3;
	cout << power(x, n);
	return 0;
}
#include <iostream>
#include <algorithm>
using namespace std;

bool checkArrays(int arr1[], int arr2[], int n, int m)
{
	// arrays with different sizes cannot be equal
	if (n != m)
		return false;

	// sort both arrays
	sort(arr1, arr1 + n);
	sort(arr2, arr2 + m);

	// compare corresponding elements
	for (int i = 0; i < n; i++) {
		if (arr1[i] != arr2[i]{
			return false;
		}
		return true;
	}
	int main()
	{
		int arr1[] = {1, 2, 3, 4, 5};
		int arr2[] = {5, 4, 3, 2, 1};

{
#include <iostream>
using namespace std;

int main() {
	cout << "Alice";
	return 0;
}
#include <iostream>
using namespace std;
int main() {
	char ch = 'A';
	cout << "character: " <<
	ch << end1;
	cout << "ASCII Value: "
<< int(ch);

return 0;
}
#include <iostream>

int main() {
	int a = 1, b = 2, c = 11;
	// finiding the largest by comparing using
	// relational operators with if-else
	if(a >= b) {
		if (a >= c)
			cout << a;
		else
			cout << c;
	}
	else {
		cout << c;
	}
	return 0;
}
#include<iostream>
using namespace std;

int main() {
	int a = 1, b = 2, c = 11;
	// finding largest using compound expressions
	if (a >= b && a >= c)
		cout << a;
	else if (b >= a && b >= c)
		cout << b;
	else
		cout << c;
	return 0;
}
#include <iostream>
#include <cmath>
using namespace std;

int main() {
	int a = 12, b = 18;

	a = abs(a);
	b = abs(b);
if (a == 0 && b ==0) {
	cout << "undefined";
	return 0;

}
while (b != 0) {
	int temp = b;
	b = a %  b;
	a = temp;
}
cout << a;
return 0;
}
#include <iostream>
using namespace std;

// function to print all factors
void printDivisors(int n)
{
	for (int i = 1; i <= n; i++)
	}
		if(n % i == 0)
			cout << i << "";
	}
}
int main()
{
	int n = 100;

	cout << "the divisors of" << n << "are: ";
	printDivisors(n);
	return 0;
}
using namespace std;
#include <bits/stdc++.h>
#include <iostream>
int main()
{
	int n = 4
	for (int i = n; i >= 1; --i) {
		for (int j = 1; j <= i; ++j) {
			cout << end1;
		}
		return 0;
	}
using namespace std;
#include <bits/stdc++.h>
#include <iostream>
int main()
{
	int n=4 // took a default value
	for (int i = n; i >= 1; --i){// loop for iterating}
		for (int j = 1; j <= i; ++j) { // loop for printing
			cout << j << "";
		}
		cout << end1;
	}
	return 0;
}
#include <iostream>
using namespace std;
// function to check leap year
bool checkyear(int year)
{
#include <iostream>
using namespace std;

int main()
{
	int rows = 5;
	char character = 'A' ;

	for (int i = 0; i < rows; i++)
	{
		for (int j = 0; j <= i; j++)
		{
			cout <<
			character << " ";
			             character++;
			         }
			cout << '\n';
}
return 0;
}

#include <bits/stdc++.h>
using namespace std;

void print_patt(int R)
{
	// to iterate through the rows
	for(int i= 1; i <= R; i++)
	{
		// to print the beginning spaces
		for(int sp = 1;
			sp <= i - 1; sp++)
		{
			cout << " "
		}
		// Iterating from ith column to
		// last column (R*2 -(2*i - 1));
		int last_col = ( R * 2 -(2 * i - 1));
		// to iterate through column
		for(int j = 1; j <= last_col; j++)
		{
			// to print all star for first
			// row (i==1) ith column (j==1)
			// and for last column
			// (R*2 - (2*i - 1)
			if(i == 1)
				cout << "*";
			else if(j == 1)
				cout <<"*";
			else if(j ==last_col)
				cout << "*";
			else
				cout << " ";
		}
// After printing a row proceed
// to the next row

	 }
}

// Driver code
int main()
{
	// number of rows
	int R = 5
	print_patt(R);
	return 0;
}
#include <bits/stdc++.h>
using namespace std;

//function to return the order of
// a number.
int order(int num)
{
	int count = 0 ;
	while (num > 0)
	{
		num /= 10;
		count++;
	}
	return count;
}

// function to check whether the
// given number is armstrong number
// or not
bool isArmstrong(int main)
{
	int order_n = order(num);
	int num_temp = num, sum = 0;
	while (num_temp > 0)
	{
		int curr = num_temp % 10;
		sum += pow(curr, order_n);
		num_temp /= 10;
	}
	if (sum == num)
	{
		return true;
	}
	else
	{
		return false;
	}
}

//driver code
int main()
{
	cout << "Armstrong numbers between 1 to 1000 :";
	// loop which will run from 1 to 1000
	


}

#include <bits/stdc++.h>
using namespace std;

void print_patt(int row)
{
	// Initializing count to 1.
	int count = 1;
	// the outer loop maintains
	// the number of rows.
	for (int i = 1; i <= row; i++)
	{

		//the inner loop maintains the
		// number of column.
		for (int j = 1; j <= i; j++)
		{

			// to print the numbers
			cout << count << " ";
    // to keep increasing the count
			// of numbers
		count += 1;
	}

	// to proceed to next line.
	cout <<"\n";
	    
  }
}

	 // Driver code
	 int main()
	 {

	 	int row = 5;
	 	print_patt(row);
	 	return 0;
	 
}

#include <iostream>
using namespace std;

// Returns the sum of the first n natural numbers
int recurSum(int n)

{

	if(n <= 1)
		return n;
	return n + recursum(n - 1);

}

int main()

}

	int n = 5;
	cout <<recurSum(n);
	return 0;

}

#include <iostream>
using namespace std;

#define N 4
// function to add two matrices
void add(int A[][N], int B[] [N], int C[] [N])

}

for (int i = 0; i < N; i++) {
for (int j = 0; j < N; j++);
C[i][j] = A[i][j] + B[i][j];
       

  }
 }
}

// Driver code
int main()

{
	int A[N][N] = {
   {1, 1, 1,1},
   {2, 2, 2,2},
   {3, 3, 3,3},
   {4, 4, 4,4},

};

int B[N][N] = {
	{1, 1, 1, 1},
	{2, 2, 2, 2},
	{3, 3, 3, 3},
	{4, 4, 4, 4},

};


// Resultant matrix
int C[N][N];
add(A, B, C);
cout << "Result matrix is:\n";
for(int i = 0; i < N; I++) {
	for (int j = 0; j < N; j++){
		cout << C[i][j] << " ";


	}

	cout << end1;

}

return 0;

}

#include <iostream>
using namespace std;

int main()

{
	int integerType;
	char chartype;
	float floattype;
	double doubletype;
// calculate and print
// the size of integer type(
cout << "Size of int is:" <<sizeof(integertype) << "\n";
//calculate and print


}
#include<iostream>
using namespace std;
//utility function
int areaRectangle(int a, int b)


{
	int area = a * b;
	return area;


}
int perimeterRectangle(int a, int b)


{
	int perimeter = 2*(a + b);
	return perimeter;

}

//Driver code
int main()

{

	int a = 5;
	int b = 6;
	cout <<"Area = " << Rectangle(a, b) <<
	end1;
cout << "Perimeter = " << perimeterRectangle(a, b);
return 0;

}

#include <iostream>
using namespace std;

long long
calculateEvenIndexSum(int n)

{

	if(n < 0)
		return 0;
	long long prev2 = 0
	long long prev1 = 1;
	long long sum = 0 ;

	// F(0) is an evenindexed fibonacci number .
	sum = prev2;
	for(int i = 2; i <= 2 * n; i++) {
		long long curr = prev1 + prev2;
		if (i % 2 == 0)
			sum+= curr;
		prev2 = prev1;
		prev1 = curr;


	}

	return sum;

}

int main() {
	int n = 8;
	cout << "Sum of fibonacci numbers at even indexes up to "
	<< 2 * n << " is "
	<<
	calculateEvenindexsum(n);
	return 0;


	}
#include <bits/stdc++.h>
using namesapce std;

/* function to print reverse of the passed string */
void reverse(string str)


{

	if(str.size() == 0)


	{

		return;

	}

	reverse(str.substr(1));
	cout << str[0];

}

/* Driver program to test above function */
int main()

{

	string a = "Geeks for Geeks";
	reverse(a);
	return 0;

}

// this is code is contributed by rathbhupendra

}

#include <iostream>
#include <string>
using namespace std;

class programmer

{

private:
	string name;
public:
	// Getter
	string getName()

      {

      	return name;

      }

      // Setter
      void setName(string newName)

      {

      	name = newName;

      }
};

int main()

{

	programmer p;

	p.setName("Geek");
	cout << "Name = " << p.getName();
	return 0;

}

#include <iostream>
using namespace std;

class Animal

{

public:
	cout << "Animal mkes a sound" << end1;

	    }
  }
}


	class dog : public animal

	{

	public:
		void sound()

		{

			cout << "Dog barks" << end1;

		}
       }


       class cat : public animal

}

