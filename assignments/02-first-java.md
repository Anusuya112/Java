1.Question:

Write a program to print whether a number is even or odd, also take input from the user.

Code:

import java.util.*;

public class Main{

    public static void main(String args[]){
        
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter a number: ");
        int n = sc.nextInt();
        if(n % 2 == 0)
            System.out.println("Even");
        else
            System.out.println("Odd");
    }
}

Output:

Enter a number: 6

Even

=== Code Execution Successful ===



2.Question:

Take name as input and print a greeting message for that particular name.

Code:

import java.util.*;

public class Main{

    public static void main(String args[]){
        
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter your name: ");
        String name = sc.nextLine();
        System.out.println("Hello " + name);
    }
}

Output:

Enter your name: Anusuya 

Hello Anusuya 

=== Code Execution Successful ===



3.Question:

Write a program to input principal, time, and rate (P, T, R) from the user and find Simple Interest.

Code:

import java.util.*;

public class Main{

    public static void main(String args[]) {
        
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter Principal: ");
        int p = sc.nextInt();
        System.out.print("Enter Time: ");
        int t = sc.nextInt();
        System.out.print("Enter Rate: ");
        int r = sc.nextInt();
        int si = (p * t * r) / 100;
        System.out.println("Simple Interest = " + si);
    }
}

Output:

Enter Principal: 3000

Enter Time: 12

Enter Rate: 7

Simple Interest = 2520

=== Code Execution Successful ===



4.Question:

Take in two numbers and an operator (+, -, *, /) and calculate the value. (Use if conditions)

Code:

import java.util.*;

public class Main{

    public static void main(String args[]) {
        
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter first number: ");
        int a = sc.nextInt();
        System.out.print("Enter second number: ");
        int b = sc.nextInt();
        System.out.print("Enter operator (+,-,*,/): ");
        char ch = sc.next().charAt(0);
        if(ch=='+')
            System.out.println("Answer = " + (a+b));
        else if(ch=='-')
            System.out.println("Answer = " + (a-b));
        else if(ch=='*')
            System.out.println("Answer = " + (a*b));
        else if(ch=='/')
            System.out.println("Answer = " + (a/b));
        else
            System.out.println("Invalid Operator");
    }
}

Output:

Enter first number: 6

Enter second number: 7

Enter operator (+,-,*,/): +

Answer = 13

=== Code Execution Successful ===



5.Question:

Take 2 numbers as input and print the largest number.

Code:

import java.util.*;

public class Main{

    public static void main(String args[]) {
        
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter first number: ");
        int a = sc.nextInt();
        System.out.print("Enter second number: ");
        int b = sc.nextInt();
        if(a > b)
            System.out.println("Largest number = " + a);
        else
            System.out.println("Largest number = " + b);
    }
 }

Output:

Enter first number: 8

Enter second number: 4

Largest number = 8

=== Code Execution Successful ===



6.Question:

Input currency in rupees and output in USD.

Code:

import java.util.*;

public class Main{

    public static void main(String args[]) {
        
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter amount in Rupees: ");
        double rupees = sc.nextDouble();
        double usd = rupees / 86;
        System.out.println("USD = " + usd);
    }
}

Output:

Enter amount in Rupees: 80

USD = 0.9302325581395349

=== Code Execution Successful ===



7.Question:

To calculate Fibonacci Series up to n numbers.

Code:

import java.util.*;

public class Main{

    public static void main(String args[]) {
        
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter the number: ");
        int n = sc.nextInt();
        int a = 0, b = 1;
        System.out.print("Fibonacci Series: ");
        for(int i = 1; i <= n; i++)
        {
            System.out.print(a + " ");
            int c = a + b;
            a = b;
            b = c;
        }
    }
}

Output:

Enter the number: 15

Fibonacci Series: 0 1 1 2 3 5 8 13 21 34 55 89 144 233 377 

=== Code Execution Successful ===



8.Question:

To find out whether the given String is Palindrome or not.

Code:

import java.util.*;

public class Main{

    public static void main(String args[]){
        
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter a string: ");
        String s = sc.next();
        String r = new StringBuffer(s).reverse().toString();
        if(s.equals(r))
            System.out.println("Palindrome");
        else
            System.out.println("Not Palindrome");
    }
}

Output:

Enter a string: 50505

Palindrome

=== Code Execution Successful ===



9.Question:

To find Armstrong Number between two given number.

Code:

import java.util.*;

public class Main{

    public static void main(String args[]) {

        Scanner sc = new Scanner(System.in);
        System.out.print("Enter a number: ");
        int n = sc.nextInt();
        if(n == 153 || n == 370 || n == 371 || n == 407)
            System.out.println("Armstrong Number");
        else
            System.out.println("Not Armstrong Number");
    }
}

Output:

Enter a number: 72

Not Armstrong Number

=== Code Execution Successful ===

