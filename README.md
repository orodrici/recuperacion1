#include <iostream>

int diagSum(void);
int main()
{
    diagSum();

    //return 0;
}

int diagSum(void)
{
    int matriz [3][3]={{3,6,1},{2,4,6},{1,5,2}};
    int N=3;
    int sumadiagA=0;
    int sumadiagB=0;
    for(int i=0; i<3; ++i)
    {
        N=N-1;
        for(int a=0; a<3; ++a)

        {
            if(i==a)
            {
             sumadiagA=sumadiagA+ matriz[i][a];
            }
            if(a==N)
            {
              sumadiagB=sumadiagB+ matriz[i][a];  
            }
           
          std::cout<<"matriz ["<<i<<"]["<<a<<"]:"<<matriz[i][a]<<std::endl;
          
        }
    }

    std::cout<<"la suma de la diagonal A es:"<<sumadiagA<<std::endl;
    std::cout<<"la suma de la diagonal B es:"<<sumadiagB<<std::endl;
}
