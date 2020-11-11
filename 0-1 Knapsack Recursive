#include <bits/stdc++.h>
#define lli long long int
using namespace std;

lli knapsack(lli wt[],lli val[],lli W, lli n)
{
    if (n==0 || W==0){
        return 0;
    }
    else if (wt[n-1]<=W){
        return max(val[n-1]+knapsack(wt,val,W-wt[n-1],n-1),knapsack(wt,val,W,n-1));
    }
    else{
        return knapsack(wt,val,W,n-1);
    }
}


int main()
{
    lli n,W;
    cin>>n;                                     //Input Number of items
    lli wt[n],val[n];
    for(lli i = 0;i<n;cin>>wt[i],i++);          //Input Values of items
    for(lli i = 0;i<n;cin>>val[i],i++);         //Input Weight of items
    cin>>W;                                     //Input Weight of Knapsack
    cout<<knapsack(wt,val,W,n);
    return 0;
}
