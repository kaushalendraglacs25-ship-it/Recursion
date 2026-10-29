# Recursion
WEEKLY ASSIGNMENT QUESTION SOLVE TO IMPROVE THEIR LOGICAL THINKING AND PROBLEM SOLVING SKILLS 
//QUES-1:PRINT THE VALUES UP TO 5-
// public class Recursion{
//     public static void funct1(int n){
//     if(n==6)
//     return;
//     System.out.print(n+" ");
//     funct1(n+1);
//     }
// public static void main(String args[]){
//  int n=1;
//  funct1(n);
//     }
// }


//QUES-2:Print the values from 5 to 0-
// public class Recursion{
//     public static void funct(int n){
//         if(n==0)
//         return;
//         System.out.print(n+" ");
//         funct(n-1);
//     }
// public static void main(String args[]){
// int n=5;
// funct(n);
// }
// }


//QUES-3:FIRST N NATIRAL NUMBERS SUM-
// public class Recursion{
// public static void funct(int i,int n,int sum){
//     if(i==n){
//         sum=sum+i;
//     System.out.println("RECURSIVE SUM:-"+sum);
//     return;
// }
//     sum=sum+i;
//     funct(i+1,n,sum);
//     }
// public static void main(String args[]){
//     int i=1;
//     int n=5;
//     int sum=0;
//     funct(i,n,sum);
//     }
// }


//QUES-4:FACTORIAL OF A NUMBER-
// public class Recursion{
// public static void funct(int i,int n,int fact){
// if(i==n){
// fact=fact*i;
// System.out.println("FACTORIAL IS:"+fact);
// return;
//}
// fact=fact*i;
// funct(i+1,n,fact);
//}
// public static void main(String[] args) {
// int i=1;
// int n=5;
// int fact=1;
// funct(i,n,fact);
// }
// }


//Fibonnaci Series:-
// import java.util.Scanner;
// public class Recursion{
// public static void main(String args[]){
// Scanner sc = new Scanner(System.in);
// int n=sc.nextInt();
// int a=0;
// int b=1;
// for(int i=0;i<n;i++){
// System.out.print(a+" ");
//         int c=a+b;
//         a=b;
//         b=c;}
//     sc.close();} }


//QUES-5:Recursion Fibonnaci Series:-
// public class Recursion{
// public static void funct(int i,int n,int a,int b){
// if(i==n){
// return;}
// System.out.print(a+" ");
// int c=a+b;
// a=b;
// b=c;
// funct(i+1,n,a,b);}
// public static void main(String args[]){
// int a=0;
// int i=0;
// int n=5;
// int b=1;
// funct(i,n,a,b); } }


//Ques-6:-Check Palindrome String using Recursion:-
// import java.util.*;
// public class Recursion{
//     public static void funct(String str,int left,int right){
// if(left>=right){
//     System.out.print(str+" is a palindrome");
// return;
// }
// if(str.charAt(left)!=str.charAt(right)){
//     System.out.print(str+" is Not Palindrome");
//     return;
// }
// funct(str,left+=1,right-=1);}
// public static void main(String args[]){
// Scanner sc = new Scanner(System.in);
// System.out.print("Enter A String:");
// String str=sc.nextLine().toUpperCase();
// //MADAM:
// int left=0;
// int right=str.length()-1;
// funct(str,left,right);
//    sc.close(); } }


//QUES-7:CHECK IF AN ARRAY IS SORTED OR NOT:
//(SIMPLE METHOD)-

// import java.util.*;
// public class Recursion{
//     public static void funct(int n){
//     }
// public static void main(String args[]){
// Scanner sc = new Scanner(System.in);
// int n= sc.nextInt();
// int arr[]=new int[n];
// boolean sorted =true;
// for(int i=0;i<arr.length;i++){
//     arr[i]=sc.nextInt();
// }
// //1 2 3 4 5 
// for(int i=0;i<arr.length-1;i++){
// if(arr[i]>arr[i+1]){
//     sorted=false;
//     break;
// }
// }
// if(sorted){
//     System.out.println("Arrays is Sorted");
// }
// else{
//     System.out.println("Array is not sorted");
// }
// sc.close();    }
// }

//QUES-7:using pointer:-

// public class Recursion{
// public static void main(String args[]){
// int arr[]={1,2,1,2,3};     
// int left=0;
// int right=arr.length-1;
// boolean sorted=true;
// while(left<right){
// if(arr[left]>arr[left+1]){
// sorted = false;
// break;}
// left++;
// }
// if(sorted){
//     System.out.println("Array is sorted");
// }
// else{
//     System.out.println("Array is not Sorted");
// }
// }
//     }

//Check array is sorted using Recursion:
// import java.util.*;
// public class Recursion{
//     public static void funct(int n,boolean sorted,int arr[],int left,int right){
//     if(left>=right){
//         if(sorted){
//             System.out.println("Array is sorted");
//         }
//         else{
//             System.out.println("Array is not sorted");
//         }
//         return;
//     }
//     if(arr[left]>arr[left+1]){
//     sorted=false;
//     }
//     funct(n,sorted,arr,left+=1,right);
//     }
// public static void main(String args[]){
// Scanner sc = new Scanner(System.in);
// int n = sc.nextInt();
// int arr[]=new int[n];
// boolean sorted=true;
// int left=0;
// int right=n-1;
// for(int i=0;i<arr.length;i++){
// arr[i]=sc.nextInt();
// }
// funct(n,sorted,arr,left,right);
//   sc.close();  }
// }
