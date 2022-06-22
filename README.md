# Number-to-string
number to string by using recursion 

#include<bits/stdc++.h>
using namespace std;

void divide(int num)
{
    string arr[]={"zero","one","two","three","four","five","six","eight","nine"};
    if(num==0)
    {
        return ;
    }
    int digit=num%10;
    divide(num/10);
    cout<<arr[digit]<<" ";
}

int main()
{
    int num;
    cout<<"enter a number :";
    cin>>num;
    divide(num);
}
