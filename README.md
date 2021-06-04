# binary_to_decimal.cpp
Convert a Binary number into decimal using c++
#include<bits/stdc++.h>
using namespace std;
int binary_to_decimal(int n)
{ 
 int ans=0;
 int x=1;
 while(n>0)
 {
  int y = n%10;
  ans += x*y;
  x *= 2; // for 2^0 = 1
  n /= 10;
 }
 return ans;
}

int main()
{
 int n; 
 cin>>n;
 cout<<binary_to_decimal(n);
}
