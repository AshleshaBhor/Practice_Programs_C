# Practice_Programs_C
/**************************************************/
//
//Author : Ashlesha Bhor
//Date : 19/09/2022
//Subject : Problems on Numbers
//
/**************************************************/


/**************************************************/



/*******************Imports************************/
#include<stdio.h>
#include<stdbool.h>

/*******************Helper Functions****************/


//Program to add 2 numbers
int Addition(int iNo1, int iNo2)
{
    int iRet = 0;
    iRet = iNo1 + iNo2;
    return iRet;
}


//Program to display class from percentage
void grade(float fPer)
{
     if(fPer >= 70.00)
     { 
        printf("Distinction");
     }
     else if(fPer >= 60.00 && fPer < 70.00)
     {
         printf("First Class");
     }
     else if(fPer >= 50.00 && fPer < 60.00)
     { 
          printf("Second Class");
     }
     else if(fPer >= 35.00 && fPer < 50.00)
     {
          printf("Pass Class");
     }
     else
     {
           printf("Fail");
     }
}



//Program to display City Name using city code
void cityCode(int iCode)
{
     switch(iCode)
     {
         case 01: printf("Mumbai");
                                 break;
         case 02: printf("Pune");
                                break;
         case 03 : printf("Manchar");
                                 break;
         case 04 : printf("Nashik");
                                  break;
         case 05 : printf("Nanded");
                                  break;
         default : printf("Invalid Code");
                                   break;
     }
}


//WAP which accept a number from user and display it for 5 times
void DisplayNum(int iNo)
{
   int iCnt = 0;
   
   for(iCnt = 1; iCnt <= iNo; iCnt++)
   {
       printf("%d\t",iNo);
   }
}

//Accept number from user & check whether it is divisible by 5 and 3
bool ChkNum(int iNo)
{
   int iCnt = 0;

   for(iCnt = 1; iCnt <= iNo; iCnt++)
   {
       if(iNo % 3 == 0 && iNo % 5 == 0)
       {
           return true;
       }
       else
       {
          return false;
       }
   }
}



/**********************Driver Function************************/
int main()
{
   /*int iValue1 = 0, iValue2 = 0, iRet = 0;
   printf("Enter the First Number:\n");
   scanf("%d",&iValue1);
   
   printf("Enter the Second Number:\n");
   scanf("%d",&iValue2);
 
   iRet = Addition(iValue1,iValue2);
   printf("Addition is: %d",iRet);*/


   /*float fPer = 0.0;
   printf("Enter the Percentage :\n");
   scanf("%d",&fPer);
   grade(fPer);*/

   /*int iCode;
   printf("Enter the City code :\n");
   scanf("%d",&iCode);
   cityCode(iCode);*/

   int iValue = 0;
   bool bRet;
  
   printf("Enter the Number:\n");
   scanf("%d",&iValue);
 
   bRet = ChkNum(iValue);
   if(bRet == true)
   {
      printf("%d is divisible by 3 and 5",iValue);
   }
   else
   {
      printf("%d is not divisible by 3 and 5",iValue);
   }

   
   return 0;
     
}
