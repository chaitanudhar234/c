
#include<stdio.h>
int main()
{
	float amt,creditamt,debitamt;
	char ch;
	printf("Enter initial amount\n");
	scanf("%f",&amt);
	printf("Enter\nc for credit\nd for debit\nb for balance\n");
	scanf("\n%c",&ch);
	switch(ch)
	{		
		case 'c':
			printf("Enter credit amount\n");
			scanf("%f",&creditamt);
			amt=amt+creditamt;
			printf("New Amount=%f",amt);
			break;
		case 'd':
			printf("Enter debit amount\n");
			scanf("%f",&debitamt);
			if(amt>=debitamt)
			{
			amt=amt-debitamt;
			printf("New Amount=%f",amt);
		    }
		    else
		    {
		    printf("Insufficient amount");
			}
			break;
		case 'b':
			printf("Amount in your account=%f",amt);
			break;
		default:
			printf("Invalid input!!");
	}
}

#include<stdio.h>
int main()
{
	float x,y;
	char ch;
	printf("Enter first number\n");
	scanf("%f",&x);
	printf("Enter second number\n");
	scanf("%f",&y);	
	printf("Enter\n+ for add\n- for sub\n* for multiply\n/ for div\n");
	scanf("\n%c",&ch);
	switch(ch)
	{		
		case '+':
			printf("Add=%f",(x+y));
			break;
		case '-':
			printf("Sub=%f",(x-y));
			break;
		case '*':
			printf("Multiply=%f",(x*y));
			break;
		case '/':
			printf("Div=%f",(x/y));
			break;
		default:
			printf("Invalid input!!");
	}
}

#include<stdio.h>
int main()
{
	float amt,creditamt,debitamt;
	char ch;
	printf("Enter initial amount\n");
	scanf("%f",&amt);
	printf("Enter\nc for credit\nd for debit\nb for balance\n");
	scanf("\n%c",&ch);
	switch(ch)
	{		
		case 'c':
			printf("Enter credit amount\n");
			scanf("%f",&creditamt);
			amt=amt+creditamt;
			printf("New Amount=%f",amt);
			break;
		case 'd':
			printf("Enter debit amount\n");
			scanf("%f",&debitamt);
			if(amt>=debitamt)
			{
			amt=amt-debitamt;
			printf("New Amount=%f",amt);
		    }
		    else
		    {
		    printf("Insufficient amount");
			}
			break;
		case 'b':
			printf("Amount in your account=%f",amt);
			break;
		default:
			printf("Invalid input!!");
	}
}

#include<stdio.h>
int main()
{
	int no,f=1;
	printf("Enter any number\n");
	scanf("%d",&no);
	for(int i=1;i<=no;i++)
	{
		f=f*i;
	}
	printf("Factorial=%d",f);
}

#include<stdio.h>
int main()
{
	int no,f=1;
	printf("Enter any number\n");
	scanf("%d",&no);
	printf("Factor is given below\n");
	for(int i=1;i<=no;i++)
	{
		if(no%i==0)
		printf("%d ",i);
	}
}

#include<stdio.h>
int main()
{
	int b,p,f=1;
	printf("Enter base\n");
	scanf("%d",&b);
	printf("Enter power\n");
	scanf("%d",&p);
	for(int i=1;i<=p;i++)
	{
	f=f*b;	
	}
	printf("Result=%d",f);
}

#include<stdio.h>
int main()
{
int no1,no2;
printf("Enter first number\n");
scanf("%d",&no1);
printf("Enter second number\n");
scanf("%d",&no2);

 for(int i=1;;i=i+1)
 {
 	if(i%no1==0&&i%no2==0)
 	{
 	  printf("LCM of %d and %d is %d",no1,no2,i);
	   break;	
	}
 }
}

#include<stdio.h>
int main()
{
int no1,no2,m=1;
printf("Enter first number\n");
scanf("%d",&no1);
printf("Enter second number\n");
scanf("%d",&no2);
 for(int i=1;i<=no1;i=i+1)
 {
 	if(no1%i==0&&no2%i==0)
 	{
 	 m=i; 	
	}
 }
 printf("HCF of %d and %d is %d",no1,no2,m);
}

#include<stdio.h>
int main()
{
	int no,m=0;
	printf("Enter any number\n");
	scanf("%d",&no);
	for(int i=2;i<=no-1;i++)
	{
		if(no%i==0)
		{
			printf("Number is not  Prime");
			m=1;
			break;
		}
	}
	if(m==0)
	printf("Number is prime");
}

#include<stdio.h>
int main()
{
	int n,m,num;
	printf("Enter any number upto you want to print prime number\n");
	scanf("%d",&num);
	printf("Prime number between 1 and %d is given below\n",num);
	for(int i=1;i<=num;i++)
	{
		n=i,m=0;
		for(int j=2;j<=n-1;j++)
	    {
		if(n%j==0)
		  {
			m=1;
			break;
		  }
	    }
	if(m==0)
	printf("%d ",n);
	}
}

#include<stdio.h>
int main()
{
	int i=1;
	int *p;
	p=&i;
	while(*p<=10)
	{
		printf("%d\n",*p);
		(*p)++;
	}
}

#include<stdio.h>
int main()
{
	for(char ch='A';ch<='Z';ch++)
	{
		printf("%c ",ch);
    }
}

#include<stdio.h>
int main()
{
	for(int i=65;i<=90;i++)
	{
		printf("%c ",i);
    }
}

#include<stdio.h>
int main()
{
	for(char ch='a';ch<='z';ch++)
	{
		printf("%c ",ch);
    }
}

#include<stdio.h>
int main()
{
	for(int i=97;i<=122;i++)
	{
		printf("%c ",i);
    }
}

#include<stdio.h>
int main()
{
	for(char ch='A';ch<='Z';ch++)
	{
		printf("%c=%d\n",ch,ch);
	}
}

#include<stdio.h>
int main()
{
printf("Odd number b/w 1 and 20 is given below\n");
 for(int i=1;i<=20;i=i+2)
 {
 	printf("%d ",i);
 }
}

#include<stdio.h>
int main()
{
	int no;
	printf("Enter any number\n");
	scanf("%d",&no);
	printf("Natural no from 1 to %d in reverse order is given below\n",no);
	for(int i=no;i>=1;i--)
	{
		printf("%d ",i);
	}
}

#include<stdio.h>
int main()
{
	int no,sum=0;
	printf("Enter any number\n");
	scanf("%d",&no);
	printf("Natural no from 1 to %d is given below\n",no);
	for(int i=1;i<=no;i++)
	{
		printf("%d ",i);
		sum=sum+i;
	}
	printf("\nTotal sum=%d",sum);
}

#include<stdio.h>
int main()
{
	int no,b,rev=0,cpy;
	printf("Enter any number\n");
	scanf("%d",&no);
	cpy=no;
	while(no!=0)
	{
		b=no%10;
		rev=rev*10+b;
		no=no/10;
	}
	if(cpy==rev)
	printf("Palindrome");
	else
	printf("Not Palindrome");
}

#include<stdio.h>
int main()
{
	int no,b,sum=0;
	printf("Enter any number\n");
	scanf("%d",&no);
	while(no!=0)
	{
		b=no%10;
		sum=sum+b;
		no=no/10;
	}
	printf("Total sum of digits=%d",sum);
}

#include<stdio.h>
int main()
{
	int i,j;
	for(i=0;i<3;i++) // i=row
	{
		for(j=0;j<3;j++)//i=row
		{
			printf("chaitan");
		}
		printf("\n")
	}
}

#include<stdio.h>
int main()
{
	int i,n;
	//for (imit ; condition; inmcriment)
	for(i=1;i<=10;i++)
	{
		printf("%d\n",i*2);
	}


	printf("enter any num:");
	scanf("%d",&n);
	for(i=0;i<=10;i++)
	{
		printf("%d\n",i*n);
	}
}

#include<stdio.h>
int main()
{
	//exit control loop: it checks condition at the end 
	int i=11;//init
	do
	{
		printf("hello from c...%d\n"i);
		i++; //i+i+1
	}while(i<=10);//condition

	printf("current value of i : %d\n",i);
}

