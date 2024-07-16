# DIAGONAL-ELEMENTS-SUM
import java.util.*;
class Main {
    public static void main(String[] args) {
        int c=0;
        Scanner sc= new Scanner(System.in);
          System.out.println("Enter array length: ");
        int n=sc.nextInt();// Array length
         int [][]a=new int[n][n];
         int sum=0;
          System.out.println("Enter array1 elements: ");
        for(int i=0;i<n;i++){
            for(int j=0;j<n;j++){
            int k=sc.nextInt();
            a[i][j]=k;
            }
        }
        for (int i=0;i<n;i++){
            for(int j=0;j<n;j++){
                if (i==j)
                sum=sum+a[i][j];
                else if ((i==0) && (j==2)||(i==2) && (j==0))
                sum+=a[i][j];
             
            }
           
        }
         System.out.println("Sum: "+sum);
    }
}
