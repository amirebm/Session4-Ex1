
//  برنامه ایی بنوسید که تعدادی عدد از ورودی گرفته و مجموع آنها را چاپ کند 
# Session4-Ex1

package com.personal.Ex1;

import java.util.Scanner;

public class Ex1 {

	public static void main(String[] args) {
		
		int arrayLength, sum=0;
		Scanner sc= new Scanner(System.in);
		System.out.println("Enter a ths size of array");
		arrayLength=sc.nextInt();
	
		int[] ar= new int[arrayLength];
		System.out.println("the length of  array is: " + (arrayLength));
		System.out.println("Please enter the numbers of array:");

		for (int i=0; i<arrayLength; i++) {
			
			System.out.println(String.format("ar[%d]:", i));		
			ar[i]= sc.nextInt();
				
			}
		
            for (int i=0; i<arrayLength; i++) {
            	
			System.out.println(String.format("ar[%d]= %d", i, ar[i]));		
				sum += ar[i];
			}
            System.out.println("The sum of the array is: "+ sum);
        
			}
	
	
}
