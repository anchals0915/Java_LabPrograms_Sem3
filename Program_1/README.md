Aim: 
Introduce the java fundamentals, data types, operators in java

Program: 
Write a java program that prints all real solutions to the quadratic equation ax2+bx+c=0. 
Read in a, b, c and use the quadratic formula.

    import java.util.*;
    import java.lang.*;

One popular way to read input from stdin is by using the Scanner class and specifying the Input Stream as System.in. 

    Scanner s =new Scanner(System.in);
    Scanner Class    s is the reference
		Scanner(System.in) here Scanner is the constructor
          s.nextInt();
          s.nextFloat();
          s.nextDouble();
          s.next();
          s.nextLine();
		
          s.nextByte();
          s.nextShort();
          s.nextLong();
          s.nextBoolean();

So before reading the data you should confirm what type of data you are getting 
s.hasNextInt(); - Returns a boolean True or False 
                  So whether the next letter that 
                 is coming in source is a integer or not.
s.hasNextFloat();


    a = s.nextInt();
    b = s.nextInt();
    c = a+ b ;
    System.out.println("Sum is "+ c);



For example:
	      
    Scanner scanner = new Scanner(System.in);
    String myString = scanner.next();
	  int myInt = scanner.nextInt();
	  scanner.close();


    System.out.println("myString is: " + myString);
    System.out.println("myInt is: " + myInt);


The code above creates a Scanner object named  and uses it to read a String and an int.
It then closes the Scanner object because there is no more input to read, and prints to stdout using System.out.println(String).
So, if our 
     
     Input :   
        Hi 5

Our code will print:
    
    Output :
    myString is: Hi 
    myInt is: 5


Alternatively, you can use the BufferedReader class.


    class ReadKeyboard
    {
        public static void main(String[] args)
        {
            Scanner sc = new Scanner(System.in);
            int x = sc.nextInt();
            System.out.println(x);
            float  y = sc.nextFloat();
            System.out.println(y);
		
            String  s1 = sc.next();
            System.out.println(s1);

            String  s2 = sc.nextLine();
            System.out.println(s2);
        }
    }

Program to print a decimal number where the input it in binary form 

    class ReadKeyboard
    {
        public static void main(String[] args)
        {      //----------> we enter a number in binary its equivalent is displayed.
            Scanner sc = new Scanner(System.in);
            sc.useRadix(2);
            int x = sc.nextInt();               //10-->2        100-->4     111-->7
            System.out.println(x);
        }
    }


Data Type 

  ~ Minimum value
  
  ~ Maximum value 
  
  ~ Bytes
  
  ~ Bits
  
    class DataSizeRange 
    {
        public static void main(String[] args) 
        {
              System.out.println("Byte Min Value : " + Byte.MIN_VALUE);
              System.out.println("Byte Max Value : " + Byte.MAX_VALUE);
              System.out.println("Byte Bytes : " + Byte.BYTES);
              System.out.println("Byte Size (bits) : " + Byte.SIZE);
        //   Byte Min Value : -128
        //   Byte Max Value : 127
        //   Byte Bytes : 1
        //   Byte Size (bits) : 8
          

              System.out.println("Short Min Value : " + Short.MIN_VALUE);
              System.out.println("Short Max Value : " + Short.MAX_VALUE);
              System.out.println("Short Bytes : " + Short.BYTES);
              System.out.println("Short Size (bits) : " + Short.SIZE);
        //   Short Min Value : -32768
        //   Short Max Value : 32767
        //   Short Bytes : 2
        //   Short Size (bits) : 16
        

              System.out.println("Int Min Value : " + Integer.MIN_VALUE);
              System.out.println("Int Max Value : " + Integer.MAX_VALUE);
              System.out.println("Int Bytes : " + Integer.BYTES);
              System.out.println("Int Size (bits) : " + Integer.SIZE);
        //   Int Min Value : -2147483648
        //   Int Max Value : 2147483647
        //   Int Bytes : 4
        //   Int Size (bits) : 32
         

              System.out.println("Long Min Value : " + Long.MIN_VALUE);
              System.out.println("Long Max Value : " + Long.MAX_VALUE);
              System.out.println("Long Bytes : " + Long.BYTES);
              System.out.println("Long Size (bits) : " + Long.SIZE);
        //   Long Min Value : -9223372036854775808
        //   Long Max Value : 9223372036854775807
        //   Long Bytes : 8
        //   Long Size (bits) : 64
        

              System.out.println("Float Min Value : " + Float.MIN_VALUE);
              System.out.println("Float Max Value : " + Float.MAX_VALUE);
              System.out.println("Float Bytes : " + Float.BYTES);
              System.out.println("Float Size (bits) : " + Float.SIZE);
        //   Float Min Value : 1.4E-45
        //   Float Max Value : 3.4028235E38
        //   Float Bytes : 4
        //   Float Size (bits) : 32
        

              System.out.println("Double Min Value : " + Double.MIN_VALUE);
              System.out.println("Double Max Value : " + Double.MAX_VALUE);
              System.out.println("Double Bytes : " + Double.BYTES);
              System.out.println("Double Size (bits) : " + Double.SIZE);
        //   Double Min Value : 4.9E-324
        //   Double Max Value : 1.7976931348623157E308
        //   Double Bytes : 8
        //   Double Size (bits) : 64
        
		  
              System.out.println("Char Min Value : " + Character.MIN_VALUE);
              System.out.println("Char Max Value : " + Character.MAX_VALUE);
              System.out.println("Char Bytes : " + Character.BYTES);
              System.out.println("Char Size (bits) : " + Character.SIZE);
            //  Char Min Value :
            //  Char Max Value : ?
            //  Char Bytes : 2
            //  Char Size (bits) : 16
        }
    }




A value in binary form or decimal form or octal form and hexadecimal form can be stored in a variable
  
  
    public class JavaProg 
    {
        public static void main(String[] args) 
        {
            byte b = 10;    //Decimal 
            byte b1 = 0b1010;   //Binary
            byte b2 = 012;  //Octal
            byte b3 = 0xA;  //Hexadecimal

            System.out.println(b);  //10    
            System.out.println(b1); //10
            System.out.println(b2); //10
            System.out.println(b3); //10
        }
    }
