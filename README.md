# Functions
Printing Primes Using functions--->

#include <iostream>

using namespace std;
void isPrime(int n){
    bool prime=true;
    for(int i=1;i<n;i++){
        if(n%i==0){
            prime=false;
        }
    }
    if(prime){
        cout<<n<<endl;
    }

}

int main()
{
   //Write a program to check whether a number is prime or not using for loops:
/*   int n;
   cout<<"Type in the number you want to check as prime"<<endl;
   cin>>n;
   bool isPrime=true;
   for(int i=2;i<n;i++){
    if(n%i==0){
        isPrime=false;
        break;
    }
   }
   if(isPrime){
    cout<<"Prime"<<endl;
   }
   else{
    cout<<"Not a Prime"<<endl;
   }

   //Break and continue statement,
   //Using break and continue, change the code of square pattern into triangular stairs pattern
   int m;
   cout<<"Type in the value of the length of side of square"<<endl;
   cin>>m;
   int i=1;
   while(i<=m){
        int j=1;
        while(j<=m){
            cout<<j;
            j++;
            if(j>i){
                break;
            }
        }
        cout<<endl;
        i++;
   }
                */
/*    int i=1;
    while(i<5){
        if(i==3){
            continue;
        }
        cout<<i<<" ";
        i++;
    }  */
    cout<<"Enter the number greater than 2 and less than desired N. I will print all the prime numbers between it."<<endl;
    int n;
    cin>>n;
    for(int i=2;i<n;i++){
        isPrime(i);
    }



    return 0;
}

                          
                          More Function Illustrations--->
  #include <iostream>

using namespace std;
int fac(int n){
    int ans=1;
    for(int i=1;i<=n;i++){
        ans=ans*i;
    }
    return ans;
}
void nCr(int n, int r){
    int num= fac(n);
    int den= fac(r)*fac(n-r);
    cout<< num/den<<endl;
}
void PrimeorNot(int n){
    bool Prime=true;
    for(int i=2; i<n;i++){
        if(n%i==0){
            Prime=false;
            break;
        }
    }
    if(Prime){
        cout<<"Prime"<<endl;
    }
    else{
        cout<<"Not a Prime number"<<endl;
    }
}

void Printnums(int n){
    for(int i=1;i<=n;i++){
        cout<<i<<endl;
    }
}

int main()
{
    //Write a cpp program and a function to determine nCr or C(n,r) where n and r are both given by users,
    cout<<"Type in the values of N and R "<<endl;
    int n,r;
    cin>>n>>r;
    nCr(n,r);

    //Write a function to check whether a given number is prime or not:
    cout<<"Type the value of number you want to check as prime or not"<<endl;
    int m;
    cin>>m;
    PrimeorNot(m);
    //Whenever we write return in the function and the return is valid for the condition given,
    //Then the below code of function don't get executed and the function ends there

    //Write a function to print 1 to n, :
    cout<<"Type in the value of n and I will print numbers from 1 to n for u"<<endl;
    int l;
    cin>>l;
    Printnums(l);




    return 0;
}

  
