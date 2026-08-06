1.Question:

Define two methods to print the maximum and the minimum number respectively among three numbers entered by the user.

Program:

import java.util.*;
public class Main {
    static void max(int a,int b,int c){
        System.out.println("Maximum = " + Math.max(a, Math.max(b,c)));
    }
    static void min(int a,int b,int c){
        System.out.println("Minimum = " + Math.min(a, Math.min(b,c)));
    }
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        int a=sc.nextInt();
        int b=sc.nextInt();
        int c=sc.nextInt();
        max(a,b,c);
        min(a,b,c);
    }
}

2.Question:

Define a program to find out whether a given number is even or odd.

Program:

import java.util.*;
public class Main{
    static void check(int n){
        System.out.println(n%2==0?"Even":"Odd");
    }
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        check(sc.nextInt());
    }
}

3.Question:

A person is eligible to vote if his/her age is greater than or equal to 18. Define a method to find out if he/she is eligible to vote.

Program:

import java.util.*;
public class Main{
    static void vote(int age){
        System.out.println(age>=18?"Eligible":"Not Eligible");
    }
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        vote(sc.nextInt());
    }
}

4.Question:

Write a program to print the sum of two numbers entered by user by defining your own method.

Program:

import java.util.*;
public class Main{
    static void sum(int a,int b){
        System.out.println(a+b);
    }
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        sum(sc.nextInt(),sc.nextInt());
    }
}

5.Question:

Define a method that returns the product of two numbers entered by user.

Program:

import java.util.*;
public class Main{
    static int product(int a,int b){
        return a*b;
    }
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        System.out.println(product(sc.nextInt(),sc.nextInt()));
    }
}

6.Question:

Write a program to print the circumference and area of a circle of radius entered by user by defining your own method.

Program:

import java.util.*;
public class Main{
    static void circle(double r){
        System.out.println("Area = "+3.14*r*r);
        System.out.println("Circumference = "+2*3.14*r);
    }
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        circle(sc.nextDouble());
    }
}

7.Question;

Define a method to find out if a number is prime or not.

Program:

import java.util.*;
public class Main{
    static void prime(int n){
        int c=0;
        for(int i=1;i<=n;i++)
            if(n%i==0) c++;
        System.out.println(c==2?"Prime":"Not Prime");
    }
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        prime(sc.nextInt());
    }
}

8.Question:

Write a program that will ask the user to enter his/her marks (out of 100). Define a method that will display grades according to the marks entered as below:

Marks        Grade 
91-100         AA 
81-90          AB 
71-80          BB 
61-70          BC 
51-60          CD 
41-50          DD 
<=40          Fail 

Program:

import java.util.*;
public class Main{
    static void grade(int m){
        if(m>=91) System.out.println("AA");
        else if(m>=81) System.out.println("AB");
        else if(m>=71) System.out.println("BB");
        else if(m>=61) System.out.println("BC");
        else if(m>=51) System.out.println("CD");
        else if(m>=41) System.out.println("DD");
        else System.out.println("Fail");
    }
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        grade(sc.nextInt());
    }
}

9.Question:

Write a program to print the factorial of a number by defining a method named 'Factorial'. Factorial of any number n is represented by n! and is equal to 1 * 2 * 3 * .... * (n-1) *n. E.g.-
4! = 1 * 2 * 3 * 4 = 24 
3! = 3 * 2 * 1 = 6 
2! = 2 * 1 = 2 
Also, 
1! = 1 
0! = 1

Program:

import java.util.*;
public class Main{
    static int Factorial(int n){
        int f=1;
        for(int i=1;i<=n;i++) f*=i;
        return f;
    }
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        System.out.println(Factorial(sc.nextInt()));
    }
}

10.Question:

Write a function to find if a number is a palindrome or not. Take number as parameter.

Program:

import java.util.*;
public class Main{
    static void palindrome(int n){
        int t=n,r=0;
        while(n>0){
            r=r*10+n%10;
            n/=10;
        }
        System.out.println(t==r?"Palindrome":"Not Palindrome");
    }
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        palindrome(sc.nextInt());
    }
}

11.Question:

Convert the programs in flow of program, first java, conditionals & loops assignments into functions.

Program:

import java.util.*;
public class Main{
    static void hello(){
        System.out.println("Hello World");
    }
    public static void main(String[] args){
        hello();
    }
}

12.Question:

Write a function to check if a given triplet is a Pythagorean triplet or not. (A Pythagorean triplet is when the sum of the square of two numbers is equal to the square of the third number).

Program:

import java.util.*;
public class Main{
    static void check(int a,int b,int c){
        if(a*a+b*b==c*c||a*a+c*c==b*b||b*b+c*c==a*a)
            System.out.println("Yes");
        else
            System.out.println("No");
    }
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        check(sc.nextInt(),sc.nextInt(),sc.nextInt());
    }
}
13.Question:

Write a function that returns all prime numbers between two given numbers.

Program:

import java.util.*;
public class Main{
    static void prime(int a,int b){
        for(int i=a;i<=b;i++){
            int c=0;
            for(int j=1;j<=i;j++)
                if(i%j==0)c++;
            if(c==2)
                System.out.print(i+" ");
        }
    }
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        prime(sc.nextInt(),sc.nextInt());
    }
}

14.Question:

Write a function that returns the sum of first n natural numbers.

Program:

import java.util.*;
public class Main{
    static int sum(int n){
        return n*(n+1)/2;
    }
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        System.out.println(sum(sc.nextInt()));
    }
}
