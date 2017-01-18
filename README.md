# cse330


//Header files
#include <stack>
#include <iostream>
#include <string>
using namespace std;

int prec (char op) // defines the prec function
{
 if (op =='c')
 return 0;
 if (op =='+' || op == '-')
 return 1;
 if (op =='*' || op == '/')
 return 2;
 return 0;
}

int main(){
stack <char> postfix;
char ch;
cin.get(ch);
while(!cin.eof()) {
    if((ch >='0' and ch < '9') or(ch >='a' and ch < 'z') or (ch >='A' and ch < 'Z'))
        cout <<ch;
    else
        if(ch == '(')
           postfix.push();

        else if (ch ==')');
         }
             while(!postfix.empty() and (postfix.top()!= '(')) {
                  cout.top();
                  postfix.pop();

             if(!postfix.empty())
                  postfix.pop();
            }

             else cout << "No matching!";
        else if((ch =='*') or  (ch =='/') or (ch =='+') or (ch =='-') )
             if (postfix.empty() or postfix.top() < ch)
                 postfix.push();
             else (postfix.top() >= ch);
                 while(!postfix.empty() and postfix.top() >= ch); {
                     postfix.top();
                     postfix.pop();
                     }
                 postfix.push();
       else cout << "check for errors";
while(!postfix.empty()) {
    postfix.top();
    postfix.pop();
}
