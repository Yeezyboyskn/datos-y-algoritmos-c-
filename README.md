#include<stdio.h>
#include<math.h>
#define MAXLARGO 50


int binario_decimal(int*binario, int largo){
	int i;
	int decimal = 0;
	
	for(i=largo-1; i >=0;i--){
		decimal=decimal+(binario[i]*pow(2,largo-1-i));
	}
	return decimal;	
}

int binario_decimal_rec(int*binario,int largo){
	
}

int main(){
	int i;
	int largo=11;
	int binario[MAXLARGO]={1,0,1,1,0,1,1,0,1,1,1};
	
	int dec;
	dec = binario_decimal(binario,largo);
	printf("el numero decimal es %d\n",dec);
}
