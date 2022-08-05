#include <stdio.h>
#include <stdlib.h>

int main()
{
    int m = 3; // rows
    int n = 4; //columns
    int arr[n][m];
    int i = 1;
    int j = 1;
    int maxi = n;
    while(maxi != 1){
               //while(j <= m){
                              if(i <= maxi){
                               j++;
                                printf("%d\t%d\n", i, j);
                              }else{
                                             i++;
                                printf("%d\t%d\n", i, j);
                                maxi = maxi - 1;
                              }
                              if(j == m && i >=1){
                                             i = i-1;
                                             printf("%d\t%d\n", i, j);
                              }else{
                                             j = m-1;
                              }
                              if(i < maxi){
                                     printf("%d\t%d\n", i, j);
                                     i++;
                              }
                              if(maxi == 1){
                                             break;
                              }
              // }
    }
    printf("Hello world!\n");
    return 0;
}
