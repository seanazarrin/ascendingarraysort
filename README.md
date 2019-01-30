# ascendingarraysort

#include<stdio.h>

int main(void) {
    
    int n,i,y=0,temp,d,z;
    
    printf("enter the number of elements = \n");
    scanf("%d",&n);
    int x[n];
     
    while(z<n){                  //input
    scanf("%d",&x[z]);
      z++;
    }
    
    while(y<n){                  //bubble
        for(i=0;i<(n-1);i++){
            if(x[i]>x[i+1]){
                temp=x[i];
                x[i]=x[i+1];
                x[i+1]=temp;
            }
        }
        y++;
    }
    while(d<n){                 //output
    printf("%d ",x[d]);
        d++;
    }
    return 0;
}
