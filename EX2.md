# Ex.No:2  
# Ex.Name: Expression Tree Construction and Evaluation  

## Date:  

## Aim:  
To write a C++ program to **construct an Expression Tree** from an infix/prefix expression and evaluate the expression.  

## Algorithm:  
1. Start the program.  
2. Define a node structure with:  
   - `data` (operand/operator)  
   - `left` and `right` child pointers.  
3. Read the expression (given in prefix form).  
4. For each character/token in the prefix expression:  
   - If it is an operand, create a new node and push it to the stack.  
   - If it is an operator, pop two nodes from the stack, make them children, and push the new node back.  
5. After processing, the stack contains the root of the expression tree.  
6. Evaluate the expression tree recursively:  
   - If the node is an operand, return its value.  
   - If the node is an operator, evaluate its left and right subtrees and apply the operator.  
7. Display the evaluated result.  
8. Stop the program.  

## Program:
```cpp
#include<iostream>
using namespace std;
class A{
    public:
    int a,b;
    int x,y,z;
};
class B:public A{
    public:
    void read1(){
        cin>>a>>b;
    }
    void dis1(){
        cout<<"Sum of two Numbers="<<a+b<<endl;
    }
};
class C: public A{
    public:
    void read2(){
        cin>>x>>y>>z;
    }
    void dis2(){
        cout<<"Sum of three Numbers="<<x+y+z;
    }
};
int main(){
    B gojo;
    gojo.read1();
    gojo.dis1();
    C jojo;
    jojo.read2();
    jojo.dis2();
}
```
## Output:
```
Input:
Prefix : /*+314+-952

Output:
2.66667


Input:
Prefix : +3*+592

Output:
31
```
 ## Result:
<img width="866" height="494" alt="image" src="https://github.com/user-attachments/assets/b7a9fff7-1bb0-4177-abd6-ddf07d07f852" />


