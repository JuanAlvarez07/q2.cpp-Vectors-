#include <iostream>
#include <vector>

using namespace std;

void fillvector(vector<int>& newVector){

  cout<<"Size of triangle: ";
  unsigned int size;
  cin>>size;
  newVector.push_back(size);
  }

void triangles(const vector<int>& newVector){
  unsigned int size= newVector[0];
  for(unsigned int i=1;i<=size;++i ){
    for(unsigned int start=1 ;start<=i;++start){
      cout<<"T";
    }
    cout<<endl;
  }
  for(int i=(size-1);i>=1;--i){
    for(int start=1;start<=i;++start){
      cout<<"T";
    }
    cout<<endl;
  }
}
int main(){

  vector<int> myVector;
  fillvector(myVector);
  triangles(myVector);
  return 0;

}

