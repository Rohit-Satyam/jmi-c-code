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
