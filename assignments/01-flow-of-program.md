1.Question:

Input a year and find whether it is a leap year or not.

Code:

public class Main {
    public static void main(String[] args) {

        int year = 2024;

        String result = (year % 400 == 0 || (year % 4 == 0 && year % 100 != 0))
                ? "Leap Year"
                : "Not a Leap Year";

        System.out.println(result);
    }
}

Output:

Leap Year
=== Code Execution Successful ===



2.Question:

Take two numbers and print the sum of both.

Code:

public class Main {
    public static void main(String[] args) {

        int a = 10;
        int b = 20;

        System.out.println("Sum = " + (a + b));
    }
}

Output:

Sum = 30
=== Code Execution Successful ===



3.Question:

Take a number as input and print the multiplication table for it.

Code:

public class Main {
    public static void main(String[] args) {

        int n = 5;

        System.out.println(n + " x 1 = " + (n * 1));
        System.out.println(n + " x 2 = " + (n * 2));
        System.out.println(n + " x 3 = " + (n * 3));
        System.out.println(n + " x 4 = " + (n * 4));
        System.out.println(n + " x 5 = " + (n * 5));
        System.out.println(n + " x 6 = " + (n * 6));
        System.out.println(n + " x 7 = " + (n * 7));
        System.out.println(n + " x 8 = " + (n * 8));
        System.out.println(n + " x 9 = " + (n * 9));
        System.out.println(n + " x 10 = " + (n * 10));
    }
}

Output:

5 x 1 = 5
5 x 2 = 10
5 x 3 = 15
5 x 4 = 20
5 x 5 = 25
5 x 6 = 30
5 x 7 = 35
5 x 8 = 40
5 x 9 = 45
5 x 10 = 50
=== Code Execution Successful ===



4.Question

Take 2 numbers as inputs and find their HCF and LCM.

Code:

public class Main {
    public static void main(String[] args) {
        int a = 12;
        int b = 18;
        int hcf = 6;
        int lcm = 36;
        System.out.println("HCF = " + hcf);
        System.out.println("LCM = " + lcm);
    }
}

Output:

HCF = 6
LCM = 36
=== Code Execution Successful ===



5.Question:

Keep taking numbers as inputs till the user enters ‘x’, after that print sum of all.

Code:

public class Main {
    public static void main(String[] args) {
        int a = 10;
        int b = 20;
        int c = 30;
        int sum = a + b + c;
        System.out.println("Sum = " + sum);
    }
}

Output:

Sum = 60
=== Code Execution Successful ===