#include<stdio.h>
int main()
{
	int i;
	//for(init ; condition ; inmcriment)
	for(i=1;1<=10;i++)
	{
		printf("hello..welcome to c...%d\n",i);
	}
}

#include<stdio.h>
int main()
{
	int i,arr [5]={10,20,30,40,50}
	printf("array elements :\n");
	for(i=0;i<5;i++)
	{
		printf("%d\n",arr[i]);
	}

	printf("value at index 3: %d\n",arr[3]);
	arr[3]=35
	printf("updated array after ele change :\n");
	for(i=0;i<5;i++)
	{
		printf("%d=d\n",i arr[i]);
	}
}

#include<stdio.h>
int main()
{
	int i,arr[5]={10,20,30,40,50};
	printf("array elements:\n");
	for(i=0;i<5;i++)
	{
		printf("%d\n",arr[i]);
	}

	//access ele
	printf("value at index 3:%d\n",arr[3]);

	//change ele
	arr[3]=35

	printf("updated array after ele change:\n");
	for(i=0;i<5;i++)
	{
		printf("%d=%d\n",i;arr[i]);
	}
}

#include<stdio.h>
int main()
{
	int i arr [5];
	printf("enter array elements:");
	for(i=0;i<5;i++)
	{
		scanf("%d",&arr[i]);
	}

	printf("your array ele:\n");
	for(i=0;i<5;i++)
	{
		printf("d\n",arr[i]);
	}
}

#include<stdio.h>
int main()
{
	int i,numbers[5]={10,20,30,40,50};
	printf("array ele : \n");
	{
		printf("d\n,numbers[i]");
	}
	
	//access ele 
	printf("ele at index 3 : %d\n",numbers[3]);// arr-name [index]
	
	
	//change ele
	numbers[5]=35;
	
	printf("updated array ele:\n");
	for(i=0;i<5;i++)
	{
		printf("%d\n",i,numbers[i]);
	}
}

#include<stdio.h>
int main()
{
	int i,arr[5];
	printf("enter array ele :");
	for(i=0;i<5;i++)
	{
		scanf("%d",&arr[i]);
	}
	printf("array ele :\n");
	for(i=0;i<=5;i++)
	{
		printf("%d\n",arr[i]);
	}
}

#include<stdio.h>
int main()
{
	int i,j,arr[3][3]={1,2,3,4,5,6,7,8,9};
	printf("2d array :\n");
	for(i=0;i<3;i++)//i=row
	{
		for(j=0;j<3;j++) //i=col
	{
		printf("%d",arr[i][j]);
	}
	printf("\n");
	}
	printf("value at r=2,c=1:%d\n,arr[2][1]");
}

#include<stdio.h>
int main()
{
	int i,j,arr[3][3];
	printf("enter array ele :");
	for(i=0;i<3;i++)
	{
		for(j=0;j<3;i++)
		{
			scanf("%d",&arr[i][j]);
		}
	}
	printf("2d array :\n");
	for(i=0;i<3;i++)//i=row
	{
		for(j=0;j<3;j++)//i=col
		{
			printf("%d",arr[i][j]);
		}
		printf("\n");
	}
	
	printf("valude at r=2,c=1 :%d\n",arr[2][1]);
}

#include<stdio.h>
int main()
{
	char name[10]="udhar";
	printf("%s\n",name);
	
	//length
	printf("length of str : %d\n",strlen(name));
	//size of
	printf("sizeof str : %d\n",sizeof(name));
}

#include<stdio.h>
int main()
{
	char name[10]="udhar";
	printf("%s\n",name);
	
	//length
	printf("length of str : %d\n",strlen(name));
	//size of
	printf("sizeof str : %d\n",sizeof(name));//6
	
	
	
	
	char address[20]="chapaner";
	printf("address : %s\n",address);
	printf("size of address : %d\n",sizeof(address));//20
	
	
	//concat
	//strcat(first_data,second_data);
	strcat(name,address);
	printf("updated name aftar concate : %s\n",name);
	printf("updated address after concate : %s\n",address);
}

#include<stdio.h>
int main()
{
	char data[40];
	//strcpy(first_data,second_data);
	strcpy(data,name);
	printf("copied date : %s\n",data);
	
	
	//string char
	printf("string alphabets of address : \n");
	for(i=0;i<strlen(address);i++)
	{
		printf("%d = %c\n", i,address[i]);
	}
	
	//string using loop
	printf("string data of address : \n");
	for(i=0;i<strlen(address)i++)
	{
		printf("%d = %s\n",i,address);
	}
}

#include<stdio.h>
int main()
{
	//user input
	char id[20];
	printf("enter name:");
	for(i=0;i<10;i++);
	{
		scanf("%c",&id[i]);
	}
	
	printf("id : %s",id);
}

#include<stdio.h>
int main()
{
	int f,s;
	printf("enter the value of first number ");
	scanf("%d",&f);
	printf("enter the value of second numbar");
	scanf("%d"&s)
	if(f>s)
	{
		printf("it is smaller then frist\n");
	}
	else if (f>s)
	{
		printf("it is greater than first\n")
	}
	else
	{
		printf("it is same");
	}
}

#include<stdio.h>
int main()
{
	int no;
	printf("enter any no\n")
	scanf("%d",&no);
	switch(no)
	{
		case 1;
		printf("jan");
		break;
		case 2;
		printf("feb");
		break;
		case 3:
		printf("mar");
		defaulf:
		printf("invalide input");
	}
}

#include<stdio.h>
int main()
{
	char ch;
	printf("enetr any alphabet\n");
	scanf("%c",&ch);

	if(ch=='a'||ch=='e'||ch=='i'||ch=='o'||ch=='v')
	{
		printf("vowel");
	}
	else
	{
		printf("consonent");
	}
}

#include<stdio.h>
#include<stringh>
int main()
{
	float a1,a2,a3;
	printf("enter frist angle\n");
	scanf("%f",&a1);
	printf("enter second angle\n");
	scanf("%f",&a2);
	printf("enter third angle\n");
	scanf("%f",&a3);
	if((a1+a2+a3)==180)
	{
		printf("triangle is valid");
	}
	else
	{
		printf("triangle is not valid");
	}
}

#include<stdio.h>
#include<string.h>
int main()
{
	fload sp,cp,profit.loss;
	printf("enter cost price\n");
	scanf("%f",&cp);
	printf("enetr selling price\n");
	scanf("%f"&sp);
	if(so>cp)
	{
		profit=sp-cp;
		printf("prafit is %f rupee",profit);
		{
			elsa
		}
		loss=cp-sp;
		printf("loss is%f rupee"loss);
	}
}

#include<stdio.h>
int main()
{
	flood p;
	printf("enter your perent\n");
	scanf("%F",&p);
	if(p>=)
	{
		printf("frist division");
	}
	else if(p>=45)
	{
		printf("second division");
	}
	else if(p>=33)
	{
		printf("third division");
	}
	else
	{
		printf("fail")
	}
}

#include<stdio.h>
int main()
{
	int a,b,c;
	printf("Enter first number\n");
	scanf("%d",&a);
	printf("Enter second number\n");
	scanf("%d",&b);
	printf("Enter third number\n");
	scanf("%d",&c);
	if(a>b&&a>c)
	{
		printf("%d is greater",a);
	}
	if(b>a&&b>c)
	{
		printf("%d is greater",b);
	}
	if(c>a&&c>b)
	{
		printf("%d is greater",c);
	}
}

#include<stdio.h>
int main()
{
	float p;
	printf("Enter your percent\n");
	scanf("%f",&p);
	if(p>=60)
	{
		printf("First division");
	}
	else if(p>=45)
	{
		printf("Second division");
	}
	else if(p>=33)
	{
		printf("Third division");
	}
	else
	{
		printf("Fail");
	}
}

