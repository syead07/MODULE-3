# Program-3-a
## C-Module 3
## EX_NO-03)a)-Function
### Date: 19-10-2025
### Name: SYEAD JASLIN
### Register Number:25017223
## AIM:
Write a C program for a function that accepts two numbers to calculate the sum and return the total number of carries.
## ALGORITHM:
1. Start the program.
2. Declare three integer variables: num1, num2, sum, and carry. Initialize sum and carry to 0.
3. Read two integer values (num1 and num2) from the user using scanf.
4. Use a for loop that continues as long as num1 > 0 or num2 > 0:
 
    a. Add the last digits of num1 and num2 and store in sum.

    b. If sum is greater than or equal to 10, increment carry by 1.

    c. Remove the last digit from num1 and num2 by dividing each by 10.

6. After the loop ends, print the value of carry.
7. End the program.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int num1,num2,sum=0,carry=0;
    scanf("%d%d",&num1,&num2);
    for(int i=0;num1>0||num2>0;i++){
        sum=(num1%10)+(num2%10);
        if(sum>=10)
        {
            carry+=1;
        }
        num1/=10;
        num2/=10;
    }
    printf("%d",carry);
}
```
## OUTPUT:
<img width="851" height="395" alt="image" src="https://github.com/user-attachments/assets/e956889f-2fcc-4eed-8cbc-3bc1a0cb6c4a" />

## RESULT:
Thus the program for a function that accepts two numbers to calculate the sum and return the total number of carries has been executed successfully
# Program-3-b
## C-Module 3
## EX_NO-03)b)-Looping
### Date: 19-10-2025
### Name: SYEAD JASLIN
### Register Number:25017223
## AIM:
Create a C program  to check whether the given number is Armstrong number or not.
## ALGORITHM:
1. Start the program.
2. Declare integer variables: num, var, var1, and sum. Initialize sum to 0.
3. Read an integer value num from the user using scanf.
4. Assign the value of num to var.
5. Use a while loop that runs as long as var is not equal to 0:

    a. Extract the last digit of var using var % 10 and store it in var1.

    b. Add the cube of var1 to sum using pow(var1, 3).

    c. Remove the last digit from var by dividing it by 10.

6. After the loop, check if sum is equal to num:

   a. If true, print that num is an Armstrong number.

    b. If false, print that num is not an Armstrong number.

7. End the program.

## PROGRAM:
```
#include<stdio.h>
#include<math.h>
int main()
{
    int num,var,var1,sum=0;
    scanf("%d",&num);
    var=num;
    while(var !=0)
    {
      var1=var%10;
      sum+=pow(var1,3);
      var/=10;
    }
    if(num==sum)
    printf("%d is armstrong number",num);
    else
    printf("%d is not a armstrong number",num);
}
```
## OUTPUT:
<img width="854" height="305" alt="Screenshot 2025-10-19 221532" src="https://github.com/user-attachments/assets/b8561f63-0069-4eb8-b33b-79cd625732c0" />

## RESULT:
Thus the program to check whether the given number is Armstrong number or not has been executed successfully
# Ptogram-3-c
## C-Module 3
## EX_NO-03)c)-ARRAY
### Date: 19-10-2025
### Name: SYEAD JASLIN
### Register Number:25017223
## AIM:
Write a program in C to read n number of values in an array and display it in reverse order.
## ALGORITHM:
1. Start the program.
2. Declare an integer variable n to store the size of the array.
3. Read the value of n from the user using scanf.
4. Declare an integer array of size n.
5. Use a for loop from 0 to n-1 to read n elements into the array using scanf.
6. Use another for loop from n-1 down to 0 to print the elements of the array in reverse order.
7. End the program.
## PROGRAM:
```
#include <stdio.h>

int main()
{
    int n, i;
    scanf("%d",&n);
    int a[n];
    for(i=0;i<n;i++)
    {
        scanf("%d",&a[i]);
}
    for(i=n-1;i>=0;i--)    
        printf("%d ",a[i]);

    return 0;
}
```
## OUTPUT:
<img width="845" height="430" alt="Screenshot 2025-10-19 222108" src="https://github.com/user-attachments/assets/6aae3495-0431-4a2e-bd0e-6ae15394112b" />

## RESULT:
Thus the program to read n number of values in an array and display it in reverse order has been executed successfully
# Program-3-d
## C-Module 3
## EX_NO-03)d)-ARRAY
### Date: 19-10-2025
### Name: SYEAD JASLIN
### Register Number:25017223
## AIM:
Write a C program to delete first element in an array
## ALGORITHM:
1. Start the program.
2. Declare an integer array of size 11.
3. Use a for loop from 0 to 10 to read 11 elements into the array using scanf.
4. Use another for loop from index 2 to 10 to print the elements of the array starting from the 3rd element.
5. End the program.
## PROGRAM:
```
#include<stdio.h>
int main()
{
    int a[11];
    for(int i=0;i<11;i++)
    {
        scanf("%d",&a[i]);
    }
    for(int j=2;j<11;j++)
    {
        printf("%d ",a[j]);
    }
}
```
## OUTPUT:
<img width="833" height="260" alt="Screenshot 2025-10-19 222944" src="https://github.com/user-attachments/assets/7c7e46e1-d85a-4343-864e-5008d9b51f48" />

## RESULT:
Thus the program to delete first element in an array has been executed successfully
# Program-3-e
## C-Module 3
## EX_NO-03)e)-ARRAY
### Date: 19-10-2025
### Name: SYEAD JASLIN
### Register Number:25017223
## AIM:
Write a C Program to Print the sum, count of even & odd Numbers in an Array
## ALGORITHM:
1. Start the program.
2. Declare integer variables: num, sum, odd, and even. Initialize sum, odd, and even to 0.
3. Read an integer value num from the user using scanf.
4. Declare an integer array of size num.
5. Use a for loop from 0 to num-1 to read num elements into the array using scanf.
6. Use a for loop from 0 to num-1 to calculate the sum of all array elements and store it in sum.
7. Use another for loop from 0 to num-1 to count:

    a. Even numbers and increment the even counter.

    b. Odd numbers and increment the odd counter.

9. Print the total sum, the count of even numbers, and the count of odd numbers.
10. End the program.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int num,sum=0,odd=0,even=0;
    scanf("%d",&num);
    int a[num];
    for(int i=0;i<num;i++)
    {
        scanf("%d",&a[i]);
    }
    for(int j=0;j<num;j++)
    {
        sum+=a[j];
    }
    for(int i=0;i<num;i++)
    {
        if(a[i]%2==0)
        even+=1;
        else
        odd+=1;
    }
    printf("Total Sum: %d\n",sum);
    printf("Even numbers: %d\n",even);
    printf("Odd numbers: %d\n",odd);

    
}
```
## OUTPUT:
<img width="839" height="303" alt="Screenshot 2025-10-19 223306" src="https://github.com/user-attachments/assets/d06ba6eb-3cdc-4f64-b337-56e95da00cf4" />

## RESULT:
Thus the program to Print the sum, count of even & odd Numbers in an Array has been executed successfully
