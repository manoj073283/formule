# formule
#include <stdio.h>
int main()
{ 
    int num,r,h;
    float volume,csa,tsa,l;
    printf("select a shape \n1.Cylinder\n2.Cube\n3.Cone\n4.Sphere");
    scanf("%d",&num);
    switch(num){
        case 1:printf("Enter radius and height of the cylinder:\n");
        scanf("%d%d",&r,&h);
        volume=3.14*r*r*h;
        csa=2*3.14*r*h;
        tsa=2*3.14*r*(r+h);
        printf("Volume of cylinder=%f\n",volume);
        printf("curved surface area of cylinder=%f\n",csa);
        printf("total surface area of cylinder=%f\n",tsa);
        break;
        case 2:printf("enter length of the cube:\n");
               scanf("%d",&h);
               volume=h*h*h;
               printf("volume of the cube=%f",volume);
               break;
        case 3:printf("Enter radius and height of the cone:\n");
               scanf("%d%d",&r,&h);
               volume=0.33*3.14*r*r*h;
               l=sqrt(r*r*h*h);
               tsa=3.14*r*(r+1);
               csa=3.14*r*1;
               printf("volume of cone=%f\n",volume);
               printf("total surface area of cone=%f\n",tsa);
               printf("curved surface area of cone=%f\n",csa);
               break;
        case 4:printf("enter radius of the sphere=\n");
               scanf("%d",&r);
               volume=0.33*3.14*r*r*r;
               tsa=4*3.14*r*r;
               printf("volume of sphere=%f\n",volume);
               printf("surface area of sphere=%f\n",tsa);
               break;
        default:printf("select a valid shape");
        printf("THE END");
               
    }

    return 0;
}
