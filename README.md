# stl
vector,all map
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
1.MAP
#include <iostream>
#include <map>
using namespace std;
int main(){
     map<string,int>m;
     m["CAR"] = 100;
     m["bbike"] = 200;
     m["aeroplanes"] = 30;
    //  for(auto p : m){
    //      cout<<p.first<<" "<<p.second<<endl;
    //  }
    //Insert
    // m.insert({"camera",100});
    // for(auto p : m){
    //     cout<<p.first<<" "<<p.second<<endl;
    // }
    //update
    // m.insert({"car",10});
    // for(auto p : m){
    //     cout<<p.first<<" "<<p.second<<endl;
    // }
    // m["car"] = 100;
    // for(auto p : m){
    //     cout<<p.first<<" "<<p.second<<endl;
    // }
    // Count
    // m.insert({"car", 10});
    // m.insert({"car", 20});
    // m.insert({"car", 3});
    // cout<<m.count("car")<<endl; // return 1 becouse it is not a multimap
    //Find
    // if(m.find("CAR")!=m.end()){
    //     cout<<"found"<<endl;
    // }else{
    //     cout<<" not found"<<endl;
    // }
2.MULTIMAP
#include <iostream>
#include <map>
using namespace std;
int main(){
    multimap<string,int>m;
    m.emplace("tv",10);
    m.emplace("tv",10);
    m.emplace("tv",10);
    m.emplace("tv",10);
    cout<<m.count("tv")<<endl;
    m.erase(m.find("tv"));//remove only 1 value of tv
    for(auto i : m){
        cout<<i.first<<" "<<i.second<<endl;
    }
}
3.UNORDERED MAP
#include <iostream>
#include <unordered_map>
using namespace std;

int main() {
    unordered_map<string, int> um;

    um["CAR"] = 100;
    um["bbike"] = 200;
    um["aeroplanes"] = 30;

    for (auto p : um) {
        cout << p.first << " " << p.second << endl;
    }
    //all operation same as map insert,erase,count ,empty,find
}
