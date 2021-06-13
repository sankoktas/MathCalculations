import java.util.Scanner;

import java.lang.Math;

public class KFS_MathCalculations_Main

{

    public static void main(String[] args)
    {
       //problem 1 
       Scanner input = new Scanner(System.in);
       System.out.println("Enter coefficients for the quadratic equation below.");
       System.out.println("If it gives 'NaN' as the roots, it means there are no real solutions for the equation you provided and roots are imaginary");
       System.out.print("a: ");
       double a = input.nextDouble();
       System.out.print("b: ");
       double b = input.nextDouble();
       System.out.print("c: ");
       double c = input.nextDouble();
       double r1, r2; 
       r1 = (-b + Math.sqrt(Math.pow(b, 2) - 4*a*c)) / (2*a);
       r2 = (-b - Math.sqrt(Math.pow(b, 2) - 4*a*c)) / (2*a);
       System.out.println("First root is " + r1);
       System.out.println("Second root is " + r2);
       
       //problem 2 
       System.out.println("Enter the x coordinate of the first point below");
       System.out.print("x1: ");
       double x1 = input.nextDouble();
       System.out.println("Enter the y coordinate of the first point below");
       System.out.print("y1: ");
       double y1 = input.nextDouble();
       System.out.println("Enter the x coordinate of the second point below");
       System.out.print("x2: ");
       double x2= input.nextDouble();
       System.out.println("Enter the y coordinate of the second point below");
       System.out.print("y2: ");
       double y2= input.nextDouble();
       double distance = Math.sqrt(Math.pow((x1-x2), 2) + Math.pow((y1-y2), 2)); 
       System.out.println("Distance between points (x1: " + x1 + ", y1: " + y1 + ") and (x2: " + x2 + ", y2: " + y2 + ") is " + distance );

       //problem 3
       double area = Math.PI * Math.pow(distance,2);
       System.out.println("The area of the circle with radius 5 is = " + area);
       
       //problem 4 
       System.out.println("The area " + area + " is rounded to " + Math.round(area));
       
       //problem 5
       System.out.println("The ceiling value of " + area + " is: " + Math.ceil(area));
       System.out.println("The floor value of " + area + " is: " + Math.floor(area));
       
       //problem 6 
       System.out.println("The difference between " + Math.ceil(area) + " and " + Math.floor(area) + " is: " + Math.abs(Math.ceil(area)-Math.floor(area)));
    }
 }
