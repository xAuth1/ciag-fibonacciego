#include <iostream>
#include <iomanip>

using namespace std;

long double fibo[100000]; int n;

int main()
{
    cout << "Ile liczb Fibonacciego mam zaznaczyc: ";
    cin>>n;

    fibo[0]=1;
    fibo[1]=1;

    for (int i=2; i<n; i++)
    {
        fibo[i] = fibo[i-1] + fibo[i-2];
    }

cout<<setprecision(10000);

    //for (int i=0; i<n; i++)
    //{
    //    cout<<endl<<"wyraz nr"<<i+1<<": "<<fibo[i];
    //}

cout<<endl<<"wyraz nr"<<n<<":"<<fibo[n-1];
    return 0;
}
