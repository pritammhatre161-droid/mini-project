# mini-project
playing with carts
// today is day i dont know whatever it is today we will play with maps and make a simple code and also post on github
#include<iostream>
#include<unordered_map>
#include<string>
using namespace std;
int main () {
  unordered_map<string ,int> cart;
  cout<<"adding items to the cart"<<endl;
  cart["apple"]=2;
  cart["banana"]=5;
  cart["coke"]=5;

  //now we will add items in apple
  cart["apple"]+= 3;

  //lets also remove the coke  keep it healthy
  cart.erase("coke");
  cout<<"your current cart contains"<<endl;
  for (auto const&pair : cart){
    cout << "- " << pair.first << ": x" << pair.second << endl;

  } 
  cout<<"the total items in the cart are"<<cart.size()<<endl;
  return 0 ;
}
