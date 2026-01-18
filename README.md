# stl
vector
#include <iostream>
#include <vector>
using namespace std;
int main(){
    //vector
    //1. size and capacity
     vector<int>v = {1,2,3,4,5};
    // cout<<v.size()<<endl;
    // cout<<v.capacity()<<endl;
    // //2.pusH_back and pop_back
    // v.push_back(7);
    // for(int i :v){
    //     cout<<i<<" ";
    // }
    // cout<<endl;
    // v.pop_back();
    // for(int i :v){
    //     cout<<i<<" ";
    // }
    cout<<endl;
    //3. emplace_back
    // v.emplace_back(23);
    // for(int i:v){
    //     cout<<i<<" ";
    // }
    // cout<<endl;
    //4.at() or []
    //cout<<v.at(2);
    // for(int i:v){
    //     cout<<i<<" ";
    // }
    //5. front & back
    // cout<<v.front()<<endl;
    // cout<<v.back()<<endl;
    //6.erase 
    // v.erase(v.begin()); //for other  v.erase(v.begin()+1); // for range v.erase(v.begin(),v.begin()+3);
    // for(int i : v){
    //     cout<<i<<" ";
    // }
    // cout<<endl;
    //7.insert
    // v.insert(v.begin()+2,100);
    // for(int i : v){
    //     cout<<i<<" ";
    // }
    // cout<<endl;
    //Iterators 
    //1. forward
    // vector<int>::iterator i;
    // for(i = v.begin();i != v.end();i++){
    //     cout<<*(i)<<" ";
    // }
    // cout<<endl;
    //2. backward
    //     vector<int>::iterator i;
    //     for (auto i = v.rbegin(); i != v.rend(); ++i) {
    //     cout << *i << " ";
    // }
    // cout << endl;
}
