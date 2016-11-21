# Simple-Calculator
This simple calculator can do simple arithmetic like adding, subtracting, multiplying, and dividing. 
#include <iostream>
#include <string>

using namespace std;
string whatfunction(string input);

int main()
{
    string input; //input = 45 + 52
    cin>>input;
    string funct = whatfunction(input);
    
    return 0;
}
string whatfunction(string input){
    for (int i = 0, i < input.length(), i++){
        if (input[i] == '+'){
            return addition;
        }
        else if (input[i] == '-'){
            return subtraction;
        }
        else if (input[i] == '/'){
            return division;
        }
        else if (input[i] == '*'){
            return multiplication;
        }
    }
}