#include<stdio.h>
int main()
{
	int a,b,c;
	printf("Enter first number\n");
	scanf("%d",&a);
	printf("Enter second number\n");
	scanf("%d",&b);
	printf("Enter third number\n");
	scanf("%d",&c);
	if(a>b&&a>c)
	{
		printf("%d is greater",a);
	}
	else if(b>a&&b>c)
	{
		printf("%d is greater",b);
	}
	else
	{
		printf("%d is greater",c);
	}
}

#include<stdio.h>
int main()
{
	char ch;
	printf("Enter any character\n");
	scanf("%c",&ch);
	if(ch>=65&&ch<=97||ch>=97&&ch<=122)
	{
	printf("It is alphabet");	
	}	
	else if(ch>=48&&ch<=57)
	{
	printf("It is digit");
	}
	else
	{
	printf("It is special symbol");
	}
}

#include<stdio.h>
int main()
{
	int no;
	printf("Enter any number\n");
	scanf("%d",&no);
	switch(no)
	{		
		case 1:
			printf("Monday");
			break;
		case 2:
			printf("Tuesday");
			break;	
		case 3:
			printf("Wednesday");
			break;
		case 4:
			printf("Thrusday");
			break;
		case 5:
			printf("Friday");
			break;
		case 6:
			printf("Saturday");
			break;
		case 7:
			printf("Sunday");
			break;
		default:
			printf("Invalid input");
	}
}

#include<stdio.h>
int main()
{
	char ch;
	printf("Enter any alphabet\n");
	scanf("%c",&ch);
	switch(ch)
	{		
		case 'a':
			printf("vowel");
			break;
		case 'e':
			printf("vowel");
			break;	
		case 'i':
			printf("vowel");
			break;
		case 'o':
			printf("vowel");
			break;
		case 'u':
			printf("vowel");
			break;
		default:
			printf("Consonent");
	}
}

#include<stdio.h>
int main()
{
	char ch;
	printf("Enter any alphabet\n");
	scanf("%c",&ch);
	switch(ch)
	{		
		case 'a':
		case 'e':
		case 'i':
		case 'o':
		case 'u':
			printf("vowel");
			break;
		default:
			printf("Consonent");
	}
}@ -1 +1,931 @@
# c

#include<stdio.h>
int main()
{
	float amt,creditamt,debitamt;
	char ch;
	printf("Enter initial amount\n");
	scanf("%f",&amt);
	printf("Enter\nc for credit\nd for debit\nb for balance\n");
	scanf("\n%c",&ch);
	switch(ch)
	{		
		case 'c':
			printf("Enter credit amount\n");
			scanf("%f",&creditamt);
			amt=amt+creditamt;
			printf("New Amount=%f",amt);
			break;
		case 'd':
			printf("Enter debit amount\n");
			scanf("%f",&debitamt);
			if(amt>=debitamt)
			{
			amt=amt-debitamt;
			printf("New Amount=%f",amt);
		    }
		    else
		    {
		    printf("Insufficient amount");
			}
			break;
		case 'b':
			printf("Amount in your account=%f",amt);
			break;
		default:
			printf("Invalid input!!");
	}
}

#include<stdio.h>
int main()
{
	float x,y;
	char ch;
	printf("Enter first number\n");
	scanf("%f",&x);
	printf("Enter second number\n");
	scanf("%f",&y);	
	printf("Enter\n+ for add\n- for sub\n* for multiply\n/ for div\n");
	scanf("\n%c",&ch);
	switch(ch)
	{		
		case '+':
			printf("Add=%f",(x+y));
			break;
		case '-':
			printf("Sub=%f",(x-y));
			break;
		case '*':
			printf("Multiply=%f",(x*y));
			break;
		case '/':
			printf("Div=%f",(x/y));
			break;
		default:
			printf("Invalid input!!");
	}
}

#include<stdio.h>
int main()
{
	float amt,creditamt,debitamt;
	char ch;
	printf("Enter initial amount\n");
	scanf("%f",&amt);
	printf("Enter\nc for credit\nd for debit\nb for balance\n");
	scanf("\n%c",&ch);
	switch(ch)
	{		
		case 'c':
			printf("Enter credit amount\n");
			scanf("%f",&creditamt);
			amt=amt+creditamt;
			printf("New Amount=%f",amt);
			break;
		case 'd':
			printf("Enter debit amount\n");
			scanf("%f",&debitamt);
			if(amt>=debitamt)
			{
			amt=amt-debitamt;
			printf("New Amount=%f",amt);
		    }
		    else
		    {
		    printf("Insufficient amount");
			}
			break;
		case 'b':
			printf("Amount in your account=%f",amt);
			break;
		default:
			printf("Invalid input!!");
	}
}

#include<stdio.h>
int main()
{
	int no,f=1;
	printf("Enter any number\n");
	scanf("%d",&no);
	for(int i=1;i<=no;i++)
	{
		f=f*i;
	}
	printf("Factorial=%d",f);
}

#include<stdio.h>
int main()
{
	int no,f=1;
	printf("Enter any number\n");
	scanf("%d",&no);
	printf("Factor is given below\n");
	for(int i=1;i<=no;i++)
	{
		if(no%i==0)
		printf("%d ",i);
	}
}

#include<stdio.h>
int main()
{
	int b,p,f=1;
	printf("Enter base\n");
	scanf("%d",&b);
	printf("Enter power\n");
	scanf("%d",&p);
	for(int i=1;i<=p;i++)
	{
	f=f*b;	
	}
	printf("Result=%d",f);
}

#include<stdio.h>
int main()
{
int no1,no2;
printf("Enter first number\n");
scanf("%d",&no1);
printf("Enter second number\n");
scanf("%d",&no2);

 for(int i=1;;i=i+1)
 {
 	if(i%no1==0&&i%no2==0)
 	{
 	  printf("LCM of %d and %d is %d",no1,no2,i);
	   break;	
	}
 }
}

#include<stdio.h>
int main()
{
int no1,no2,m=1;
printf("Enter first number\n");
scanf("%d",&no1);
printf("Enter second number\n");
scanf("%d",&no2);
 for(int i=1;i<=no1;i=i+1)
 {
 	if(no1%i==0&&no2%i==0)
 	{
 	 m=i; 	
	}
 }
 printf("HCF of %d and %d is %d",no1,no2,m);
}

#include<stdio.h>
int main()
{
	int no,m=0;
	printf("Enter any number\n");
	scanf("%d",&no);
	for(int i=2;i<=no-1;i++)
	{
		if(no%i==0)
		{
			printf("Number is not  Prime");
			m=1;
			break;
		}
	}
	if(m==0)
	printf("Number is prime");
}

#include<stdio.h>
int main()
{
	int n,m,num;
	printf("Enter any number upto you want to print prime number\n");
	scanf("%d",&num);
	printf("Prime number between 1 and %d is given below\n",num);
	for(int i=1;i<=num;i++)
	{
		n=i,m=0;
		for(int j=2;j<=n-1;j++)
	    {
		if(n%j==0)
		  {
			m=1;
			break;
		  }
	    }
	if(m==0)
	printf("%d ",n);
	}
}

#include<stdio.h>
int main()
{
	int i=1;
	int *p;
	p=&i;
	while(*p<=10)
	{
		printf("%d\n",*p);
		(*p)++;
	}
}

#include<stdio.h>
int main()
{
	for(char ch='A';ch<='Z';ch++)
	{
		printf("%c ",ch);
    }
}

#include<stdio.h>
int main()
{
	for(int i=65;i<=90;i++)
	{
		printf("%c ",i);
    }
}

#include<stdio.h>
int main()
{
	for(char ch='a';ch<='z';ch++)
	{
		printf("%c ",ch);
    }
}

#include<stdio.h>
int main()
{
	for(int i=97;i<=122;i++)
	{
		printf("%c ",i);
    }
}

#include<stdio.h>
int main()
{
	for(char ch='A';ch<='Z';ch++)
	{
		printf("%c=%d\n",ch,ch);
	}
}

#include<stdio.h>
int main()
{
printf("Odd number b/w 1 and 20 is given below\n");
 for(int i=1;i<=20;i=i+2)
 {
 	printf("%d ",i);
 }
}

