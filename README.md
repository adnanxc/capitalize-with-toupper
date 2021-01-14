# capitalize-with-toupper
capitalize the first letter of each string 


#include <iostream>
using namespace std;

string modify (string a){
    string n = a;
    int length = a.length();
    if(a[0]>=97 && a[0]<=122){
    n[0]= toupper(a[0]);
    }

    for(int i=1; i<length; i++){
        if(a[i]==' '){
            n[i+1]= toupper(a[i+1]);
        }

    }

   return n;
}




int main(){
    string s;
    cout << "Enter your string: ";
    getline(cin,s);

    cout << "New string: " << modify(s);
}
