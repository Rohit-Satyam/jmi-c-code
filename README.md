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
11. Generate number from 1 - 100.