#include<stdio.h>
int main()
{
	int no;
	printf("Enter any number\n");
	scanf("%d",&no);
	printf("Natural no from 1 to %d in reverse order is given below\n",no);
	for(int i=no;i>=1;i--)
	{
		printf("%d ",i);
	}
}

#include<stdio.h>
int main()
{
	int no,sum=0;
	printf("Enter any number\n");
	scanf("%d",&no);
	printf("Natural no from 1 to %d is given below\n",no);
	for(int i=1;i<=no;i++)
	{
		printf("%d ",i);
		sum=sum+i;
	}
	printf("\nTotal sum=%d",sum);
}

#include<stdio.h>
int main()
{
	int no,b,rev=0,cpy;
	printf("Enter any number\n");
	scanf("%d",&no);
	cpy=no;
	while(no!=0)
	{
		b=no%10;
		rev=rev*10+b;
		no=no/10;
	}
	if(cpy==rev)
	printf("Palindrome");
	else
	printf("Not Palindrome");
}

#include<stdio.h>
int main()
{
	int no,b,sum=0;
	printf("Enter any number\n");
	scanf("%d",&no);
	while(no!=0)
	{
		b=no%10;
		sum=sum+b;
		no=no/10;
	}
	printf("Total sum of digits=%d",sum);
}

#include<stdio.h>
int main()
{
	int i,j;
	for(i=0;i<3;i++) // i=row
	{
		for(j=0;j<3;j++)//i=row
		{
			printf("chaitan");
		}
		printf("\n")
	}
}

#include<stdio.h>
int main()
{
	int i,n;
	//for (imit ; condition; inmcriment)
	for(i=1;i<=10;i++)
	{
		printf("%d\n",i*2);
	}


	printf("enter any num:");
	scanf("%d",&n);
	for(i=0;i<=10;i++)
	{
		printf("%d\n",i*n);
	}
}

#include<stdio.h>
int main()
{
	//exit control loop: it checks condition at the end 
	int i=11;//init
	do
	{
		printf("hello from c...%d\n"i);
		i++; //i+i+1
	}while(i<=10);//condition

	printf("current value of i : %d\n",i);
}

#include<stdio.h>
int main()
{
	int i;
	//for(init ; condition ; inmcriment)
	for(i=1;1<=10;i++)
	{
		printf("hello..welcome to c...%d\n",i);
	}
}

#include<stdio.h>
int main()
{
	int i,arr [5]={10,20,30,40,50}
	printf("array elements :\n");
	for(i=0;i<5;i++)
	{
		printf("%d\n",arr[i]);
	}

	printf("value at index 3: %d\n",arr[3]);
	arr[3]=35
	printf("updated array after ele change :\n");
	for(i=0;i<5;i++)
	{
		printf("%d=d\n",i arr[i]);
	}
}

#include<stdio.h>
int main()
{
	int i,arr[5]={10,20,30,40,50};
	printf("array elements:\n");
	for(i=0;i<5;i++)
	{
		printf("%d\n",arr[i]);
	}

	//access ele
	printf("value at index 3:%d\n",arr[3]);

	//change ele
	arr[3]=35

	printf("updated array after ele change:\n");
	for(i=0;i<5;i++)
	{
		printf("%d=%d\n",i;arr[i]);
	}
}

#include<stdio.h>
int main()
{
	int i arr [5];
	printf("enter array elements:");
	for(i=0;i<5;i++)
	{
		scanf("%d",&arr[i]);
	}

	printf("your array ele:\n");
	for(i=0;i<5;i++)
	{
		printf("d\n",arr[i]);
	}
}

#include<stdio.h>
int main()
{
	int i,numbers[5]={10,20,30,40,50};
	printf("array ele : \n");
	{
		printf("d\n,numbers[i]");
	}
	
	//access ele 
	printf("ele at index 3 : %d\n",numbers[3]);// arr-name [index]
	
	
	//change ele
	numbers[5]=35;
	
	printf("updated array ele:\n");
	for(i=0;i<5;i++)
	{
		printf("%d\n",i,numbers[i]);
	}
}

#include<stdio.h>
int main()
{
	int i,arr[5];
	printf("enter array ele :");
	for(i=0;i<5;i++)
	{
		scanf("%d",&arr[i]);
	}
	printf("array ele :\n");
	for(i=0;i<=5;i++)
	{
		printf("%d\n",arr[i]);
	}
}

#include<stdio.h>
int main()
{
	int i,j,arr[3][3]={1,2,3,4,5,6,7,8,9};
	printf("2d array :\n");
	for(i=0;i<3;i++)//i=row
	{
		for(j=0;j<3;j++) //i=col
	{
		printf("%d",arr[i][j]);
	}
	printf("\n");
	}
	printf("value at r=2,c=1:%d\n,arr[2][1]");
}

#include<stdio.h>
int main()
{
	int i,j,arr[3][3];
	printf("enter array ele :");
	for(i=0;i<3;i++)
	{
		for(j=0;j<3;i++)
		{
			scanf("%d",&arr[i][j]);
		}
	}
	printf("2d array :\n");
	for(i=0;i<3;i++)//i=row
	{
		for(j=0;j<3;j++)//i=col
		{
			printf("%d",arr[i][j]);
		}
		printf("\n");
	}
	
	printf("valude at r=2,c=1 :%d\n",arr[2][1]);
}

#include<stdio.h>
int main()
{
	char name[10]="udhar";
	printf("%s\n",name);
	
	//length
	printf("length of str : %d\n",strlen(name));
	//size of
	printf("sizeof str : %d\n",sizeof(name));
}

#include<stdio.h>
int main()
{
	char name[10]="udhar";
	printf("%s\n",name);
	
	//length
	printf("length of str : %d\n",strlen(name));
	//size of
	printf("sizeof str : %d\n",sizeof(name));//6
	
	
	
	
	char address[20]="chapaner";
	printf("address : %s\n",address);
	printf("size of address : %d\n",sizeof(address));//20
	
	
	//concat
	//strcat(first_data,second_data);
	strcat(name,address);
	printf("updated name aftar concate : %s\n",name);
	printf("updated address after concate : %s\n",address);
}

#include<stdio.h>
int main()
{
	char data[40];
	//strcpy(first_data,second_data);
	strcpy(data,name);
	printf("copied date : %s\n",data);
	
	
	//string char
	printf("string alphabets of address : \n");
	for(i=0;i<strlen(address);i++)
	{
		printf("%d = %c\n", i,address[i]);
	}
	
	//string using loop
	printf("string data of address : \n");
	for(i=0;i<strlen(address)i++)
	{
		printf("%d = %s\n",i,address);
	}
}

#include<stdio.h>
int main()
{
	//user input
	char id[20];
	printf("enter name:");
	for(i=0;i<10;i++);
	{
		scanf("%c",&id[i]);
	}
	
	printf("id : %s",id);
}

#include<stdio.h>
int main()
{
	int f,s;
	printf("enter the value of first number ");
	scanf("%d",&f);
	printf("enter the value of second numbar");
	scanf("%d"&s)
	if(f>s)
	{
		printf("it is smaller then frist\n");
	}
	else if (f>s)
	{
		printf("it is greater than first\n")
	}
	else
	{
		printf("it is same");
	}
}

#include<stdio.h>
int main()
{
	int no;
	printf("enter any no\n")
	scanf("%d",&no);
	switch(no)
	{
		case 1;
		printf("jan");
		break;
		case 2;
		printf("feb");
		break;
		case 3:
		printf("mar");
		defaulf:
		printf("invalide input");
	}
}

#include<stdio.h>
int main()
{
	char ch;
	printf("enetr any alphabet\n");
	scanf("%c",&ch);

	if(ch=='a'||ch=='e'||ch=='i'||ch=='o'||ch=='v')
	{
		printf("vowel");
	}
	else
	{
		printf("consonent");
	}
}

