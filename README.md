# Write-a-program-that-allows-input-n-then-input-n-integer-elements-can-be-positive-or-negative-.
Write a program that allows input n, then input n integer elements (can be positive or negative).
import java.util.Scanner;
public class BaiTapJavaCoBan13
{
    public static void main(String[] args)
    {
       int n;
       int[] soNguyen;
       int min = 0;
       Scanner sc = new Scanner(System.in);

       System.out.println("Enter n:");
       n = sc.nextInt();
       soNguyen = new int[n];
       for (int i = 0; i < n; i++)
       {
          System.out.println("Integer:");
          soNguyen[i] = sc.nextInt();
       }

       min = soNguyen[0];

       for (int i = 0; i < n; i++)
       {
          if(soNguyen[i] < min)
          min = soNguyen[i];
       }

       System.out.println("Minimum element is: " + min);
    }
}
