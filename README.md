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
5
```C
#include <stdio.h>
int main()
{
	int n,m,temp;
	scanf("%d%d",&n,&m);
	if(m>n) temp=n;
	else temp=m;
	int ans;
	for(int i=1;i<=temp;i++){
		if(n%i==0&&m%i==0) ans=i;
	}
	printf("%d %d\n",n/ans,m/ans);
}
```





























```C
#include <stdio.h>
struct POINT {
    float x,y,z;
};

struct POINT point[5]={{0,0,0},{1,0,0},{0,1,0},{0,0,1},{1,1,1}};

int main()
{
    struct POINT*p=&point[0];
    printf("%.2f %.2f %.2f\n",p->x,p->y,p->z);

    p++;
    printf("%.2f %.2f %.2f\n",p->x,p->y,p->z);

    p++;
    printf("%.2f %.2f %.2f\n",p->x,p->y,p->z);
}

```
```C
#include <stdio.h>
struct DATA{
    int x,y;
}a[3];
struct DATA b={100,200};

int main()
{
    for(int i=0;i<3;i++){
        printf("a[%d]:%d %d\n",i,a[i].x,a[i].y);
    }
    printf("b: %d %d\n",b.x,b.y);
    struct DATA c;
    printf("c: %d %d\n",c.x,c.y);

    c=b;
    printf("c: %d %d\n",c.x,c.y);
}

```