#include<stdio.h>
#include<stringh>
int main()
{
	float a1,a2,a3;
	printf("enter frist angle\n");
	scanf("%f",&a1);
	printf("enter second angle\n");
	scanf("%f",&a2);
	printf("enter third angle\n");
	scanf("%f",&a3);
	if((a1+a2+a3)==180)
	{
		printf("triangle is valid");
	}
	else
	{
		printf("triangle is not valid");
	}
}

#include<stdio.h>
#include<string.h>
int main()
{
	fload sp,cp,profit.loss;
	printf("enter cost price\n");
	scanf("%f",&cp);
	printf("enetr selling price\n");
	scanf("%f"&sp);
	if(so>cp)
	{
		profit=sp-cp;
		printf("prafit is %f rupee",profit);
		{
			elsa
		}
		loss=cp-sp;
		printf("loss is%f rupee"loss);
	}
}

#include<stdio.h>
int main()
{
	flood p;
	printf("enter your perent\n");
	scanf("%F",&p);
	if(p>=)
	{
		printf("frist division");
	}
	else if(p>=45)
	{
		printf("second division");
	}
	else if(p>=33)
	{
		printf("third division");
	}
	else
	{
		printf("fail")
	}
}

#include<stdio.h>
int main()
{
	int a,b,c;
	printf("Enter first number\n");
	scanf("%d",&a);
	printf("Enter second number\n");
	scanf("%d",&b);
	printf("Enter third number\n");
	scanf("%d",&c);
	if(a>b&&a>c)
	{
		printf("%d is greater",a);
	}
	if(b>a&&b>c)
	{
		printf("%d is greater",b);
	}
	if(c>a&&c>b)
	{
		printf("%d is greater",c);
	}
}

#include<stdio.h>
int main()
{
	float p;
	printf("Enter your percent\n");
	scanf("%f",&p);
	if(p>=60)
	{
		printf("First division");
	}
	else if(p>=45)
	{
		printf("Second division");
	}
	else if(p>=33)
	{
		printf("Third division");
	}
	else
	{
		printf("Fail");
	}
}

#include<stdio.h>
int main()
{
	int a,b,c;
	printf("Enter first number\n");
	scanf("%d",&a);
	printf("Enter second number\n");
	scanf("%d",&b);
	printf("Enter third number\n");
	scanf("%d",&c);
	if(a>b&&a>c)
	{
		printf("%d is greater",a);
	}
	else if(b>a&&b>c)
	{
		printf("%d is greater",b);
	}
	else
	{
		printf("%d is greater",c);
	}
}

#include<stdio.h>
int main()
{
	char ch;
	printf("Enter any character\n");
	scanf("%c",&ch);
	if(ch>=65&&ch<=97||ch>=97&&ch<=122)
	{
	printf("It is alphabet");	
	}	
	else if(ch>=48&&ch<=57)
	{
	printf("It is digit");
	}
	else
	{
	printf("It is special symbol");
	}
}

#include<stdio.h>
int main()
{
	int no;
	printf("Enter any number\n");
	scanf("%d",&no);
	switch(no)
	{		
		case 1:
			printf("Monday");
			break;
		case 2:
			printf("Tuesday");
			break;	
		case 3:
			printf("Wednesday");
			break;
		case 4:
			printf("Thrusday");
			break;
		case 5:
			printf("Friday");
			break;
		case 6:
			printf("Saturday");
			break;
		case 7:
			printf("Sunday");
			break;
		default:
			printf("Invalid input");
	}
}

#include<stdio.h>
int main()
{
	char ch;
	printf("Enter any alphabet\n");
	scanf("%c",&ch);
	switch(ch)
	{		
		case 'a':
			printf("vowel");
			break;
		case 'e':
			printf("vowel");
			break;	
		case 'i':
			printf("vowel");
			break;
		case 'o':
			printf("vowel");
			break;
		case 'u':
			printf("vowel");
			break;
		default:
			printf("Consonent");
	}
}

#include<stdio.h>
int main()
{
	char ch;
	printf("Enter any alphabet\n");
	scanf("%c",&ch);
	switch(ch)
	{		
		case 'a':
		case 'e':
		case 'i':
		case 'o':
		case 'u':
			printf("vowel");
			break;
		default:
			printf("Consonent");
	}
}

for(int i=1;;i=i+1)
 {
 	if(i%no1==0&&i%no2==0)
 	{
 	  printf("LCM of %d and %d is %d",no1,no2,i);
	   break;	
	}
 }
}

#include <stdio.h>

int main() {
    int a = 25, b = 5;

    // using operators and printing results
    printf("a & b: %d\n", a & b);
    printf("a | b: %d\n", a | b);
    printf("a ^ b: %d\n", a ^ b);
    printf("~a: %d\n", ~a);
    printf("a >> b: %d\n", a >> b);
    printf("a << b: %d\n", a << b);

    return 0;
}

#include <stdio.h>

int main() {
    int a = 25, b = 5;

    // using operators and printing results
    printf("a = b: %d\n", a = b);
    printf("a += b: %d\n", a += b);
    printf("a -= b: %d\n", a -= b);
    printf("a *= b: %d\n", a *= b);
    printf("a /= b: %d\n", a /= b);
    printf("a %%= b: %d\n", a %= b);
    printf("a &= b: %d\n", a &= b);
    printf("a |= b: %d\n", a |= b);
    printf("a ^= b: %d\n", a ^= b);
    printf("a >>= b: %d\n", a >>= b); 
    printf("a <<= b: %d\n", a <<= b);

    return 0;
}

#include<stdio.h>
int main()
{
int no1,no2,m=1;
printf("Enter first number\n");
scanf("%d",&no1);
printf("Enter second number\n");
scanf("%d",&no2);
 for(int i=1;i<=no1;i=i+1)
 {
 	if(no1%i==0&&no2%i==0)
 	{
 	 m=i; 	
	}
 }
 printf("HCF of %d and %d is %d",no1,no2,m);
}

#include<stdio.h>
int main()
{
	int no,m=0;
	printf("Enter any number\n");
	scanf("%d",&no);
	for(int i=2;i<=no-1;i++)
	{
		if(no%i==0)
		{
			printf("Number is not  Prime");
			m=1;
			break;
		}
	}
	if(m==0)
	printf("Number is prime");
}

// C Program to demonstrate the use of Misc operators
#include <stdio.h>

int main()
{
    // integer variable
    int num = 10;
    int* add_of_num = &num;

    printf("sizeof(num) = %d bytes\n", sizeof(num));
    printf("&num = %p\n", &num);
    printf("*add_of_num = %d\n", *add_of_num);
    printf("(10 < 5) ? 10 : 20 = %d\n", (10 < 5) ? 10 : 20);
    printf("(float)num = %f\n", (float)num);

    return 0;
}

#include <stdio.h>

int main(){
    int age = 11;

    if (age >= 18) {
        if (age >= 60)
            printf("Eligible to vote (Senior Citizen)\n");
        else
            printf("Eligible for vote\n");
    }
    else {
        printf("Not eligible to vote (Under 18)\n");
        if (age >= 13) 
                printf("teenager\n");
            else
                printf("not a teenager\n");
        }

    return 0;
}

#include <stdio.h>

int main() {
    
    // variable to be used in switch statement
    int var = 18;

    // declaring switch cases
    switch (var) {
    case 15:
        printf("You are a kid");
        break;
    case 18:
        printf("Eligible for vote");
        break;
    default:
        printf("Default Case is executed");
        break;
    }

    return 0;
}

#include<stdio.h>
int main()
{
	int n,m,num;
	printf("Enter any number upto you want to print prime number\n");
	scanf("%d",&num);
	printf("Prime number between 1 and %d is given below\n",num);
	for(int i=1;i<=num;i++)
	{
		n=i,m=0;
		for(int j=2;j<=n-1;j++)
	    {
		if(n%j==0)
		  {
			m=1;
			break;
		  }
	    }
	if(m==0)
	printf("%d ",n);
	}
}

#include<stdio.h>
int main()
{
	int i=1;
	int *p;
	p=&i;
	while(*p<=10)
	{
		printf("%d\n",*p);
		(*p)++;
	}
}

#include<stdio.h>
int main()
{
	for(char ch='A';ch<='Z';ch++)
	{
		printf("%c ",ch);
    }
}

