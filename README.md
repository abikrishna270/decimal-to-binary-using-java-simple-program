# decimal-to-binary-using-java-simple-program
package com.company;

import java.util.Scanner;

public class decimaltobinary {

    public static void main(String[] args) {
	System.out.println("ENTER THE DECIMAL NUMBER");
    }
}

    	Scanner sc =new Scanner(System.in);
    int dec=sc.nextInt();
    int array[]=new int[200];
    int i;
    for( i=0;i<=100;i++){
        array[i]=dec%2;
        dec=dec/2;
        if(dec<1){
            break;
        }
    }
    int j;
    for( j=i;j>=0;j--){
        System.out.print(array[j]);
    }
