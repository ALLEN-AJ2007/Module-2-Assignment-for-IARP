# Module-2-Assignment-for-IARP

# PROGRAMS AND OUTPUTS

# 1)Print square number pattern of one and zero with one at odd row and zero at even row using loop in C programming
```
#include <stdio.h>

int main()
{
  int row,col;
  printf("Enter the no of rows and cols :");
  scanf("%d %d",&row,&col);
  for(int i=1;i<=row;i++)
  {
      for(int j=1;j<=col;j++)
      {
          if(i%2!=0)
          printf("1");
          else
          printf("0");
      }
      printf("\n");
  }
}
```
<img width="382" height="163" alt="Screenshot 2025-10-19 154829" src="https://github.com/user-attachments/assets/0b2f6576-bbf2-4f8d-8b13-2b8871018b33" />
# 2)write a c program to print hollow triangle pattern 

```
#include <stdio.h>

int main()
{
  int row;
  printf("Enter the no of rows :");
  scanf("%d",&row);
  for(int i=1;i<=row;i++)
  {
      for(int j=1;j<=i;j++)
      {
         if(i==1||j==1||j==i||i==row)
         printf("*");
         else
         printf(" ");
      }
      printf("\n");
  }
}
```
<img width="436" height="248" alt="Screenshot 2025-10-19 155518" src="https://github.com/user-attachments/assets/8754d46b-4446-43a4-aa10-35a21b4bc326" />

#3)Write a C program to generate Fibonacci sequence of n numbers using function, with arguments & without return type.
```
#include <stdio.h>
void fib(int N)
{
    int num1=0,num2=1,num3;
    if(N==1)
    printf("%d",num1);
    else if(N==1)
    printf("%d %d",num1,num2);
    else{
    printf("%d %d",num1,num2);
    for(int i=1;i<=N-2;i++)
    {
        num3=num1+num2;
        printf(" %d ",num3);
        num1=num2;
        num2=num3;
    }
    }
    
}

int main()
{
    int n;
  printf("Enter the no of digits to produce output :");
  scanf("%d",&n);
  fib(n);
}
```
<img width="750" height="160" alt="Screenshot 2025-10-19 160404" src="https://github.com/user-attachments/assets/cc133462-e123-4124-bd87-b0b21ea5607c" />

# 4)Write a C program to check the input entered by the user is palindrome or not using while loop.
```
#include<stdio.h>
int main(){
    int a,rev=0,copy;
    scanf("%d",&a);
    copy=a;
    while(copy>0){
            rev=rev*10;
            rev=rev+(copy%10);
            copy/=10;
    }
    if(rev==a){
        printf("Palindrome Number");
    }
    else{
        printf("Not a Palindrome Number");
    }
            

}
```
<img width="398" height="152" alt="Screenshot 2025-10-19 160733" src="https://github.com/user-attachments/assets/e73f741d-b578-40c6-a8c4-1ffe37684852" />

#5)Write a C program for finding the factorial of a given number using function without return type with arguments.
```
#include <stdio.h>

void fact(int num) {
    int fact = 1;

    if (num < 0) {
        printf("Factorial is not defined for negative numbers.\n");
        return;
    }

    for (int i = 1; i <= num; i++) {
        fact *= i;
    }

    printf("Factorial value is: %d\n", fact);
}

int main() {
    int a;
    scanf("%d", &a);
    fact(a);
}

```
<img width="412" height="191" alt="Screenshot 2025-10-19 161535" src="https://github.com/user-attachments/assets/89ff90e3-9349-4b44-af3e-322d948f9698" />





