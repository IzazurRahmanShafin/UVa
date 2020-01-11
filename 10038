#include<bits/stdc++.h>
using namespace std;
#define nwl printf("\n")
#define spc printf(" ")

int abst(int n){
    if (n>=0) return n;
    else return -1*n;
}
int main(){
    int n;
    while (scanf("%d",&n)!=EOF){
        vector<int>arr;
        vector<int>jl;
        for(int i=0;i<n;i++){
            int a;
            cin >> a;
            arr.push_back(a);
        }
        if (n==1) cout << "Jolly\n";
        else {
            for (int i=0;i<n-1;i++){
                int p = abst(arr[i] - arr[i+1]);
                jl.push_back(p);
            }
            sort(jl.begin(), jl.end());
            if (jl[0]==1){
                bool flag = 1;
                for(int i=0;i<jl.size()-1;i++){
                    if (jl[i]+1!=jl[i+1]){
                        flag = 0;
                        break;
                    }
                }
                if (flag == 1) cout << "Jolly\n";
                else cout << "Not jolly\n";
            }
            else cout << "Not jolly\n";
        }
    }
    return 0;
}
