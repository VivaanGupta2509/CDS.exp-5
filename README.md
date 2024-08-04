# Experiment 5 
## Aim - 
To study and implement C++ decision making statements.

## Software Used - 
VS code

## Theory -
Conditional statements allow you to make decisions within your programs. Specifically they can be used to execute specific blocks of code for particular situations only. <br>
There are four primary conditional statements in C language: _if statement_, _if-else statement_,_nested if-else statement_, and _switch statement_. <br> 
### _if:_ 
The simplest form among conditionals where a certain condition is evaluated and if it evaluates true then certain flow control unit executes its commands. <br>

### _if-else:_
This is an extension of the first form since we have the alternative block whose commands get executed provided that the original statement was false when selected. <br>

### _nested if-else:_
This enables the evaluation of several conditions sequentially until it finds one which is true whereby if this happens its contained or associated block will be executed while ignoring all other blocks. <br>

### _switch case:_ 
This facilitates picking one among many subprograms depending on a variable’s value. So rather than using multiple nested if-else statements we can use switch instead.

## Code- 
### A1-
```
#include<iostream>
using namespace std;

int main() 
{
    // if statements 
    int x = 20;
    int y = 18;
    if (x > y)
    {
        cout<< "x is greater than y "<<endl;
    }
    

    // else statement
    int time = 20;
    if (time < 18) 
    {
        cout<<"Good Morning"<<endl;
    }
    else{
        cout<<"Good Evening"<<endl;
    }

    // simple if else 

    int  num;
    cout<<"Enter positive number: ";
    cin>>num;
    if(num==0) {
        cout<<num<<"You have entered zero"<<endl;
    }
    else if(num%2!=0){
        cout<<num<<" is odd"<<endl;
    }
    else {
        cout<<num<<" is even"<<endl;
    }
    
    return 0;


}
```
### A2-
```
#include<iostream>
using namespace std;

// Nested if else program
int main() {
    int  num1, num2, num3;
    cout<<"Enter number-1: ";
    cin>>num1;
    cout<<"Enter number-2: ";
    cin>>num2;
    cout<<"Enter number-3: ";
    cin>>num3;

    if(num1>=num2) {
        if(num1>=num3) {
            cout<<num1<<" is the greatest number"<<endl;
        }
        else {
            cout<<num3<<" is the greatest number"<<endl;
        }
    }
    else if(num2>=num1) {
        if(num2>=num3) {
            cout<<num2<<" is the greatest number"<<endl;
        }
        else {
            cout<<num3<<" is the greatest number"<<endl;
        }
    }
    
}
```

### B-
```
#include<iostream>
using namespace std;
 // Simple calculator using 'Switch case'
 
 int main()
 {
    int choice;
    double num1,num2;
    cout<<"This is a simple calculator"<<endl;
    cout<<"1 for addition"<<endl;
    cout<<"2 for subtraction"<<endl;
    cout<<"3 for multiplication"<<endl;
    cout<<"4 for multiplication"<<endl;
    cout<<" Enter the operation choice number (1-4)"<<endl;
    cin>>choice;

    cout<<"Enter any two numbers: "<<endl;
    cin>>num1>>num2;

    switch(choice){
        case 1:
        cout<<"Addition = "<<num1+num2<<endl;
        break;

        case 2:
        cout<<"subtraction = "<<num1 - num2<<endl;
        break;

        case 3:
        cout<<"Multiplication = "<<num1*num2<<endl;
        break;

        case 4:
        cout<<"Division = "<<num1/num2<<endl;
        break;
    }

    return 0;
 }
```

## Output - 
### A1 - 


### A2 - 
<img width="687" alt="Screenshot 2024-08-05 at 2 04 50 AM" src="https://github.com/user-attachments/assets/e737d7b0-c583-4895-9dcc-1fe1c9567a2e">


### B - 
<img width="684" alt="Screenshot 2024-08-05 at 2 03 33 AM" src="https://github.com/user-attachments/assets/5ff21d26-0d5c-4a65-8ca2-dc4224a13332">







