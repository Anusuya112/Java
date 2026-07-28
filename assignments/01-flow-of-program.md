Question:
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
