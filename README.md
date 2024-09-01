# Experiment-
## AIM:
To study and implement C++ arrays and strings.
## THEORY:
C++ arrays are collections of elements with the same types that are stored together in contiguous memory. They are declared by specifying the element type followed by square brackets containing the number of elements. In C++, arrays start counting from zero, so the first element is at index zero, the second at index one, and so on. Arrays in C++ have fixed sizes that must be determined at compile time.
In C++, strings can be managed using C-style strings or by using the `string` class from the Standard Library. In this programming language, strings are sequences of characters terminated by a null character (`\0`). Operations on C-style strings are performed using functions from the C standard library, such as `strlen`, `strcpy`, and `strcat`.
### code:
a
#include <iostream>  
using namespace std;
int main()
{
    int n = 0,i = 0;
    int a[n];
    cout<<"Enter size of array: ";
    cin>>n;
    for(i = 0; i < n;i++)
    {
        cout<<"Enter element no. "<< i <<" of  the array: ";
        cin>>a[i];

    }
    cout<<endl;
    cout<<"The array defined by the user: "<<endl;
    cout<<"{";
    for(i = 0; i < n;i++)
    {
        cout<<a[i]<<" ";

    }
    cout<<"}";
    cout<<endl;

    return 0;
}

b
#include <iostream>
using namespace std;
int main()
{
    int n = 0,i = 0;
    int a[n];
    cout<<"Enter size of array: ";
    cin>>n;
    for(i = 0; i < n;i++)
    {
        cout<<"Enter element no. "<< i+1 <<" of  the array: ";
        cin>>a[i];

    }
    cout<<endl;
    cout<<"The array defined by the user: "<<endl;
    for(i = 0; i < n;i++)
    {
        cout<<a[i]<<" ";

    }
    cout<<endl;

    cout<<"The array reversed: "<<endl;
    cout<<"{ ";
    for(i = n-1 ; i > -1 ;i--)
    {
        cout<<a[i]<<" ";

    }
    cout<<"}";
    cout<<endl;

    return 0;
}
c
#include <iostream>
using namespace std;
int main()
{
    int n = 0,i = 0;
    int num = 0, co = 0, flag = 0;
    int a[n];
    cout<<"Enter size of array: ";
    cin>>n;
    for(i = 0; i < n;i++)
    {
        cout<<"Enter element no. "<< i+1 <<" of  the array: ";
        cin>>a[i];
    }
    cout<<endl;
    cout<<"Enter the number you want to check: ";
    cin>>num;
    for(i = 0; i < n;i++)
    {
        if(a[i] == num)
        {
            co++;
            flag++;

        }
    }
    if (flag == 0)
    {
        cout<<"Element was not found.";
    }
    else
    {
        cout<<"The element was found "<<co<<" times.";
    }

}
d
#include <iostream>
using namespace std;
int main()
{
    int n = 0,i = 0;
    int a[n];
    int num = 0, maxi = 0, mini = a[0];
    
    cout<<"Enter size of array: ";
    cin>>n;
    for(i = 0; i < n;i++)
    {
        cout<<"Enter element no. "<< i+1 <<" of  the array: ";
        cin>>a[i];
    }
    cout<<endl;
    for(i = 0; i < n;i++)
    {
        if(a[i] > maxi)
        {
            maxi = a[i];
        }
        if(a[i] < mini)
        {
            mini = a[i];
        }
    }
    cout<<"Maximum value amongst the elements are: "<<maxi<<endl;
    cout<<"Minimum value amongst the elements are: "<<mini<<endl;


}
e
#include <iostream>
using namespace std;
int main()
{
    int n = 0,i = 0;
    int num = 0, sum = 0, avg = 0;
    int a[n];
    cout<<"Enter size of array: ";
    cin>>n;
    for(i = 0; i < n;i++)
    {
        cout<<"Enter element no. "<< i+1 <<" of  the array: ";
        cin>>a[i];
    }
    cout<<endl;
    for(i = 0; i < n;i++)
    {
        sum = sum + a[i];
    }
    avg = sum/n;
    cout<<"Sum of elements: "<<sum<<endl;
    cout<<"Average of elements: "<<avg<<endl;


}
f
#include <iostream>
#include <string>
using namespace std; 

int main()
{
    //printing a string
    string s;
    cout<<"Enter a word: ";
    cin>>s;
    cout<<"Word entered by user is: "<<s<<endl;
    cout<<endl;

    //concatenation
    string s1,s2;
    cout<<"Enter a word: ";
    cin>>s1;
    cout<<"Enter another word: ";
    cin>>s2;
    cout<<"Concatenated word is: "<<s1+s2<<endl;
    cout<<endl;

    //reverse
    string s3;
    int i = 0;
    cout<<"Enter a word: ";
    cin>>s3;
    cout<<"Reverse String: ";
    for (i = s3.length()-1; i>=0; i-- )
    {
        cout<<s3[i];
    }
    cout<<endl;
    cout<<endl;

    //palindrome.
    string s4,rs;
    int j = 0;
    cout<<"Enter a word: ";
    cin>>s4;
    for (j = s4.length()-1; j>=0; j-- )
    {
        rs = rs + s4[j];
    }
    if (rs == s4)
    {
        cout<<"It is a palindrome."<<endl;
    }
    else
    {
        cout<<"It is not a palindrome."<<endl;   
    }
    cout<<endl;
}

### Output
a) ![image](https://github.com/user-attachments/assets/b761c17e-d686-4528-a085-d4381d8bc032)
b)![image](https://github.com/user-attachments/assets/88b628c3-a150-4076-a197-22282ea66969)
c)![image](https://github.com/user-attachments/assets/7f88b1c0-3e8f-43e1-a908-e9ed19417abe)
d)![image](https://github.com/user-attachments/assets/f136e7e1-3faa-4a52-9a4d-434ebe19378f)
e)![image](https://github.com/user-attachments/assets/9456e549-beaf-4213-b7a2-e2dabd22dc3e)
f)![image](https://github.com/user-attachments/assets/af59ed80-60ea-4062-b18a-4a1e20106031)

## Conclusion:
→ We learnt the use case of arrays in C++.
→ We learnt how to perform basic string manipulations in C++.