#include<stdio.h>
int main()
{
	for(int i=65;i<=90;i++)
	{
		printf("%c ",i);
    }
}

#include<stdio.h>
int main()
{
	for(char ch='a';ch<='z';ch++)
	{
		printf("%c ",ch);
    }
}

#include<stdio.h>
int main()
{
	for(int i=97;i<=122;i++)
	{
		printf("%c ",i);
    }
}

#include<stdio.h>
int main()
{
	for(char ch='A';ch<='Z';ch++)
	{
		printf("%c=%d\n",ch,ch);
	}
}

#include<stdio.h>
int main()
{
printf("Odd number b/w 1 and 20 is given below\n");
 for(int i=1;i<=20;i=i+2)
 {
 	printf("%d ",i);
 }
}

#include<stdio.h>
int main()
{
	int no;
	printf("Enter any number\n");
	scanf("%d",&no);
	printf("Natural no from 1 to %d in reverse order is given below\n",no);
	for(int i=no;i>=1;i--)
	{
		printf("%d ",i);
	}
}

#include<stdio.h>
int main()
{
	int no,sum=0;
	printf("Enter any number\n");
	scanf("%d",&no);
	printf("Natural no from 1 to %d is given below\n",no);
	for(int i=1;i<=no;i++)
	{
		printf("%d ",i);
		sum=sum+i;
	}
	printf("\nTotal sum=%d",sum);
}

#include<stdio.h>
int main()
{
	int no,b,rev=0,cpy;
	printf("Enter any number\n");
	scanf("%d",&no);
	cpy=no;
	while(no!=0)
	{
		b=no%10;
		rev=rev*10+b;
		no=no/10;
	}
	if(cpy==rev)
	printf("Palindrome");
	else
	printf("Not Palindrome");
}

#include<stdio.h>
int main()
{
	int no,b,sum=0;
	printf("Enter any number\n");
	scanf("%d",&no);
	while(no!=0)
	{
		b=no%10;
		sum=sum+b;
		no=no/10;
	}
	printf("Total sum of digits=%d",sum);
}

#include<stdio.h>
int main()
{
	int i,j;
	for(i=0;i<3;i++) // i=row
	{
		for(j=0;j<3;j++)//i=row
		{
			printf("chaitan");
		}
		printf("\n")
	}
}

#include<stdio.h>
int main()
{
	int i,n;
	//for (imit ; condition; inmcriment)
	for(i=1;i<=10;i++)
	{
		printf("%d\n",i*2);
	}


	printf("enter any num:");
	scanf("%d",&n);
	for(i=0;i<=10;i++)
	{
		printf("%d\n",i*n);
	}
}

#include<stdio.h>
int main()
{
	//exit control loop: it checks condition at the end 
	int i=11;//init
	do
	{
		printf("hello from c...%d\n"i);
		i++; //i+i+1
	}while(i<=10);//condition

	printf("current value of i : %d\n",i);
}

#include<stdio.h>
int main()
{
	int i;
	//for(init ; condition ; inmcriment)
	for(i=1;1<=10;i++)
	{
		printf("hello..welcome to c...%d\n",i);
	}
}

#include<stdio.h>
int main()
{
	int i,arr [5]={10,20,30,40,50}
	printf("array elements :\n");
	for(i=0;i<5;i++)
	{
		printf("%d\n",arr[i]);
	}

	printf("value at index 3: %d\n",arr[3]);
	arr[3]=35
	printf("updated array after ele change :\n");
	for(i=0;i<5;i++)
	{
		printf("%d=d\n",i arr[i]);
	}
}

#include<stdio.h>
int main()
{
	int i,arr[5]={10,20,30,40,50};
	printf("array elements:\n");
	for(i=0;i<5;i++)
	{
		printf("%d\n",arr[i]);
	}

	//access ele
	printf("value at index 3:%d\n",arr[3]);

	//change ele
	arr[3]=35

	printf("updated array after ele change:\n");
	for(i=0;i<5;i++)
	{
		printf("%d=%d\n",i;arr[i]);
	}
}

#include<stdio.h>
int main()
{
	int i arr [5];
	printf("enter array elements:");
	for(i=0;i<5;i++)
	{
		scanf("%d",&arr[i]);
	}

	printf("your array ele:\n");
	for(i=0;i<5;i++)
	{
		printf("d\n",arr[i]);
	}
}

#include<stdio.h>
int main()
{
	int i,numbers[5]={10,20,30,40,50};
	printf("array ele : \n");
	{
		printf("d\n,numbers[i]");
	}
	
	//access ele 
	printf("ele at index 3 : %d\n",numbers[3]);// arr-name [index]
	
	
	//change ele
	numbers[5]=35;
	
	printf("updated array ele:\n");
	for(i=0;i<5;i++)
	{
		printf("%d\n",i,numbers[i]);
	}
}

#include<stdio.h>
int main()
{
	int i,arr[5];
	printf("enter array ele :");
	for(i=0;i<5;i++)
	{
		scanf("%d",&arr[i]);
	}
	printf("array ele :\n");
	for(i=0;i<=5;i++)
	{
		printf("%d\n",arr[i]);
	}
}

#include<stdio.h>
int main()
{
	int i,j,arr[3][3]={1,2,3,4,5,6,7,8,9};
	printf("2d array :\n");
	for(i=0;i<3;i++)//i=row
	{
		for(j=0;j<3;j++) //i=col
	{
		printf("%d",arr[i][j]);
	}
	printf("\n");
	}
	printf("value at r=2,c=1:%d\n,arr[2][1]");
}

#include<stdio.h>
int main()
{
	int i,j,arr[3][3];
	printf("enter array ele :");
	for(i=0;i<3;i++)
	{
		for(j=0;j<3;i++)
		{
			scanf("%d",&arr[i][j]);
		}
	}
	printf("2d array :\n");
	for(i=0;i<3;i++)//i=row
	{
		for(j=0;j<3;j++)//i=col
		{
			printf("%d",arr[i][j]);
		}
		printf("\n");
	}
	
	printf("valude at r=2,c=1 :%d\n",arr[2][1]);
}

#include<stdio.h>
int main()
{
	char name[10]="udhar";
	printf("%s\n",name);
	
	//length
	printf("length of str : %d\n",strlen(name));
	//size of
	printf("sizeof str : %d\n",sizeof(name));
}

#include<stdio.h>
int main()
{
	char name[10]="udhar";
	printf("%s\n",name);
	
	//length
	printf("length of str : %d\n",strlen(name));
	//size of
	printf("sizeof str : %d\n",sizeof(name));//6
	
	
	
	
	char address[20]="chapaner";
	printf("address : %s\n",address);
	printf("size of address : %d\n",sizeof(address));//20
	
	
	//concat
	//strcat(first_data,second_data);
	strcat(name,address);
	printf("updated name aftar concate : %s\n",name);
	printf("updated address after concate : %s\n",address);
}

#include<stdio.h>
int main()
{
	char data[40];
	//strcpy(first_data,second_data);
	strcpy(data,name);
	printf("copied date : %s\n",data);
	
	
	//string char
	printf("string alphabets of address : \n");
	for(i=0;i<strlen(address);i++)
	{
		printf("%d = %c\n", i,address[i]);
	}
	
	//string using loop
	printf("string data of address : \n");
	for(i=0;i<strlen(address)i++)
	{
		printf("%d = %s\n",i,address);
	}
}

#include<stdio.h>
int main()
{
	//user input
	char id[20];
	printf("enter name:");
	for(i=0;i<10;i++);
	{
		scanf("%c",&id[i]);
	}
	
	printf("id : %s",id);
}

#include<stdio.h>
int main()
{
	int f,s;
	printf("enter the value of first number ");
	scanf("%d",&f);
	printf("enter the value of second numbar");
	scanf("%d"&s)
	if(f>s)
	{
		printf("it is smaller then frist\n");
	}
	else if (f>s)
	{
		printf("it is greater than first\n")
	}
	else
	{
		printf("it is same");
	}
}

