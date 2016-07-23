#include<stdio.h>
int main(){
    int n,k,t=0;
    scanf("%d",&n);
    int a[n],i,j;
    for(i=0;i<n;i++){
        scanf("%d",&a[i]);
    }
    k=0;
    for(i=0;i<n-1;i++){
        for(j=i+1;j<n;j++){
            for(k=j+1;k<n;k++){
            if((a[i]+a[j])==a[k]){
                    printf("%d+%d=%d",a[i],a[j],a[k]);
                t=1;
            }
                
            }
            if(t==1)
            break;
        }
        if(t==1)
        break;
    }

    return 0;
}
