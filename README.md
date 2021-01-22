# jmi-c-code

1. Calculate the area of circle

```c
//Area of the circle
#include <iostream>

using namespace std;

class CircleArea{
  private:
  double area;
  
 
  public:
  int radius;
  void inputRadius(){
      cout<<"Please Enter Radius of circle";
    cin>>radius;
    
  }
  
  void calculateArea(){
      area=3.14*radius*radius;
      cout<<"Area of Circle is: "<<area;
  }
    
};

int main()
{
    CircleArea circleArea;
    circleArea.inputRadius();
    circleArea.calculateArea();

    return 0;
}
```
2. Check Gender

```c
//Check whether a person is male or female
#include <iostream>

using namespace std;

class CheckGender{
    private:
    string gender;
    
    public:
    string ch;
    void inputCharacter(){
        cout<<"Please enter gender as M/F";
        cin>>ch;
    }
    
    void displayGender(){
        if(ch=="m" || ch=="M"){
            gender="Male";
            cout<<"You have selected: "<<gender;
        }
        else if(ch=="f" || ch=="F"){
            gender="Female";
            cout<<"You have selected: "<<gender;
        }
        else{
            cout<<"You have entered invalid character";
        }
        
            }
};

int main()
{
    
    CheckGender checkGender;
    checkGender.inputCharacter();
    checkGender.displayGender();
    return 0;
}
```
3. Check Vowel

```c
//Check Vowel Using Switch Case
#include <iostream>

using namespace std;

class CheckVowel
{
  
  private:
  char chk;
  
  public:
  char ch;
  void input(){
      cout<<"Enter a letter to check: ";
      cin>>ch;
      chk=ch;
  }
  
  void check()
  {
      switch (chk) 
    { 
        case 'a':  
            cout << "You entered ["<<chk<<"] which is a vowel"; 
            break; 
        case 'e':  
            cout <<  "You entered ["<<chk<<"] which is a vowel";
            break; 
        case 'i':  
            cout <<  "You entered ["<<chk<<"] which is a vowel";
            break; 
        case 'o':  
            cout <<  "You entered ["<<chk<<"] which is a vowel";
            break; 
        case 'u':  
            cout <<  "You entered ["<<chk<<"] which is a vowel";
            break; 
        
        default:  
            cout << "You entered ["<<chk<<"] which is a consonant"; 
            break;   
    } 
  }
};

int main()
{
   CheckVowel vowel;
   vowel.input();
   vowel.check();

    return 0;
}
```
4. Display Name

```c
//Display Name on screen
#include <iostream>

using namespace std;

class DisplayName{
  private:
  string privateName;
 
  public:
  string name;
  void inputName(){
      cout<<"Please Enter your name";
    cin>>name;
    privateName=name;
  }
  
  void display(){
      cout<<"Hello, I am "<<privateName;
  }
    
};

int main()
{
    DisplayName displayName;
    displayName.inputName();
    displayName.display();

    return 0;
}
```
5. Calculate salary

```c
//Check whether a person is male or female
#include <iostream>

using namespace std;
class CalculateSalary{
    private: 
    double salary;
    double hra;
    
    public:
    int basicSal;
    void inputBasicSalary(){
        cout<<"Please enter basic salary: ";
        cin>>basicSal;
    }
    
    void totalSalary(){
        if(basicSal>20000){
            salary=basicSal*1.02;
            hra=basicSal*0.02;
        }
        else{
            salary=basicSal*1.012;
            hra=basicSal*0.012;
        }
        
        cout<<"Total Salary including HRA is: "<<salary<<" and HRA is: "<<hra;
    }
};

int main()
{
    CalculateSalary calculateSalary;
    calculateSalary.inputBasicSalary();
    calculateSalary.totalSalary();
  
    return 0;
}
```
6. Simple Interest

```c

//Find Simple Interest
#include <iostream>

using namespace std;

class SimpleInterest{
  private: 
  double interest;
  
  public:
  int principal,years,rate;
  
  void enterValues() {
      cout<<"Program to calculate Simple Interest "<<endl;
     cout<<"Please enter Principal: ";
      cin>>principal;
      cout<<"Please enter Years: ";
      cin>>years;
    
      cout<<"Please enter Rate of Interest: ";
      cin>>rate;
  }
  
  void calculateInterest(){
      interest=(principal*rate*years)/100;
      cout<<"Simple Interest of Entered values is:Rs "<<interest;
  }
    
};



int main()
{
    SimpleInterest simpleInterest;
    simpleInterest.enterValues();
    simpleInterest.calculateInterest();
    return 0;
}
```

6. Wap to print 1 to 100

