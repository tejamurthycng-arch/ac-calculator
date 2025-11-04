# ac-calculator
int main()
{
    int R,L,C,F;
    float XL,XC,Z,Fr,Pf;
    printf("enter the value of resistance :");
    scanf("%d",&R);
    printf("\n enter the value of inductance :");
    scanf("%d",&L);
    printf("\n enter the value of capicitance :");
    scanf("%d",&C);
    printf("\n enter the value of frequency :");
    scanf("%d",&F);
    XL=(2*3.14*L*F);
    XC=(1/(2*3.14*C*F));
    Z=sqrt(pow(R,2)+pow((XL-XC),2));
    Fr=1/(2*3.14*sqrt(L*C)); 
    Pf=R/Z;
    printf("\n In an ac circuit");
    printf("\n the value of inductance resistance is :%f",XL);
    printf("\n the value of capicative resistance is :%f",XC);
    printf("\n The value of impedence is : %f",Z);
    printf("\n The value of resonating frequency is : %f",Fr);
    printf("\n The value of powerfactor is : %f",Pf);
    return 0;

}
