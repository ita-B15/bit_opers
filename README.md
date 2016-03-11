#include <stdio.h>



int main()

{

      int x1,x2,x3;
      int data,rez;
      int y1,y2,y3;
int i=0;

for(;i<8;++i){

data=i;
  
  x3=data&0x00000001;
  data=data>>1;
  x2=data&0x00000001;
  data=data>>1;
  x1=data&0x00000001;
  
  

  //printf("x1=%i x2=%i x3=%i\n\n",temp.bit1,temp.bit2,temp.bit3);
  y1=x2;
  y2=x2|(!x3);
  y3=((!x2)&x3)|((!x1)&x3);
  
  rez=y1*4+y2*2+y3;
  
  printf("x1=%i x2=%i x3=%i y1=%i y2=%i y3=%i in=%i out=%i\n",x1,x2,x3,y1,y2,y3,i,rez);
}}
  

	

