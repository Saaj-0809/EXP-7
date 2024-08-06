# EXP-7
# EXP-1
## AIM: To study and implement C++ Arrays and Strings

## SOFTWARE USED: 

VS CODE

## THEORY:

An array stores a fixed-size sequential collection of elements of the same type. All arrays consist of contiguous memory locations. The lowest address corresponds to the first element and the highest address to the last element To declare an array in C++, we must specify the type of elements and the number of elements required by an array −: type arrayName [ array_size ] You can initialize C++ array elements either one by one or using a single statement as follows −: int arr[5] = {1000, 2, 3, 17, 50} Arrays are used to store multiple values in a single variable, instead of declaring separate variables for each value.

## CODE 1: Creating Array Declaration

#include<iostream>
using namespace std;

int main()
{
    int array1[5] = {1,6,10,34,3}, array2[3] = {2,8,4}, array3[2] = {5,6};

    cout<<"traditional method"<<endl;
    for (int i=0;i<3;i++)
    {
        cout<<array1[i]<<" "<<endl;
    }

    cout<<"modern method"<<endl;
    for(int j : array2)
    {
        cout<<j<<" ";
    }
    return 0;
}

## OUTPUT1:

<img width="842" alt="image" src="https://github.com/user-attachments/assets/75089078-8226-46f2-a4d5-161f388bc5a4">

## CODE 2: Reversing An Array

#include<iostream>
using namespace std;

int main() 
{
    int n, i, j=0, k, l, temp;
    cout<<"Enter size of array: ";
    cin>>n;
    int a1[n], a2[n];

    for(i=0;i<5;i++) 
    {
        cout<<"Enter element-"<<i+1<<": ";
        cin>>a1[i];
    }
    cout<<"\nArray given by user: ";
    for(l=0;l<5;l++) 
    {
        cout<<a1[l];
    }
    cout<<endl;
    for(k=4;k>=0;k--) 
    {
        temp = a1[k];
        a2[j] = temp;
        j++;
    }
    cout<<"Reversed array: ";
    for(l=0;l<5;l++) {
        cout<<a2[l];
    }
}

## OUTPUT2:

<img width="839" alt="image" src="https://github.com/user-attachments/assets/44a08fbb-1866-4017-bc6a-b25cb3859f8b">
