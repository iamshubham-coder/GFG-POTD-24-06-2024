# GFG-POTD-24-06-2024
question is :
A matrix is constructed of size n*n and given an integer ‘q’. The value at every cell of the matrix is given as, M(i,j) = i+j, where ‘M(i,j)' is the value of a cell, ‘i’ is the row number, and ‘j’ is the column number. Return the number of cells having value ‘q’.

Note: Assume, the array is in 1-based indexing.


explanation:
--------------
  it is so simple that we need to count the number of element present whsoe value is equal to q given in the question
  
     the idea is to create the matrix whose element is equal to i+j
     i.e for i=1,j=1 mat(i,j)=2 simlarily for i=1,j=2 mat(i,j)=3 and so on;
     i have applied the basic approach to solve this question that i will run two for loop first is inner for loop and second one for the is outer for loop
     and create the matrix;
     and create a condition that if i+j==q then count++;
     and return the value of count;
    
     
     
     code:
------------
class solution{
public:
long long sumMatrix(long long n,long long q)
{
long long count=0;
for(int i=1;i<=n;i++){
for(int j=1;j<=n;j++){
if(i+j==q){
count++;
}
}
}
return count;
}
};

it will runn correctly but if u submit it only pass 2 test case only;
//IF SOMEBODY HAS KNOW TO CORRECT THE CODE THEN PLEASE COMMENT;

i was stucked another solution in my mind 
code2
-----
long long sumMatrix(long long n,long long q)
{
long long count=0;
for(int i=1;i<=n;i++){
int j=q-1;
if(j>=0||j<=n){
count++;
}
}
return count
}
};
//it is also passing few of the test case only

main code i have attached with text file copy it and run the code

