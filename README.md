# 8th
#include<iostream>
using namespace std;
// all about pass by value and pass by reference
// int a = 10;
 
// int main(){
//     // to access global variable and not the local variable then we have a 
//     // a technique known as scope resolution -> [::]
//     int a = 5;// this is a local variable i.e. only accessible in main function
//     cout<<a<<endl;// this will print the local variable
//     a++;
//     cout<<a<<endl;
//     cout<<::a<<endl;// this will print the global variable 

//     return 0;
// }

// example of pass by value 
// void changeValue(int z){
//     z=100;
// }
// int main(){
//     int a = 5;
//     changeValue(a);
//     cout<<a;
//     return 0;
// }


// example of pass by reference 
// int main(){
//     int p=5;
//     int &q=p;
//     q++;
//     cout<<&q<<endl;
//     cout<<&p;
//     return 0;
// }


// one more relatable example
//     void changeValue(int &z,int &y){
//     z=100;
//     y=99;
// }
// int main(){
//     int a = 5;
//     int b = 10;
//     changeValue(a,b);
//     cout<<a<<" "<<b<<endl;
//     return 0;
// }

// Default parameter
int add(int a,int b=1, int c=10){
    return (a+b)+c;
}
int main(){
    cout<<add(1)<<endl;//12
    cout<<add(10,20)<<endl;//40
    cout<<add(10,20,40)<<endl;//70
    return 0;
}
