# String-In-equal-Parts
By Using input Function string to be divided into equal parts!!
import java.util.*;
import java.util.Scanner;
class Main {
  public static void main(String[] args) {
    Scanner sc=new Scanner(System.in);
    System.out.println("Enter the string");//Take a input  from user
    String str=sc.next(); 
    System.out.println("enter the number which wll give the string divide");
     int n = sc.nextInt();//take the input for divide the string in that part
     int len = str.length();
       int temp = 0, chars = len/n;
     //String bag="";
     String[] equalStr = new String [n];//create a new string
     if(len % n != 0) //use  condition for if string not divided into such part
     { 
      System.out.println("notdivided into "+ n +" equal parts.");  
       }
    else
    {
       for(int i = 0; i < len; i = i+chars) //take a foor loop to print the string
       {  
       String part = str.substring(i, i+chars);  //use the function it gives equal part
          equalStr[temp] = part;  
          temp++;//add the string
        }
      for(int i=0;i<=equalStr.length;i++)//final string will be printed
        {
          
      System.out.println(equalStr[i]);
    }
  }
}
}

  //for(int i = 0; i < equalStr.length; i++) { 
   //  System.out.print(equalStr[i]);
   
