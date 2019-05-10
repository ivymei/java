# java
###### ArrayOperation
package javaapplication1;

/**
   This program demonstrates a switch statement.
*/

public class ArrayOperation
{
   public static void main(String[] args)
   {      
       int [] arr = { 1, 2, 3, 4, 5, 6, 7, 8};
       
       System.out.println("Total = " + getTotal(arr));
       System.out.println("Average = " + getAverage(arr));
       System.out.println("highest = " + getHighest(arr));
       System.out.println("lowest = " + getLowest(arr));    
   }
   
   public static int getTotal(int[] arr)
   {
       int total = 0;
       for( int i=0; i<arr.length; i++)
       {
           total = total + arr[i];
       }
       
       return total;
   }
   
   public static double getAverage(int[] arr)
   {
       double total = getTotal(arr);
       
       return total/arr.length;
   }
   
   public static int getHighest(int[] arr)
   {
       int highest = arr[0];
       for( int i=1; i<arr.length; i++)
           if(highest<arr[i])
               highest = arr[i];
       return highest;
   }
   
   public static int getLowest(int[] arr)
   {
       int lowest = arr[0];
       for( int i=1; i<arr.length; i++)
           if(lowest>arr[i])
               lowest = arr[i];
       return lowest;
   }
}

