# 2021cce
hw
1
```C
#include <stdio.h>
int main()
{
	int n;
	scanf("%d",&n);
	printf("%d=50*%d+5*%d+1*%d\n",n,n/50,n%50/5,n%5);
}
```
2
```C
#include <stdio.h>
int main()
{
	int n;
	scanf("%d",&n);
	int num=1;
	for(int i=1;i<n;i++){
		if (n%i==0) num++;
	}
	printf("%d\n",num);
}
```
3
```C
#include <stdio.h>
int a[10];
int main()
{
	for(int i=0;i<10;i++){
		scanf("%d",&a[i]);
	}
	int num=0;
	for(int i=0;i<10;i++){
		if(a[i]%3==0) num++;
	}
	printf("%d\n",num);
}
```
4
```C
#include <stdio.h>
int main()
{
	int n;
	scanf("%d",&n);
	
	if(n>=90) printf("A\n");
	else if(n<90 && n>=80) printf("B\n");
	else if(n<80 && n>=60) printf("C\n");
	else printf("F\n");
}
```