```c
#include<iostream>
using namespace std;
 class sequence
 {
     private:
     int i=1;
     public:
     void input();
     void output();
 };
 void sequence::input(){
     
 }

 void sequence::output()
 {
while(i<=100)
{
    cout<<"\t"<<i;
    i++;

}
 }
int main()
 {
     sequence(x);
     x.input();
     x.output();
 }
 ```
 7. Display even number from 1 - 50 & find its sum.
 
 ```c
 #include<iostream>
using namespace std;
 class even
 {
     private:
     int i=2,sum=0;
     public:
     void input();
     void output();
 };
 void even::input(){
     
 }

 void even::output()
 {
while(i<=50)
{
    cout<<"\t"<<i;
    i=i+2;
    sum=sum+i;
}
 cout<<"sum:"<<sum;
 }
int main()
 {
     even(x);
     x.input();
     x.output();
 }
 ```
 8. Display odd number from 1 - 50 & find its sum.
 
 ```c
 #include<iostream>
using namespace std;
 class odd
 {
     private:
     int i=1,sum=0;
     public:
     void input();
     void output();
 };
 void odd::input(){
     
 }

 void odd::output()
 {
for(i=1;i<=50;i=i+2)
{
    cout<<"\t"<<i;
    i=i+2;
    sum=sum+i;
}
 cout<<"sum:"<<sum;
 }
int main()
 {
     odd(x);
     x.input();
     x.output();
 }
 ```
 9. Find root of quadratic equation
 
 ```c
 #include <iostream>
#include <cmath>
using namespace std;
class roots {
    private:
    int a, b, c, d, r1, r2;
    public: 
    void input();
    void output();
};
void roots::input() {
    cout << "Standard form of quadratic equation is:\n";
    cout << "ax^2 + bx + c = 0\n";
    cout << "where a, b, c are known numbers and a != 0\n\n";
    
    cout << "Enter a: ";
    cin >> a;
    
    cout << "Enter b: ";
    cin >> b;
    
    cout << "Enter c: ";
    cin >> c;
}
void roots::output() {
     d = (b*b) - 4*a*c;
    if (d > 0) {
        cout << "It has two real roots:\n";
        r1 = (-b + sqrt(d)) / 2*a;
        r2 = (-b - sqrt(d)) / 2*a;
        cout << "First root: " << r1;
        cout << "\nSecond root: " << r2;
    }
    else if (d == 0) {
        cout << "It has one real root.\n";
        r1 = -b / 2*a;
        cout << "Root: " << r1;
    }
    else if (d < 0) {
        cout << "It has no real roots";
    }
    else {
        cout << "Enter valid numbers";
    }
}
int main () {
    roots q;
    q.input();
    q.output();
}
```
10. Find sequence of a protein as given below:  
            C = ccttaattaattccat
            A = attcttcttc
            T = ttatccta by entering a character. (switch case)
```c
 #include <iostream>
using namespace std;
class protein {
    private:
    char letter;
    public: 
    void switchcase();  //I named the function switchcase
};
void protein::switchcase() {
    cout << "Enter a letter: ";
    cin >> letter;
    switch (letter) {
        case 'c':
        case 'C': cout << "The protein sequence is: ccttaattaattccat";
        break;
        case 'a':
        case 'A': cout << "The protein sequence is: attcttcttc";
        break;
        case 't':
        case 'T': cout << "The protein sequence is: ttatccta";
        break;
        default: cout << "ERROR: Enter an appropriate character.";
    }
}
int main () {
    protein q;
    q.switchcase();
}
```
11. Generate number from 1 - 100 using do/while loop.

```c
#include <iostream>
using namespace std;
class numbers {
    private:
    int i;
    public: 
    void no();
};
void numbers::no() {
    i = 1;
    do {
        cout << i << "\t";
        i++;
    }
    while (i <= 100);
}
int main () {
    numbers n;
    n.no();
}

```
12. Generate numbers from 1 - 100 without using a loop

```c
#include <iostream>
using namespace std;
class numbers {
    private:
    int i;
    public: 
    void no();
};
void numbers::no() {
    i = 1;
    x:
    cout << i << "\t";
    i++;
    if (i <= 100) {
        goto x;
    }
}
int main () {
    numbers n;
    n.no();
}
```
13. Calculate electricity bill of a consumer with the following condition:
-	Unit less than 200. Price is Rs. 1.5  per unit.
-	Unit greater than 200 and less than 400. Price is Rs. 4 per unit.
-	Unit greater than 400 and less than 900. Price is Rs. 6 per unit.

