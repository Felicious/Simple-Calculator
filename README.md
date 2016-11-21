# Simple-Calculator
This simple calculator can do simple arithmetic like adding, subtracting, multiplying, and dividing. 
#include <iostream>
#include <string>

using namespace std;
void whatfunction(string input, string &m);

int main()
{
    string input; //input = 45 + 52
    getline(cin, input);
    string m = "";
    whatfunction(input,m);

    return 0;
}
void whatfunction(string input, string &m){
    for (int i = 0; i < input.length(); i++){
        if (input[i] == '+'){
            m = "add";
        }
        else if (input[i] == '-'){
            m = "sub";
        }
        else if (input[i] == '/'){
            m = "div";
        }
        else if (input[i] == '*'){
            m = "mul";
        }
    }
}
