# Else-if-ladder
#include <stdio.h>

int main()
{
   int mm,yy,dd;
   scanf("%d/%d/%d",&dd,&mm,&yy);
   if(yy>=2000)
   {
       if(mm>=1&&mm<=12)
       {
           if((mm==1||mm==3||mm==5||mm==7||mm==8||mm==10||mm==12)&&(dd>=1&&dd<=31))
           {
               printf("valid");
           }
           else if((mm==4||mm==6||mm==9||mm==11)&&(dd>=1&&dd<=30))
           {
                printf("valid");
           }
           else if((mm==2)&&((yy%4==0&&yy%100!=0)||(yy%4==0))&&(1>=mm&&mm<=29))
           {
            printf("valid");
           }
           else if(mm==2&&(dd>=1&&dd<=28)){
                printf("valid");
           }
           else
           {
                printf("Invalid");
           }
           
       }
       else
       {
            printf("Invalid");
       }
       
   }
   else
   {
       printf("Invalid");
   }
   
   

    return 0;
}