```c
#include <iostream>
using namespace std;
class elecBill {
    private:
    int units;
    float bill;
    public: 
    void input();
    void output();
};
void elecBill::input() {
    cout << "Enter units of electricity consumed: ";
    cin >> units;
}
void elecBill::output() {
    if (units <= 200) {
        cout << "\nFor the units consumed by you, rate of 1 unit electricity is: Rs. 1.5\n";
        bill = 200 * 1.5;
        cout << "\nYour electricity bill is Rs. " << bill;
    }
    else if (units > 200 && units <= 400) {
        cout << "\nFor the units consumed by you, rate of 1 unit electricity is: Rs. 4\n";
        bill = 200 * 4;
        cout << "\nYour electricity bill is Rs. " << bill;
    }
    else if (units > 400 && units <= 900) {
        cout << "\nFor the units consumed by you, rate of 1 unit electricity is: Rs. 6\n";
        bill = 200 * 6;
        cout << "\nYour electricity bill is Rs. " << bill;
    }
    else {
        cout << "\nERROR: Enter valid amount";
    }
}
int main () {
    elecBill n;
    n.input();
    n.output();
}
```
14. Swap two characters

```c
#include<iostream>
using namespace std;
class afsha
{
    private:
    char a,b,c;
    public:
    void inputz();
    void outputz();
};
void afsha::inputz()
{
cout<<"enter value of a,b=";
cin>>a>>b;
cout<<"After swaping:\n";
}
void afsha::outputz()
{
c=a;
a=b;
b=c;
cout<<"a="<<a<<"\n";
cout<<"b="<<b;
}
int main()
{
afsha o;
o.inputz();
o.outputz();
}
```
15. Area of Rectangle

```
#include<iostream>
using namespace std;
class rectangle
{
    private:
    int l,b,a;
    public:
    void inputz();
    void outputz();
};
void rectangle::inputz()
{
cout<<"enter value of l and b=";
cin>>l>>b;
}
void rectangle::outputz()
{
a=l*b;
cout<<"area of rectangle="<<a;
}
int main()
{
rectangle o;
o.inputz();
o.outputz();
}
```
16. Area of Circle

```c
#include<iostream>
using namespace std;
class circle
{
    private:
    float r,a;
    public:
    void inputz();
    void outputz();
};
void circle::inputz()
{
cout<<"enter value of r=";
cin>>r;
}
void circle::outputz()
{
a=3.14*r*r;
cout<<"area of circle="<<a;
}
int main()
{
circle o;
o.inputz();
o.outputz();
}
```
17. Swap two variables

```c
#include<iostream>
using namespace std;
class exchange
{
    private:
    int a,b,e;
    public:
    void inputz();
    void outputz();
};
void exchange::inputz()
{
cout<<"enter value of a,b=";
cin>>a>>b;
}
void exchange::outputz()
{
e=a;
a=b;
b=e;
cout<<"a:"<<a<<"\t";
cout<<"b:"<<b;
}
int main()
{
exchange o;
o.inputz();
o.outputz();
}
```
18. Swap two variables without the third variable

```c
#include<iostream>
using namespace std;

class swp
{
    private:
    int a,b;
    public:
    void inputz();
    void outputz();
};
void swp::inputz()
{
cout<<"enter value of a,b=";
cin>>a>>b;
cout<<"After swaping:\n";
}
void swp::outputz()
{
a=a+b;
b=a-b;
a=a-b;
cout<<"a="<<a<<"\n";
cout<<"b="<<b;
}
int main()
{
swp o;
o.inputz();
o.outputz();
}
```
19. Square of a number

```c
#include<iostream>
using namespace std;
class square
{
    private:
    int a,s;
    public:
    void inputz();
    void outputz();
};
void square::inputz()
{
cout<<"enter value of a=";
cin>>a;
}
void square::outputz()
{
s=a*a;
cout<<"square="<<s;
}
int main()
{
square o;
o.inputz();
o.outputz();
}
```
20. Sum of 2 numbers

```c
#include<iostream>
using namespace std;
class afsha
{
    private:
    int a,b,s;
    public:
    void inputz();
    void outputz();
};
void afsha::inputz()
{
cout<<"enter value of a,b=";
cin>>a>>b;
}
void afsha::outputz()
{
s=a+b;
cout<<"sum="<<s;
}
int main()
{
afsha o;
o.inputz();
o.outputz();
}
```
21. Product of 3 numbers

```c
#include<iostream>
using namespace std;
class prod
{
    private:
    int a,b,c,p;
    public:
    void inputz();
    void outputz();
};
void prod::inputz()
{
cout<<"enter value of a,b,c=";
cin>>a>>b>>c;
}
void prod::outputz()
{
p=a*b*c;
cout<<"product="<<p;
}
int main()
{
prod o;
o.inputz();
o.outputz();
}
```
22. 



