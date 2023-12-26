#include <stdio.h>
int main()
{
   
    int a,p,w,d,i,AMT=5000;
    printf("ENter the pin number ");
    scanf("%d",&a);
   
    if(a==1234)
    {
        while(p!=4)
       
       { printf("Press 1 for balance\nPress 2 for withdraw\n
         Press 3 for deposit\nPress 4 To exit Transaction\n");
        scanf("%d",&p);
        switch(p)
        {
        case 1:
        printf("Balance is 5000\n");
        break;
       
            case 2:
        printf("Enter Withdraw Amount\n");
        scanf("%d",&w);
        if(w<=AMT)
        {
            printf("Amount withdrawn is %d\n",w);
            AMT=AMT-w;
            printf("Balance is %d\n",AMT);
        }
        else
        {
            printf("Invalid Amount \n");
            }
                break;
            case 3:
                    printf("Enter deposit Amount\n");
                    scanf("%d",&d);
                    printf("Amount deposited is  %d\n",d);
                               AMT=AMT+d;
                    printf("Balance %d\n",AMT);
            break;
           default:
            break;
         }
       }
    }
   
    else {printf("Invalid Pin");}


    return 0;




}




