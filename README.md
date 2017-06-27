import java.util.*;
class solution1
{
public static void main(String s[])
{
int b=0,c,num,asum=0,bsum;
int a[]=new int[50];
System.out.println("Enter the number");
Scanner obj=new Scanner(System.in);
num=obj.nextInt();
  for(int i=1;i<=num/2;i++)
   {
    if(num%i==0)
    asum=asum+i;
    }
System.out.println("Aliquotsum="+asum);
if(asum==num)
 {
  System.out.println("The number you entered is a perfect number");
 }
else
  {
  System.out.println("The number you entered is not  a perfect number");
  }
int k=0;
System.out.println("The perfect numbers between 1 to 100 are ");
  for(int j=2;j<=100;j++)
 {
   bsum=1;
   for(int i=2;i<j;i++)
   {
    if(j%i==0)
    bsum=bsum+i;
    }
   if(j==bsum){
   System.out.println(j);
   }
 }

}
}

