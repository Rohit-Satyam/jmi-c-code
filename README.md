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


