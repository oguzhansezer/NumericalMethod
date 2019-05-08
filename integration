#include<stdio.h>
#include<math.h>
#define f(x) exp(x)
int main()
{
    int choice;
    float  a,b,h,it,is1,is2,ib;
    printf("Solution for integration of exp(x) \n");
    printf("Enter lower limit and upper limit\n");   
    scanf("%f%f",&a,&b);
    printf("Select Options\n1.Trapezoidal Rule\n2.Simpson's Rule\n3.Simpson's 3/8 Rule\n4.Boole's Rule\n5.Exit\n");
a:printf("\nEnter Choice : ");
    scanf("%d",&choice);
    switch(choice)
    {
            
            //Trapezoidal Rule
        case 1:
            h=b-a;
            it=((f(a)+f(b))/2)*h;
            printf("It = %.4f\n",it);
            break;
    
            //Simpson's Rule
        case 2:
            h=(b-a)/2;
            is1=(h/3)*(f(a)+f(b)+4*f(a+h));
            printf("Is1 = %.4f\n",is1);
            break;
            //Simpson's 3/8 Rule
        case 3:
            h=(b-a)/3;
            is2=(3*h/8)*(f(a)+f(b)+3*f(a+h)+3*f(a+2*h));
            printf("Is2 = %.4f\n",is2);
            break;
            
            //Boole's Rule
        case 4:
            h=(b-a)/4;
            ib=(2*h/45)*(7*f(a)+7*f(b)+12*f(a+2*h)+32*(f(a+h)+f(a+3*h)));
            printf("Ib = %.4f\n",ib);
            break;
            
        case 5:
            exit(0);
            
        default:
            printf("\nEnter the correct choice...\n");
    }
    goto a;
    return 0;
}