#include<stdio.h>
int main()
{
	int no;
	printf("enter any no\n")
	scanf("%d",&no);
	switch(no)
	{
		case 1;
		printf("jan");
		break;
		case 2;
		printf("feb");
		break;
		case 3:
		printf("mar");
		defaulf:
		printf("invalide input");
	}
}

#include<stdio.h>
int main()
{
	char ch;
	printf("enetr any alphabet\n");
	scanf("%c",&ch);

	if(ch=='a'||ch=='e'||ch=='i'||ch=='o'||ch=='v')
	{
		printf("vowel");
	}
	else
	{
		printf("consonent");
	}
}

#include<stdio.h>
#include<stringh>
int main()
{
	float a1,a2,a3;
	printf("enter frist angle\n");
	scanf("%f",&a1);
	printf("enter second angle\n");
	scanf("%f",&a2);
	printf("enter third angle\n");
	scanf("%f",&a3);
	if((a1+a2+a3)==180)
	{
		printf("triangle is valid");
	}
	else
	{
		printf("triangle is not valid");
	}
}

#include<stdio.h>
#include<string.h>
int main()
{
	fload sp,cp,profit.loss;
	printf("enter cost price\n");
	scanf("%f",&cp);
	printf("enetr selling price\n");
	scanf("%f"&sp);
	if(so>cp)
	{
		profit=sp-cp;
		printf("prafit is %f rupee",profit);
		{
			elsa
		}
		loss=cp-sp;
		printf("loss is%f rupee"loss);
	}
}

#include<stdio.h>
int main()
{
	flood p;
	printf("enter your perent\n");
	scanf("%F",&p);
	if(p>=)
	{
		printf("frist division");
	}
	else if(p>=45)
	{
		printf("second division");
	}
	else if(p>=33)
	{
		printf("third division");
	}
	else
	{
		printf("fail")
	}
}

#include<stdio.h>
int main()
{
	int a,b,c;
	printf("Enter first number\n");
	scanf("%d",&a);
	printf("Enter second number\n");
	scanf("%d",&b);
	printf("Enter third number\n");
	scanf("%d",&c);
	if(a>b&&a>c)
	{
		printf("%d is greater",a);
	}
	if(b>a&&b>c)
	{
		printf("%d is greater",b);
	}
	if(c>a&&c>b)
	{
		printf("%d is greater",c);
	}
}

#include<stdio.h>
int main()
{
	float p;
	printf("Enter your percent\n");
	scanf("%f",&p);
	if(p>=60)
	{
		printf("First division");
	}
	else if(p>=45)
	{
		printf("Second division");
	}
	else if(p>=33)
	{
		printf("Third division");
	}
	else
	{
		printf("Fail");
	}
}

#include<stdio.h>
int main()
{
	int a,b,c;
	printf("Enter first number\n");
	scanf("%d",&a);
	printf("Enter second number\n");
	scanf("%d",&b);
	printf("Enter third number\n");
	scanf("%d",&c);
	if(a>b&&a>c)
	{
		printf("%d is greater",a);
	}
	else if(b>a&&b>c)
	{
		printf("%d is greater",b);
	}
	else
	{
		printf("%d is greater",c);
	}
}

#include<stdio.h>
int main()
{
	char ch;
	printf("Enter any character\n");
	scanf("%c",&ch);
	if(ch>=65&&ch<=97||ch>=97&&ch<=122)
	{
	printf("It is alphabet");	
	}	
	else if(ch>=48&&ch<=57)
	{
	printf("It is digit");
	}
	else
	{
	printf("It is special symbol");
	}
}

#include<stdio.h>
int main()
{
	int no;
	printf("Enter any number\n");
	scanf("%d",&no);
	switch(no)
	{		
		case 1:
			printf("Monday");
			break;
		case 2:
			printf("Tuesday");
			break;	
		case 3:
			printf("Wednesday");
			break;
		case 4:
			printf("Thrusday");
			break;
		case 5:
			printf("Friday");
			break;
		case 6:
			printf("Saturday");
			break;
		case 7:
			printf("Sunday");
			break;
		default:
			printf("Invalid input");
	}
}

#include<stdio.h>
int main()
{
	char ch;
	printf("Enter any alphabet\n");
	scanf("%c",&ch);
	switch(ch)
	{		
		case 'a':
			printf("vowel");
			break;
		case 'e':
			printf("vowel");
			break;	
		case 'i':
			printf("vowel");
			break;
		case 'o':
			printf("vowel");
			break;
		case 'u':
			printf("vowel");
			break;
		default:
			printf("Consonent");
	}
}

#include<stdio.h>
int main()
{
	char ch;
	printf("Enter any alphabet\n");
	scanf("%c",&ch);
	switch(ch)
	{		
		case 'a':
		case 'e':
		case 'i':
		case 'o':
		case 'u':
			printf("vowel");
			break;
		default:
			printf("Consonent");
	}
}

#include <stdio.h>

int main() {

    // array declaration and initialization
    int arr[5] = {2, 4, 8, 12, 16};

    // accessing element at index 2 i.e 3rd element
    printf("%d ", arr[2]);

    // accessing element at index 4 i.e last element
    printf("%d ", arr[4]);

    // accessing element at index 0 i.e first element
    printf("%d ", arr[0]);
    return 0;
}
#include <stdio.h>

union A{
    int x;
    char y;
};

union B{
    int arr[10];
    char y;
};


