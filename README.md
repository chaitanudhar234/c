
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

