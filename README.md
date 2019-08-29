package javaapplication19;

import java.util.Scanner;

/**
 *
 * @author LENOVO
 */
public class JavaApplication19 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        
         Scanner sc = new Scanner(System.in);
         
        int i;
        System.out.println("Input size of array: ");
        int kol=sc.nextInt();
        int[]array=new int[kol];
       
        System.out.println("Input elements of array: ");
        for( i=0; i<kol; i++)
           array[i]=sc.nextInt();
        
        System.out.println("Input sdvig of array: ");
        int s=sc.nextInt();
       for (int j=1; j<=s; j++){
        int b=array[0];
        for(i=0; i<kol-1; i++){
            array[i]=array[i+1];
        }
        
        array[kol-1]=b; 
       }
        System.out.println("Result: ");
       for( i=0; i<kol; i++)
            System.out.print(array[i]+" ");
    }
    
}
