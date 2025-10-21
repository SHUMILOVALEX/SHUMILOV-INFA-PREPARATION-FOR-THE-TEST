TASK 1
#include <iostream>
#include <vector>
#include <ctime>
using namespace std;

int main(){
    srand(time(0));
    int ar;
    cout<<"размер ";
    cin>>ar;
    vector<int> vec(ar);
    float sum = 0;
    for (int i = 0; i != ar; i++){
        int start = 1;
        int end = 9;
        int x = rand() % (end - start + 1) + start;
        sum+=x;
        vec[i]=x;
        cout<<x<<endl;
    }
    int kol=0;
    for (int j : vec){
        if (j<sum/ar){
            kol++;
        }
        
  }
    cout<<sum/ar<<" "<<kol;
}
TASK 2
#include <iostream>
#include <vector>
#include <ctime>
using namespace std;

int main(){
    srand(time(0));
    int ar;
    cout<<"размер ";
    cin>>ar;
    vector<int> vec(ar);
    int num = 0;
    int last = 0;
    for (int i = 0; i != ar; i++){
        int start = 1;
        int end = 9;
        int x = rand() % (end - start + 1) + start;
        last = num;
        num = x;
        if (i % 2 == 1){
            vec[i-1] = num;
            vec[i] = last;
            
   }
     cout<<x<<" ";
   }
  cout <<"\n" <<last<<" "<< num<<" ";
   for(int i : vec){
   cout<<i<<" ";
  }
}
TASK 3
#include <iostream>
#include <vector>
#include <ctime>
using namespace std;

int main(){
    srand(time(0));
    int ar;
    cout<<"size";
    cin>>ar;
    vector<int> vec(ar);
    vector<int> vec1;
    
  int sum = 0;
   for (int i = 0; i != ar; i++){
  int start = 1;
   int end = 9;
  int x = rand() % (end - start + 1) + start;
    if (x % 3 ==0){
  vec1.push_back(x);
  }
    cout<<x;
  }
  cout<<" answer";
  for (int i:vec1){
      cout<<" "<<i;
  }
} 
Task 4
#include <iostream>
#include <vector>
#include <ctime>
#include <cmath>
using namespace std;

int main(){
    srand(time(0));
    int ar;
    cout<<"size";
    cin>>ar;
    vector<int> vec(ar);
    vector<int> vec1;
        int sum = 0;
    for (int i = 0; i != ar; i++){
        int start = 1;
        int end = 9;
        int x = rand() % (end - start + 1) + start;
        vec1.push_back(x*x);
        cout<<x<<" ";
  }
  cout<<" answer";
    for (int i:vec1){
      cout<<" "<<i;
  }
}
Task 9 
#include <iostream>
#include <vector>
#include <ctime>
#include <cmath>
using namespace std;

int func(int a, int b){
    return a * b;
}

int main(){
    int num1;
    int num2;
    cout<<"Введи 2 числa ";
    cin>>num1;
    cin>>num2;
    cout<<"answer = "<<func(num1,num2);
}
