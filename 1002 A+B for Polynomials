/*
This time, you are supposed to find A+B where A and B are two polynomials.

Input Specification:
Each input file contains one test case. Each case occupies 2 lines, and each line contains the information of a polynomial:

Output Specification:
For each test case you should output the sum of A and B in one line, with the same format as the input. Notice that there must be NO extra space at the end of each line. Please be accurate to 1 decimal place.

Sample Input:
2 1 2.4 0 3.2
2 2 1.5 1 0.5
Sample Output:
3 2 1.5 1 2.9 0 3.2
*/

#include<stdio.h>
float res[1001];
void rec(void){
	int m,exp;
	float coe;
	scanf("%d",&m);
	for(int i=0;i<m;i++){
		scanf("%d%f",&exp,&coe);
		res[exp]+=coe;
	}
}
int main(){
    int i,count=0;
	rec();
	rec();
	for(i=0;i<1001;i++)
		if(res[i]!=0)
			count++;
	printf("%d",count);
	for(i=1000;i>=0;i--)
		if(res[i]!=0.0)
			printf(" %d %.1f",i,res[i]);
}
