# matrix-multiplication-in-c
matrix multiplication of any type of two matrix if matrix multiplication rules follow than it print matrix otherwise its show error
#include<stdio.h>

int main(){
     int r1,c1,r2,c2,i,j,a[100][100],b[100][100],k,c[100][100];
	 printf("for a first materix A\n");
	 printf("enter a first materix row\n");
	 scanf("%d",&r1);
	 printf("enter a first materix colum\n");
	 scanf("%d",&c1);
	 for(i=0;i<r1;i++){
	 	for(j=0;j<c1;j++){
	 		printf("enter a first matrix\n");
	 		scanf("%d",&a[i][j]);
	 		
		 }
	 }
	 	for(i=0;i<r1;i++){
	 	for(j=0;j<c1;j++){
	 		printf("%d\t",a[i][j]);
	 		
		 }
		 printf("\n");
	 }
	 	
	
printf("for a first materix B\n");
	 printf("enter a second materix row\n");
	 scanf("%d",&r2);
	 printf("enter a second materix colum\n");
	 scanf("%d",&c2);
	 for(i=0;i<r2;i++){
	 	for(j=0;j<c2;j++){
	 		printf("enter a second matrix\n");
	 		scanf("%d",&b[i][j]);
	 		
		 }
	 }
	 	for(i=0;i<r2;i++){
	 	for(j=0;j<c2;j++){
	 		printf("%d\t",b[i][j]);
	 		
		 }
		 printf("\n");
	 }
	 	
	  for (int i = 0; i < r1; ++i) {
            for (int j = 0; j < c2; ++j) {
                        c[i][j] = 0;
      }
   }
	if(c1==r2){
		for(i=0;i<r1;i++){
			for(j=0;j<c2;j++){
				for(k=0;k<c1;k++){
					c[i][j] +=a[i][k]*b[k][j];
				}
				
			}
		}
	}
	 else{
	 	printf("sorry your choosen matrix are can't applicabel for multiplication \n");
	 	
	 }
	 for(i=0;i<r1;i++){
	 	for(j=0;j<c2;j++){
	 		printf("%d\t",c[i][j]);
	 		
		 }
		 printf("\n");
	 }
	 return 0;	
}
