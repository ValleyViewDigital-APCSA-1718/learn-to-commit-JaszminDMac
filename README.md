# learn-to-commit-JaszminDMac
learn-to-commit-JaszminDMac created by GitHub Classroom

/**
 * Jaszmin Delt-Makey
 * 9-8-17
 * PP 2.9
 * */

import java.util.Scanner;
import java.text.DecimalFormat;

public class SphereStats
{
    public static void main(String[] args)
    {
        int radius;
        double area, volume;
        Scanner keyboard = new Scanner(System.in);
        
        System.out.print ("Enter the sphere's radius: ");
        radius = keyboard.nextInt();

        area = 4 * Math.PI * Math.pow(radius, 2);
        volume = (4/3) * Math.PI * Math.pow(radius, 3);
        
        DecimalFormat fmt = new DecimalFormat("0.####");
        
        System.out.println("The sphere's volume:" + fmt.format(volume));
        System.out.println("The sphere's surface area: " + fmt.format(area));
        
    }// end method main
    
}// end class SphereStats


/**
 * Jaszmin Delt-Makey
 * 9-7-17
 * Classwork #3
 * */
import java.util.Calendar;
import java.util.Locale;

public class usePrintF
{
    public static void main(String[] args)
    {
        long n = 461012;
        System.out.format("%d%n", n);  // ---> "461012"
        System.out.format("%08d%n", n); // ---> "00461012"
        System.out.format("%+8d%n" , n); // ---> " +461012"
        System.out.format("%,8d%n" , n); // ---> " 461,012"
        System.out.format("%+,8d%n%n" , n); // ---> "461,012"
        
        double pi = Math.PI;
        
        System.out.format("%f%n", pi);   // ---> "3.141593"
        System.out.format("%.3f%n", pi); // ---> "3.142"
        System.out.format("%10.3f%n", pi); // ---> "     3.142"
        System.out.format("%-10.3f%n", pi); // ---> "3.142"
        System.out.format(Locale.FRANCE,
                         "%-10.4f%n%n", pi); // ---> "3,1416"
      
        Calendar c = Calendar.getInstance();
        System.out.format("%tB %te, %tY%n", c, c, c); // ---> "May 29, 2006"
        
        System.out.format("%tl:%tM %tp%n", c, c, c); // ---> "2:34 am"
        
        System.out.format("%tD%n", c);              // ---> "05/29/06"
        
    
    }// end method main
    
}// end class usePrintF


