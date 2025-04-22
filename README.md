# codsofttaskno1
This is code for a program that generates a random number and asks the user to guess it. It also provides feedback on whether the guess is too high or too low until the user guesses the correct number.
#include<iostream>
#include <cstdlib>
using namespace std;


int main()
{
    int num;
 int guess =rand()%100+1;
 int icount =0;
   do
    {
    cout<<"Enter your guess between 1 and 100 ";
    cin>>num;



       if (num<guess)
       {
           cout<<"Number is too low"<<endl;
       }
       else if (num>guess)
       {
           cout<<"Number is too high"<<endl;
       }
       else{
       cout<<"Guess is correct :)"<<endl;
       }
       icount ++;
    } while (num != guess);
cout<<"You needed"<<icount<<" "<<" tries to get the guess right";
return 0;

}