int main() {
   // Finding size using sizeof() operator
    printf("Sizeof A: %l
	d\n", sizeof(union A));
    printf("Sizeof B: %ld\n", sizeof(union B));
    return 0;
}

void printStr(char str[]) {
    printf("%s", str);
}

int main() {
    char str[] =
	 "GeeksforGeeks";

    // Passing string to a 
    // function
    printStr(str);
    return 0;
}

// C Program to demonstrate the structure packing
#include <stdio.h>
#pragma pack(1)

// structure A
typedef struct structa_tag {
    char c;
    short int s;
} structa_t;

// structure B
typedef struct structb_tag {
    short int s;
    char c;
    int i;
} structb_t;

// structure C
typedef struct structc_tag {
    char c;
    double d;
    int s;
} structc_t;

// structure D
typedef struct structd_tag {
    double d;
    int s;
    char c;
} structd_t;

int main()
{
    printf("sizeof(structa_t) = %lu\n", sizeof(structa_t));
    printf("sizeof(structb_t) = %lu\n", sizeof(structb_t));
    printf("sizeof(structc_t) = %lu\n", sizeof(structc_t));
    printf("sizeof(structd_t) = %lu\n", sizeof(structd_t));

    return 0;
}

#include <stdio.h>
#include <stdlib.h>

// Global variable
int gvar = 66;

// Constant global variable
const int cgvar = 1010;

// uninitialized global variable
int ugvar;

void foo() {
    
    // Local variable
    int lvar = 1;
    printf("Address of lvar:\t%p", (void*)&lvar);
}

int main() {
    
    // Heap variable
    int *hvar = (int*)malloc(sizeof(int));
    
    
    // Checking and comparing address of different
    // elements of program that should be stored in
    // different segements of the memory
    printf("Address of foo:\t\t%p\n", (void*)&foo);
    printf("Address of cgvar:\t%p\n", (void*)&cgvar);
    printf("Address of gvar:\t%p\n", (void*)&gvar);
    printf("Address of ugvar:\t%p\n", (void*)&ugvar);
    printf("Address of hvar:\t%p\n", (void*)hvar);
    foo();
    
	return 0;
}

#include <stdio.h>
#include <stdlib.h>

int main() {
    int *ptr = (int *)malloc(20);
    
    // Populate the array
    for (int i = 0; i < 5; i++)
        ptr[i] = i + 1;
        
    // Print the array
    for (int i = 0; i < 5; i++)
        printf("%d ", ptr[i]);
    return 0;
}

#include <stdio.h>
#include <stdlib.h>

int main()
{
    int *ptr = (int *)malloc(sizeof(int) * 5);

    // Populate the array
    for (int i = 0; i < 5; i++)
        ptr[i] = i + 1;

    // Print the array
    for (int i = 0; i < 5; i++)
        printf("%d ", ptr[i]);
    return 0;
}

#include <stdio.h>
#include <stdlib.h>

int main() {
    int *ptr = (int *)malloc(sizeof(int) * 5);
    
    // Checking if failed or pass
    if (ptr == NULL) {
        printf("Allocation Failed");
        exit(0);
    }
    
    // Populate the array
    for (int i = 0; i < 5; i++)
        ptr[i] = i + 1;
        
    // Print the array
    for (int i = 0; i < 5; i++)
        printf("%d ", ptr[i]);
    return 0;
}

#include <stdio.h>
#include <stdlib.h>

int main() {
    int *ptr = (int *)calloc(5, sizeof(int));
    
    // Checking if failed or pass
    if (ptr == NULL) {
        printf("Allocation Failed");
        exit(0);
    }
    
    // No need to populate as already
    // initialized to 0
        
    // Print the array
    for (int i = 0; i < 5; i++)
        printf("%d ", ptr[i]);
    return 0;
}

#include <stdio.h>
#include <stdlib.h>

int main() {
    int *ptr = (int *)malloc(5 * sizeof(int));

    // Resize the memory block to hold 10 integers
    ptr = (int *)realloc(ptr, 10 * sizeof(int));
    
    // Check for allocation failure
    if (ptr == NULL) {
        printf("Memory Reallocation Failed");
        exit(0);
    }

    return 0;
}

#include <stdio.h>
#include <stdlib.h>

int main()
{
    int *ptr = (int *)malloc(5 * sizeof(int));

    // Reallocation
    int *temp = (int *)realloc(ptr, 10 * sizeof(int));

    // Only update the pointer if reallocation is successful
    if (temp == NULL)
        printf("Memory Reallocation Failed\n");
    else
        ptr = temp;

    return 0;
}

#include <stdio.h>
#include <stdlib.h>

int main() {
    
    // Initially allocate memory for 5 integers
    int *ptr = (int *)malloc(5 * sizeof(int));
    
    // Check if allocation was successful
    if (ptr == NULL) {
        printf("Memory Allocation Failed\n");
        exit(0);
    }
    
    // Now, we need to store 8 elements so
    // Reallocate to store 8 integers
    ptr = (int *)realloc(ptr, 8 * sizeof(int)); 
    
    // Check if reallocation was successful
    if (ptr == NULL) {
        printf("Memory Reallocation Failed\n");
        exit(0);
    }
    
    // Assume we only use 5 elements now
    for (int i = 0; i < 5; i++) {
        ptr[i] = (i + 1) * 10;
    }
    
    // Shrink the array back to 5 elements
    ptr = (int *)realloc(ptr, 5 * sizeof(int));
    
    // Check if shrinking was successful
    if (ptr == NULL) {
        printf("Memory Reallocation Failed\n");
        exit(0);
    }
    
    for (int i = 0; i < 5; i++)
        printf("%d ", ptr[i]);
    
    // Finally, free the memory when done
    free(ptr);
    
    return 0;
}

#include <stdio.h>
#include <stdlib.h>

int main() {
    
    // File pointer
    FILE* fptr;

    // Get the data to be written in file
    char data[50] = "GeeksforGeeks-A Computer "
                    "Science Portal for Geeks";

    // Creating file using fopen()
    // with access mode "w"
    fptr = fopen("file.txt", "w");

    // Checking if the file is created
    if (fptr == NULL) 
        printf("The file is not opened.");
    else{
        printf("The file is now opened.\n");
        fputs(data, fptr);
        fputs("\n", fptr);

        // Closing the file using fclose()
        fclose(fptr);
        printf("Data successfully written in file "
               "file.txt\n");
        printf("The file is now closed.");
    }
    return 0;
}

#include <stdio.h>
#include <string.h>

int main() {
    FILE* fptr;

    // Declare the character array 
    // for the data to be read from file
    char data[50];
    fptr = fopen("file.txt", "r");

    if (fptr == NULL) {
        printf("file.txt file failed to open.");
    }
    else {

        printf("The file is now opened.\n");

        // Read the data from the file
        // using fgets() method
        while (fgets(data, 50, fptr)
               != NULL) {

            // Print the data
            printf("%s", data);
        }

        // Closing the file using fclose()
        fclose(fptr);
    }
    return 0;
}

#include <stdio.h>
#include <stdlib.h>

int main() {
    
    // File pointer
    FILE* fptr;

    // Get the data to be written in file
    char data[50] = "GeeksforGeeks-A Computer "
                    "Science Portal for Geeks";

    // Creating file using fopen()
    // with access mode "w"
    fptr = fopen("file.txt", "w");

    // Checking if the file is created
    if (fptr == NULL) 
        printf("The file is not opened.");
    else{
        printf("The file is now opened.\n");
        fputs(data, fptr);
        fputs("\n", fptr);
        fseek(fptr, -6, SEEK_END);
        
        fputs("GeeksforGeeks", fptr);

        // Closing the file using fclose()
        fclose(fptr);
        printf("Data successfully written in file "
               "file.txt\n");
        printf("The file is now closed.");
    }
    return 0;
}

#include <stdio.h>
#include <stdlib.h>

struct threeNum {
    int n1, n2, n3;
};

int main() {
    int n =1 ;
    
    // Structure variable declared.
    struct threeNum num;
    FILE* fptr;
    fptr = fopen("binaryFile.bin", "wb");
    int flag = 0;
    num.n1 = n;
    num.n2 = 5 * n;
    num.n3 = 5 * n + 1;
    
    // Write the Structure data
    // to binary file.
    flag = fwrite(&num, sizeof(struct threeNum), 1,
                  fptr);

    // Checking if the data is written.
    if (!flag)
        printf("Write Operation Failure");
    else
        printf("Write Operation Successful");
    fclose(fptr);
    return 0;
}

#include <stdio.h>
#include <stdlib.h>

// Structure that store
// binary file data
struct threeNum {
    int n1, n2, n3;
};

int main() {
    int n;
    struct threeNum num;
    FILE* fptr;
    fptr = fopen("binaryFile.bin", "rb");
    
    // Read the data from binary 
    // file and print that data
    fread(&num, sizeof(struct threeNum), 1, fptr);
    printf("n1: %d\tn2: %d\tn3: %d\n", num.n1, num.n2,
           num.n3);
    fclose(fptr);
    return 0;
}

// C program for writing
// struct to file
#include <stdio.h>
#include <stdlib.h>

// a struct to be read and written
struct person {
    int id;
    char fname[20];
    char lname[20];
};

int main()
{
    FILE* outfile;

    // open file for writing
    outfile = fopen("person.bin", "wb");
    if (outfile == NULL) {
        fprintf(stderr, "\nError opened file\n");
        exit(1);
    }

    struct person input1 = { 1, "rohan", "sharma" };

    // write struct to file
    int flag = 0;
    flag = fwrite(&input1, sizeof(struct person), 1,
                  outfile);
    if (flag) {
        printf("Contents of the structure written "
               "successfully");
    }
    else
        printf("Error Writing to File!");

    // close file
    fclose(outfile);

    return 0;
}

// C program for reading
// struct from a file
#include <stdio.h>
#include <stdlib.h>

// struct person with 3 fields
struct person {
    int id;
    char fname[20];
    char lname[20];
};

// Driver program
int main()
{
    FILE* infile;

    // Open person.dat for reading
    infile = fopen("person1.dat", "wb+");
    if (infile == NULL) {
        fprintf(stderr, "\nError opening file\n");
        exit(1);
    }

    struct person write_struct = { 1, "Rohan", "Sharma" };

    // writing to file
    fwrite(&write_struct, sizeof(write_struct), 1, infile);

    struct person read_struct;

    // setting pointer to start of the file
    rewind(infile);

    // reading to read_struct
    fread(&read_struct, sizeof(read_struct), 1, infile);

    printf("Name: %s %s \nID: %d", read_struct.fname,
           read_struct.lname, read_struct.id);

    // close file
    fclose(infile);

    return 0;
}

