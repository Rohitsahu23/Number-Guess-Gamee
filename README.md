#include<iostream>
#include<cstdlib>

using namespace std;
int main()
{
    string name;
    char input;
    int inputuser;
    int score;
    cout<<"Enter your Name    ";
    getline(cin,name);
    cout<<endl;
    do
    {
        srand(0);
        int variable=rand()%9 ;
        cout<<"Enter any number in between range 0 to 9       ";
        cin>>inputuser;
        cout<<endl;
        if (inputuser==variable)
        {
            cout<<"CONGRATULATION ! You Win This Round  "<<endl;
            score++;
        }
        else
        {
            cout<<"Sorry , You Loss Try Again "<<endl;
        }
        cout<<"Would You Like to Try Again   Y/N         ";
        cin>>input;
        cout<<endl;
 }while(input!='N');
 cout<<"Your Score is       "<<score<<endl;
cout<<"Game End  "<<endl; 
}

//# Number-Guess-Gamee
Number Guess Game with the help of C++
