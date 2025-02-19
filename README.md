#include "BankAccount.h"
#include <iostream>
using namespace std;
BankAccount::BankAccount(string name){
    Name=name;
    Balance=0.0;
};
BankAccount::BankAccount(string name, double balance){
    Name=name;
    Balance=balance;
};
BankAccount::Withdraw(double amount){
    if (amount <=0){
        cout<< "invalid" << endl;
    }
    if (Balance-amount<=-500){
        cout<<"cant over draft more than 500";
    }
    else{
        
    }
    
};
//bankacc.cpp  

#include <iostream>
#include <string>
using namespace std;
class BankAccount {
    private:
    string Name;
    double Balance;
    public:
    void BankAccount(string);
    void BankAccount(string,double);
    void Withdraw(double);  
    void deposit(double);
    void SetBalance(double);
    string GetName();
    double GetBalance(); 
};
//bank acc.h
