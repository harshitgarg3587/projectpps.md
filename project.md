 ![Gndec Logo](https://github.com/harshitgarg3587/images/blob/master/gndec_image.png)
 # PROGRAMMING FOR PROBLEM SOLVING ESC -18105
 
 ## My Programs
|                         |    |
| --------------------   | --------------  |
| Submitted by           | Harshit Garg    |
| Roll Number            | 1921040        |
| Branch                 | ITA2          |
| Submitted to           | Er. RANJODH KAUR| 
___________________________________

|  S.No. |          Program Name                  |
| -------| --------------  |
| 1.     | Experience of Employees   |
| 2.     | Check whether given no. is even or odd                           |
| 3.     | Construct a basic calculator using switch case          |
| 4.     | Check whether given no. is positive or negative| 
| 5.     | Check whether given no. is prime or not| 
| 6.     | Print the table of entered no. using for loop|
| 7.     | Convert Fahrenheit to Celsius|
| 8.     | Add 100 to each element of an array|
| 9.     | Print sum of all the elements of an array| 
| 10.     | Multiply two functions using an array| 
| 11.     | Er. RANJODH KAUR| 
| 12.     | Er. RANJODH KAUR| 
| 13.     | Er. RANJODH KAUR| 
| 14.     | Er. RANJODH KAUR| 
| 15.     | Er. RANJODH KAUR| 

```c
 #include<stdio.h>
int main()
{
int n,sum=0,exp;
printf("Enter number of employeers:");
scanf("%d",&n);
for(int i=1;i<=n;i++)
{
printf("Enter experience of %d th employeers:",i);
scanf("%d",&exp);
sum=sum+exp;
}
printf("%d\n",sum);
return 0;
}
```
![](https://github.com/harshitgarg3587/images/blob/master/employer.png)
```c
#include<stdio.h>
int main()
{

int  num;
printf("Enter any number:");
scanf("%d",&num);

if (num%2==0)
printf("Given number %d is Even \n",num);
else
printf("Given number %d is Odd \n",num);

return 0;
}
```
![](https://github.com/harshitgarg3587/images/blob/master/odd_even.png)
```c
#include<stdio.h>

void main()
{
  int a,b;
  char op;
  printf("Enter two integer values: ");
  scanf("%d%d", &a,&b);
  fflush(stdin);
  printf("Enter a operand + or - or * or / or %");
  scanf("%c",&op);
  switch(op)
 {
  
   case '+' :
       printf("Result is: %d",(a+b));
       break;
  
  case  '-' :
      printf("Result is: %d",(a-b));
      break;
  
  case  '*' :
      printf("Result is: %d",(a*b));
      break;
  
  case  '/' :
     printf("Result is:  %d",(a/b));
      break;
  
  case '%':
     printf("Result is:  %d",(a%b));
     break;

  default:
     printf("Invalid operand!");
  
}
  
}
    ```
    ![](https://github.com/harshitgarg3587/images/blob/master/calculator.png)
```c
    #include<stdio.h>

int main()
{

int num;
printf("Enter any number: \n");
scanf("%d",&num);

if(num>0)
printf("%d is positive number \n",num );

else if(num<0)
printf("%d is negative number \n",num );

else
printf("You have entered value zero \n");

return 0;
}
```
![](https://github.com/harshitgarg3587/images/blob/master/prime.png)
```c
#include<stdio.h>
int main()
{
int last;
printf("Enter number:");
scanf("%d",&last);
int prime,range=0;
for(int a=2;a<last;a++)
{
 prime=0;
  for(int i=2;i<last;i++)
  {
if(last%i==0)
{
prime=prime+1;
printf("No\n");
break;
}
}
if(prime==0)
{
printf("Yes\n");
break;
}
break;
}
return 0;
}
```
![](https://github.com/harshitgarg3587/images/blob/master/table.png)

```c
#include<stdio.h>
int main()
{
int i,j;
printf("Table of:");
scanf("%d\n",&j);

for(i=0;i<=10;i++) 
printf("%d x %d = %d\n",j,i,j*i);

return 0;
}
```
```c
#include<stdio.h>
int main()
{
int i,j;
printf("Table of:");
scanf("%d\n",&j);
if(j%2==0)
{
for(i=0;i<=10;i++)
printf("%d X  %d  =  %d\n",j,i,j*i);
}
else
{
printf("Number is not even\n");
}

return 0;
}
```

```c
#include<stdio.h>

int main()
{
 float celcius,fehrenheit;

printf("Please enter the temperature in fehrenheit: \n");
scanf("%f",&fehrenheit);
 
celcius=(fehrenheit-32)*5/9;

printf("\n %.2f fehrenheit= %.2f celcius \n", fehrenheit,celcius);

return 0;
}
```
```c
#include<stdio.h>

int main()
{
 int n[10];
 int i,j;

 for(i=10;i<10;i++)
{
  n[i]=i+100;
}
 for(j=0;j<10;j++)
{
 printf( "Element[%d]= %d\n",j,n[j] );
}
 return 0;
}
```
```c
#include<stdio.h>
int main()
{
 int a,b, result, n, i;
 printf("Enter the number of terms: ");
 scanf("%d", &n);

 a=0;
 b=1;

 for(i=1; i<=n; i++)
{
   printf("%d\n",a);
   result=a+b;
   a=b;
   b=result;
}
}
```
![](https://github.com/harshitgarg3587/images/blob/master/multiply.png)
```c
#include<stdio.h>
float multi(float a,float b);
int main()
{
 float m,n;
 printf("\n Please enter a number : \n");
 scanf("%f",&m);
 printf("\n Please add another number\n");
 scanf("%f",&n);

float result=multi(m,n);
printf("result is %.5f\n",result);
}

float multi(float a,float b)
{
float multiple=a*b;
return(multiple);
}
```
![](https://github.com/harshitgarg3587/images/blob/master/pyramid.png)
```c
#include<stdio.h>
int main()
{
int n,i,j;
printf("Enter number of rows you want to print for pyramid:\n");
scanf("%d",&n);

for(i=1;i<=n;i++)
{
for(j=1;j<=2*n-1;j++)
{
if(j>=n-(i-1) && j<=n+(i-1))
printf("*");
else
printf(" ");
}
printf("\n");
}
return 0;
}
```
```c
#include<stdio.h>
int main(){
int  a,b,i,hcf;
printf("Enter 1st integer:\n");
scanf("%d",&a);
printf("enter 2nd intger:\n");
scanf("%d",&b);

for(int i=1;i<=a||i<=b;i++)
{
if(a%i==0 && b%i==0)
hcf=i;
}
printf("hcf=%d",hcf);

return 0;
}
```
```c
#include<stdio.h>
int main(){
int  a,b,i,lcm,gcd;
printf("Enter 1st integer:\n");
scanf("%d",&a);
printf("enter 2nd intger:\n");
scanf("%d",&b);
printf("\n");

for(int i=1;i<=a&&i<=b;i++)
{
if(a%i==0 && b%i==0)
gcd=i;
}
lcm=(a*b)/gcd;
printf("lcm=%d",lcm);

return 0;
}
```
```c
#include<stdio.h>
int main(){
int m,n,p,q;
printf("enter number of rows of 1st matrix: ");
scanf("%d",&m);
printf("enter number of columns of 1st matrix: ");
scanf("%d",&n);
printf("enter number of rows of 2nd matrix: ");
scanf("%d",&p);
printf("enter number of columns of 2nd matrix: ");
scanf("%d",&q);

if(n==p){
//for matrix 1
puts("\n\t matrix 1");
int matrix1[m][n];
// input for matrix 1
for(int i=1;i<=m;i++){
for(int j=1;j<=n;j++){
printf("enter value at %dth row and %dth column : ",i,j);
scanf("%d",&matrix1[i][j]);
}}
// output for matrix 1
puts("\nmatrix 1 is -->");
for(int i=1;i<=m;i++){
for(int j=1;j<=n;j++){
printf("%d\t",matrix1[i][j]);
if(j==n)
printf("\n");}}

//matrix 2
int matrix2[p][q];

puts("\n\t matrix 2");
// input for matrix 2
for(int k=1;k<=p;k++){
for(int l=1;l<=q;l++){
printf("enter value at %dth row and %dth column : ",k,l);
scanf("%d",&matrix2[k][l]);
}}
// output for matrix 2
puts("\nmatrix 2 is -->");
for(int k=1;k<=p;k++){
for(int l=1;l<=q;l++){
printf("%d\t",matrix2[k][l]);
if(l==q)
printf("\n");}}

//multiplication of both matrices
int matrix[m][q];
int sum=0;
//multiplication
for(int a=1;a<=m;a++){
for(int b=1;b<=q;b++){
for(int c=1;c<=p;c++){
sum =sum + matrix1[a][c]*matrix2[c][b];}
matrix[a][b]=sum;
sum=0;}}
//output for matrix 
puts("\n\t product of two matrices is -->");
for(int a=1;a<=m;a++){
for(int b=1;b<=q;b++){
printf("%d\t",matrix[a][b]);
if(b==q)
printf("\n");
}}
}
return 0;
}
```
```c
#include<stdio.h>
int main()
{
int arra[5]={1,5,8,2,7};
int c;
printf("enter the number you want to check");
scanf("%d",&c);
for(int i=0;i<5;i++)
{
if(c==arra[i])
{printf("yes");}
else
printf("no");
}
return 0;}
```
```c
#include<stdio.h>
int main(){
int no,n,r,c,sum=0;
printf("enter  a number:\n");
scanf("%d",&n);
no=n;
while(n>0)
{
r=n%10;
c=r*r*r;
 sum=sum+c;
n=n/10;
}
if(no==sum)
printf("the given number %d is an armstrong number\n",no);
if(no!=sum)
printf("the given number %d is not an armstrong number\n",no);
return 0;
}
```
```c
#include<stdio.h>
int sum(int c);

int  main()
{

int a,b;
printf("please enter a number to calculate the sum of digits:\n");
scanf("%d",&a);
b=sum(a);
printf("%d\n",b);
}

int sum(int c)
{
int sum1=0,n;
while(c!=0)
{
sum1=sum1+c%10;
c=c/10;


}
return sum1;
}
```
```c
#include<stdio.h>
int avg(int a,int  b,int c,int d,int e);
int main()
{
int a,b,c,d,e,f;
printf("enter 5 numbers:\n");
scanf("%d %d %d %d %d",&a,&b,&c,&d,&e);
f=avg(a,b,c,d,e);
printf("avg is %d",f);
}
int avg(int a,int b,int c,int d,int e)
{
int  ans;
ans=(a+b+c+d+e)/5;
//printf("the average of entered 5 numbers %3.f %3.f %3.f %3.f %3.f is %3.f",a,b,c,d,e,ans);
return ans;
}
```
```c
#include<stdio.h>
int main(){
printf("use operators + ,-,*,/\n");
puts("+ FOR ADDITION");
puts("- FOR SUBTRACTION");
puts("* FOR MULTIPLICATION");
puts("/ FOR DIVIDING");

int n,i;
printf("\n\nhow many times you want to perform operation  ");
scanf("%d",&n);
int a,d;
char c;
int sum;
printf("enter the number  ");
scanf("%d",&a);
printf("enter operator  ");
scanf(" %c",&c);
if(c=='+'||c=='-'||c=='*'||c=='/'){
for(int i=1;i<=n;i++)
{if(i==1){
printf("enter another operatant  ");
scanf("%d",&d);
if(c=='+')
sum=d+a;
if(c=='-')
sum=d-a;
if(c=='*')
sum=d*a;
if(c=='/')
sum=d/a;
}
if(i>1){
puts(" ");
printf("enter another operator ");
scanf(" %c",&c);
if(c=='+'||c=='-'||c=='*'||c=='/'){
printf("enter other operand ");
scanf("%d",&a);
if(c=='+')
sum=sum+a;
if(c=='-')
sum=sum-a;
if(c=='*')
sum=sum*a;
if(c=='/')
sum=sum/a;

}
else
printf("enter correct operator");
}}
printf("answer is %d\n",sum);

}

else
printf("enter correct operator");
return 0;
}
```
