# studious-waddle
Write a program to calculate total “Volume” of different measure (Shapes) such as cube, sphere, cylinder and cone. Write separate functions for each shape and return their volume to main for total calculation. Display total volume in main function.
#include<iostream>
using namespace std;

float volume(int);
float volume(float,int);
float volume(float);
float volume(float,float);


float volume(int a)
{
int cube =  a*a*a;
return cube;
}

float volume(float b, int c)
{
float cylinder = 3.14*b*b*c;
return cylinder;
}

float volume(float d)
{
float sphere = (4/3)*3.14*d*d*d;
return sphere;
}

float volume (float e,float f)
{
float cone=(1*3.14*e*e*f)/3;
return cone;
}
int main()
{

int a;
cout<<"enter the value for side of cube";
cin>>a;
cout<<"volume of cube"<<volume(a)<<endl;

int c; float b;
cout<<"enter radius of cylinder and height of cylinder";
cin>>b>>c;
cout<<"volume of cylinder"<<volume(b,c)<<endl;

float d;
cout<<"enter radius of sphere";
cin>>d;
cout<<"volume of sphere"<<volume(d)<<endl;

float e,f;
cout<<"enter radius and height of cone";
cin>>e>>f;
cout<<"volume of cone"<<volume(e,f)<<endl;
}
