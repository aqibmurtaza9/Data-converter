#include <stdio.h> 
#include <stdlib.h>
#include <conio.h> 


int main()
{
	char choice,another;
	int bytes=1024,kbs=1024,mbs=1024,gbs=1024,tbs=1024;
	int s,d;
	double bt,byt,kb,mb,gb,tb,a;
    
    while(1)
    {
        system("cls"); ///clear the console window
        
		printf("1. Converter \n"); 
        printf("2. About \n"); 
        printf("3. Exit \n");
        printf("Your Choice: "); /// enter the choice 1, 2, 3
        choice  = getche(); /// get the input from keyboard
        
		switch(choice)
        {
        case '2':  /// if user press 1
            system("cls");
           
            another = 'y';
            while(another == 'y')
            {
              printf("Data Converter 1.9v [Mega]");
              printf("\nDeveloped By Aqib.");
              printf("\nVersion: 1.9[Mega] x86 December 2018");
			  printf("\n\nPress any key to Back.... ");
                fflush(stdin);
                another = getche();
            }
            break;
		case '1':// if user press 2
			system("cls");
			another = 'y';
			while(another == 'y')
			{
				system("cls");
				
				printf("1. Bits \n");
				printf("2. Bytes \n");
				printf("3. Kilobytes (KB) \n");
				printf("4. Megabytes (MB) \n");
				printf("5. Gigabytes (GB) \n");
				printf("6. Terabytes (TB) \n");
                
				printf("\n\nSelect Data Unit: ");
                scanf("%d",&s);
                printf("\nConver to: ");
                scanf("%d",&d);
                
                if(s==1&&d==2) //for bit to bytes
                {
                	system("cls");
                	
                	printf("Bits To Bytes");
                	printf("\n\nEnter Value (bits): ");
                	scanf("%lf",&bt);
                	a=bt*0.125;
                	system("cls");
                	printf("Converted...");
                	printf("\n%.2lf Bits equal to: %.2lf Bytes",bt,a);
                	printf("\n\nContinue using Converter (Y/N)....");
				}
				if(s==1&&d==3) //for bit to kilobytes
				{
					system("cls");
					
					printf("Bits To Kilobytes(KB) \n");
					printf("\n\nEnter Value (bits): \n");
					scanf("%lf",&bt);
					a=bt/1000;
					system("cls");
					printf("Converted....\n");
					printf("\n%.2lf Bits equal to: %.2lf KB \n",bt,a);
					printf("\n\nContinue using Converter (Y/N)....");
				}
				if(s==1&&d==4) //for bits to megabytes
				{
					system("cls");
				    
					printf("Bits To Megabytes(MB) \n");
					printf("\n\nEnter Value (bits): \n");
					scanf("%lf",&bt);
					a=bt/1000000;
					system("cls");
					printf("Converted.... \n");
					printf("\n%.2lf Bits equal to: %.2lf MB \n",bt,a);
					printf("\n\nContinue using Converter (Y/N).... \n");
				}
				if(s==1&&d==5) //for bit to gigabytes
				{
					system("cls");
					
					printf("Bits To Gigabytes(GB)  \n");
					printf("\n\nEnter Value (bits): \n");
					scanf("%lf",&bt);
					a=bt/1000000000;
					system("cls");
					printf("Converted.... \n");
					printf("\n%.2lf Bits equal to: %.2lf GB \n",bt,a);
					printf("\n\nContinue using Converter (Y/N).... \n");
				}
				if(s==1&&d==6) //for bit to terabytes
				{
					system("cls");
					
					printf("Bits To Terabytes(TB) \n");
					printf("\n\nEnter Value (bits): \n");
					scanf("%lf",&bt);
					a=bt*0.00000000000012;
					
					system("cls");
				     printf("Converted.... \n");
					printf("\n%.2lf Bits equal to: %.2lf TB \n",bt,a);
					printf("\n\nContinue using Converter (Y/N).... \n");
				}
				if(s==2&&d==1) //for bytes to bits
				{
					system("cls");
					
					printf("Bytes To Bits \n");
					printf("\n\nEnter Value (bytes): \n");
					scanf("%lf",&byt);
					a=byt*8;
					
					system("cls");
					printf("Converted....\n");
					printf("\n%.2lf Bytes equal to: %.2lf Bits \n",byt,a);
					printf("\n\nContinue using Converter (Y/N).... \n");
				}
				if(s==2&&d==3) //for bytes to kilobytes
				{
					system("cls");
					printf("Bytes To Kilobytes(KB) \n");
					printf("\n\nEnter Value (bytes): \n");
					scanf("%lf",&byt);
					a=byt/kbs;
					system("cls");
					printf("Converted.... \n");
					printf("\n%.2lf Bytes equal to: %.2lf KB \n",byt,a);
					printf("\n\nContinue using Converter (Y/N).... \n");
				}
				if(s==2&&d==4) //for bytes to megabytes
				{
					system("cls");
					printf("Bytes To Megabytes(MB) \n");
					printf("\n\nEnter Value (bytes): \n");
					scanf("%lf",&byt);
					a=byt/kbs/mbs;
					system("cls");
					printf("Converted.... \n");
					printf("\n%.2lf Bytes equal to: %.2lf MB \n",byt,a);
					printf("\n\nContinue using Converter (Y/N).... \n");
				}
				if(s==2&&d==5) //for bytes to gigabytes
				{
					system("cls");
					
					printf("Bytes To Gigabytes(GB) \n");
					printf("\n\nEnter Value (bytes): \n");
					scanf("%lf",&byt);
					a=byt/kbs/mbs/gbs;
					system("cls");
					printf("Converted.... \n");
					printf("\n%.2lf Bytes equal to: %.2lf GB \n",byt,a);
					printf("\n\nContinue using Converter (Y/N)....");
				}
				if(s==2&&d==6) //for bytes to terabytes
				{
					system("cls");
					printf("Bytes To Terabytes(TB) \n");
					printf("\n\nEnter Value (bytes): \n");
					scanf("%lf",&byt);
					a=byt/kbs/mbs/gbs/tbs;
					system("cls");
					printf("Converted....\n");
					printf("\n%.2lf Bytes equal to: %.2lf TB \n",byt,a);
					printf("\n\nContinue using Converter (Y/N).... \n");
				}
				if(s==3&&d==1) //kilobytes to bits
				{
					system("cls");
					printf("Kilobytes(KB) To Bits \n");
					printf("\n\nEnter Value (KB): \n");
					scanf("%lf",&kb);
					a=kb*8000;
					system("cls");
					printf("Converted.... \n");
					printf("\n%.2lf KB equal to: %.2lf Bits \n",kb,a);
					printf("\n\nContinue using Converter (Y/N)....");
				}
				if(s==3&&d==2) //kilobytes to bytes
				{
					system("cls");
					printf("Kilobytes(KB) To Bytes \n");
					printf("\n\nEnter Value (KB): \n");
					scanf("%lf",&kb);
					a=kb*1024;
					system("cls");
					printf("Converted....\n");
					printf("\n%.2lf KB equal to: %.2lf Bytes \n",kb,a);
					printf("\n\nContinue using Converter (Y/N)....");
				}
				if(s==3&&d==4) //kilobytes to megabytes
				{
					system("cls");
					printf("Kilobytes(KB) To Megabytes(MB) \n");
					printf("\n\nEnter Value (KB): \n");
					scanf("%lf",&kb);
					a=kb/mbs;
					system("cls");
					printf("Converted....\n");
					printf("\n%.2lf KB equal to: %.2lf MB \n",kb,a);
					printf("\n\nContinue using Converter (Y/N)....");
				}
				if(s==3&&d==5) //kilobytes to gigabytes
				{
					system("cls");
					printf("Kilobytes(KB) To Gigabytes(GB) \n");
					printf("\n\nEnter Value (KB): \n");
					scanf("%lf",&kb);
					a=kb/mbs/gbs;
					system("cls");
					printf("Converted....\n");
					printf("\n%.2lf KB equal to: %.2lf GB \n",kb,a);
					printf("\n\nContinue using Converter (Y/N)....");
				}
				if(s==3&&d==6) //kilobytes to terabytes
				{
					system("cls");
					printf("Kilobytes(KB) To Terabytes(TB) \n");
					printf("\n\nEnter Value (KB): \n");
					scanf("%lf",&kb);
					a=kb/mbs/gbs/tbs;
					system("cls");
					printf("Converted.... \n");
					printf("\n%.2lf KB equal to: %.2lf TB \n",kb,a);
					printf("\n\nContinue using Converter (Y/N)....");
				}
				if(s==4&&d==1) //for megabytes to bits
				{
					system("cls");
					printf("Megabytes(MB) To Bits \n");
					printf("\n\nEnter Value (MB): \n");
					scanf("%lf",&mb);
					a=mb*8000000;
					system("cls");
					printf("Converted.... \n");
					printf("\n%.2lf MB equal to: %.2lf Bits \n",mb,a);
					printf("\n\nContinue using Converter (Y/N)....");
				}
				if(s==4&&d==2) //for megabytes to bytes
				{
					system("cls");
					printf("Megabytes(MB) To Bytes \n");
					printf("\n\nEnter Value (MB): \n");
					scanf("%lf",&mb);
					a=mb*mbs*bytes;
					system("cls");
					printf("Converted.... \n");
					printf("\n%.2lf MB equal to: %.2lf Bytes \n",mb,a);
					printf("\n\nContinue using Converter (Y/N)....");
				}
				if(s==4&&d==3) //for megabytes to kilobytes
				{
					system("cls");
					printf("Megabytes(MB) To Kilobytes(KB) \n");
					printf("\n\nEnter Value (MB): \n");
					scanf("%lf",&mb);
					a=mb*kbs;
					system("cls");
					printf("Converted.... \n");
					printf("\n%.2lf MB equal to: %.2lf KB \n",mb,a);
					printf("\n\nContinue using Converter (Y/N)....");
				}
				if(s==4&&d==5)//for megabytes to gigabytes
				{
					system("cls");
					printf("Megabytes(MB) To Gigabytes(GB) \n");
					printf("\n\nEnter Value (MB): \n");
					scanf("%lf",&mb);
					a=mb/kbs;
					system("cls");
					printf("Converted.... \n");
					printf("\n%.2lf MB equal to: %.2lf GB \n",mb,a);
					printf("\n\nContinue using Converter (Y/N)....");
				}
				if(s==4&&d==6)//for megabytes to terabytes
				{
					system("cls");
					printf("Megabytes(MB) To Terabytes(TB) \n");
					printf("\n\nEnter Value (MB): \n");
					scanf("%lf",&mb);
					a=mb/kbs/gbs;
					system("cls");
					printf("Converted.... \n");
					printf("\n%.2lf MB equal to: %.2lf TB \n",mb,a);
					printf("\n\nContinue using Converter (Y/N)....");
				}
				if(s==5&&d==1) //for gigabytes to bits
				{
					system("cls");
					printf("Gigabytes(GB) To Bits \n");
					printf("\n\nEnter Value (GB): \n");
					scanf("%lf",&gb);
					a=gb*8000000000;
					system("cls");
					printf("Converted....\n");
					printf("\n%.2lf GB equal to: %.2lf Bits \n",gb,a);
					printf("\n\nContinue using Converter (Y/N)....");
				}
				if(s==5&&d==2) //for gigabytes to bytes
				{
					system("cls");
					printf("Gigabytes(GB) To Bytes \n");
					printf("\n\nEnter Value (GB): \n");
					scanf("%lf",&gb);
					a=gb*mbs*kbs*bytes;
					system("cls");
					printf("Converted....\n");
					printf("\n%.2lf GB equal to: %.2lf Bytes \n",gb,a);
					printf("\n\nContinue using Converter (Y/N)....");
				}
				if(s==5&&d==3) //for gigabytes to kilobytes
				{
					system("cls");
					printf("Gigabytes(GB) To Kilobytes(KB) \n");
					printf("\n\nEnter Value (GB): \n");
					scanf("%lf",&gb);
					a=gb*mbs*kbs;
					system("cls");
					printf("Converted.... \n");
					printf("\n%.2lf GB equal to: %.2lf KB \n",gb,a);
					printf("\n\nContinue using Converter (Y/N)....");
				}
				if(s==5&&d==4) //for gigabytes to megabytes
				{
					system("cls");
					printf("Gigabytes(GB) To Megabytes(MB) \n");
					printf("\n\nEnter Value (GB): \n");
					scanf("%lf",&gb);
					a=gb*mbs;
					system("cls");
					printf("Converted.... \n");
					printf("\n%.2lf GB equal to: %.2lf MB \n",gb,a);
					printf("\n\nContinue using Converter (Y/N)....");
				}
				if(s==5&&d==6) //for gigabytes to terabytes
				{
					system("cls");
					printf("Gigabytes(GB) To Terabytes(TB) \n");
					printf("\n\nEnter Value (GB): \n");
					scanf("%lf",&gb);
					a=gb/tbs;
					system("cls");
					printf("Converted.... \n");
					printf("\n%.2lf GB equal to: %.2lf TB \n",gb,a);
					printf("\n\nContinue using Converter (Y/N)....");
				}
				if(s==6&&d==1) //for Terabytes to Bits
				{
					system("cls");
					printf("Terabytes(TB) To Bits \n");
					printf("\n\nEnter Value (TB): \n");
					scanf("%lf",&tb);
					a=tb*8000000000000;
					system("cls");
					printf("Converted.... \n");
					printf("\n%.2lf TB equal to: %.2lf Bits \n",tb,a);
					printf("\n\nContinue using Converter (Y/N)....");
				}
				if(s==6&&d==2) //for Terabytes to Bytes
				{
					system("cls");
					printf("Terabytes(TB) To Bytes \n");
					printf("\n\nEnter Value (TB): \n");
					scanf("%lf",&tb);
					a=tb*gbs*mbs*kbs*bytes;
					system("cls");
					printf("Converted....\n");
					printf("\n%.2lf TB equal to: %.2lf Bytes \n",tb,a);
					printf("\n\nContinue using Converter (Y/N)....");
				}
				if(s==6&&d==3) //for Terabytes to Kilobytes
				{
					system("cls");
					printf("Terabytes(TB) To Kilobytes(KB) \n");
					printf("\n\nEnter Value (TB):  \n");
					scanf("%lf",&tb);
					a=tb*gbs*mbs*kbs;
					system("cls");
					printf("Converted.... \n");
					printf("\n%.2lf TB equal to: %.2lf KB \n",tb,a);
					printf("\n\nContinue using Converter (Y/N)....");
				}
				if(s==6&&d==4) //for Terabytes to Megabytes
				{
					system("cls");
					printf("Terabytes(TB) To Megabytes(MB) \n");
					printf("\n\nEnter Value (TB): \n");
					scanf("%lf",&tb);
					a=tb*gbs*mbs;
					system("cls");
					printf("Converted....\n");
					printf("\n%.2lf TB equal to: %.2lf MB \n",tb,a);
					printf("\n\nContinue using Converter (Y/N)....");
				}
				if(s==6&&d==5) //for Terabytes to Gigabytes
				{
					system("cls");
					printf("Terabytes(TB) To Gigabytes(GB) \n");
					printf("\n\nEnter Value (TB): \n");
					scanf("%lf",&tb);
					a=tb*gbs;
					system("cls");
					printf("Converted.... \n");
					printf("\n%.2lf TB equal to: %.2lf GB \n",tb,a);
					printf("\n\nContinue using Converter (Y/N)....");
				}
				if(s==d) //for same selection notification
				{
				printf("\n\nSame Unit Not Allowed");
				printf("\n\nPress Y to Continue....");
				}
				else if(s>6||s<1||d>6||d<1) //for out of option selection notification
				{
					printf("\nPlease Select Between 1 and 6");
					printf("\n\nPress Y to Continue....");
				}
                fflush(stdin);
                another = getche();
			}
			break;
				
        case '3':
            exit(0); /// exit from the program
        }
    }
    return 0;
}
