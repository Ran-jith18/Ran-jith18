#include <iostream.h> 

#include <conio.h> 

int add(int a, int b){ 

return a+b; 

} 

int subtract(int a, int b) 

{ 

return a-b; 

} 

int multiply(int a, int b) 

{ 

return a*b; 

} 

double divide(int a, int b) 

{ 

if(b==0){ 

cout<<"Error:Division by zero!"<< endl; 

return 0; 

} 

return (double) a/b; 

} 

int rectangleArea(int length, int width) 

{ 

return length*width;
} 

double circleArea(int radius) 

{ 

return 3.14159 * radius * radius; 

} 

int main() 

{ 

int choice, num1, num2, length, width, radius; 

cout<<"Simple calculator program"<< endl; 

cout<<"1. Addition"<< endl; 

cout<<"2. Subtraction"<< endl; 

cout<<"3. Multiplication"<< endl; 

cout<<"4. Division"<< endl; 

cout<<"5. Rectangle Area"<< endl; 

cout<<"6. Circle Area"<< endl; 

cout<<"Enter your choice (1-6):"; 

cin>> choice; 

switch(choice) 

{ 

case 1: 

cout<<"Enter two numbers:"; 

cin>>num1>>num2; 

cout<<"Result:"<< add(num1, num2)<< endl; 

break; 

case 2:
cout<<"Enter two numbers:"; 

cin>>num1>>num2; 

cout<<"Result:"<<subtract(num1, num2) << endl; 

break; 

case 3: 

cout<<"Enter two numbers:"; 

cin>>num1>>num2; 

cout<<"Result:"<<multiply(num1, num2)<< endl; 

break; 

case 4: 

cout<<"Enter two numbers:"; 

cin>> num1>>num2; 

cout<<"Result:"<<divide(num1, num2)<< endl; 

break; 

case 5: 

cout<<"Enter length and width of rectangle:"; 

cin>>length>>width; 

cout<<"Area:"<<rectangleArea(length, width)<< endl; 

break; 

case 6: 

cout<<"Enter radius of the circle:"; 

cin>>radius; 

cout<<"Area:"<<circleArea(radius)<< endl; 

break; 

default: 
cout<<"Invalid choice!"<< endl; 

break; 

} 

getch(); 

return 0; 

}


