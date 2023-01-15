# flippedcount



//Online C++ compiler to run C++ program online
#include <iostream>

int countsetbits(int n) 
{
    int count=0;
    while(n>0){
        
        count++;
        n&=(n-1); 
        }
        // Write C++ code here
    
    return count;
}
int flippedcount(int a, int b)
{
    return countsetbits(a^b);
}
int main()
{
    int a=90;
    int b=80;
    cout<<flippedcount(a,b)<<endl;
    return 0;
}
