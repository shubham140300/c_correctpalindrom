//c_correctpalindrom c  language
#include<stdio.h>
#include<string.h>
void pl(char a[]){
     int i,n,x=0;
       n=strlen(a);
    for(i=0;i<n/2;i++)
    { 
        if(a[i]==a[n-1-i])
        x++;
         else
        {
            printf("not palindrome\n");
            break;
        }
        
    }
    if(x==n/2)
     printf("palindrome");
    
}
int main()
{
    char a[50];
    printf("enter string: ");
    gets(a);
    pl(a);
    return 0;
}
