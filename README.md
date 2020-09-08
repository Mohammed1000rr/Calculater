# Calculater

#include <stdio.h>

#include <stdlib.h>

int main()

{

 char ope = 0 , ch = '\0';
 
 int num1 , num2 ;

 do{

  printf(" enter first number :");
  
  scanf("%d" , &num1);

  printf(" enter ope :");
  
  scanf(" %c" , &ope);

  printf(" enter second number :");
  
  scanf("%d" , &num2);

  switch(ope){

  case '+':
  
      printf("%d + %d = %d" , num1,num2,num1+num2);
      
      break;
      
  case '-':
  
      printf("%d - %d = %d" , num1,num2,num1-num2);
      
      break;
      
  case '*':
  
      printf("%d * %d = %d" , num1,num2,num1*num2);
      
      break;
      
  case '/':
  
      printf("%d / %d = %d" , num1,num2,num1/num2);
      
      break;
      
  case '%':
  
      printf("%d %% %d = %d" , num1,num2,num1%num2);
      
      break;
      
  default:
  
      printf(" wrong choice !");
      
  }

  printf(" \n Do You Want Again (y/n)?");
  
  scanf(" %c",&ch);
  
 }while(ch == 'y');



  return 0;

}
