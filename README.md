# Pair-Sum
Starting Questions from CodeStudio in c++
#include <bits/stdc++.h> 
#include <bits/stdc++.h> 
vector<vector<int>> pairSum(vector<int> &arr, int s){
   vector <vector<int>> shraddha;
    for(int i=0;i<arr.size();i++)
    {
        for(int j=i+1;j<arr.size();j++)
        {
            if(arr[i]+arr[j]==s)
            {
                vector<int> ekor;
                ekor.push_back(min(arr[i],arr[j]));
                ekor.push_back(max(arr[i],arr[j]));
                shraddha.push_back(ekor);
            }
        }
    }
    sort(shraddha.begin(),shraddha.end());
    return shraddha;
}
