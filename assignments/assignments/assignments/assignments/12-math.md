1.Question:

Roman to Integer.

Program:

import java.util.*;

public class Solution {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String s = sc.next();
        int ans = 0;

        for (int i = 0; i < s.length(); i++) {
            int a = "IVXLCDM".indexOf(s.charAt(i));
            int v[] = {1,5,10,50,100,500,1000};
            if (i < s.length()-1 && v[a] < v["IVXLCDM".indexOf(s.charAt(i+1))])
                ans -= v[a];
            else
                ans += v[a];
        }
        System.out.println(ans);
    }
}

2.Question:

Happy Number.

Program:

import java.util.*;

public class Solution {
    static int sum(int n){
        int s=0;
        while(n>0){
            int d=n%10;
            s+=d*d;
            n/=10;
        }
        return s;
    }

    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();

        while(n!=1 && n!=4)
            n=sum(n);

        System.out.println(n==1);
    }
}


3.Question:

Armstrong Numbers

Program:

import java.util.*;

public class Solution {
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt(),t=n,s=0;

        while(t>0){
            int d=t%10;
            s+=d*d*d;
            t/=10;
        }

        System.out.println(s==n);
    }
}

4.Question:

Power of Four

Program:

import java.util.*;

public class Solution{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();

        while(n>1 && n%4==0)
            n/=4;

        System.out.println(n==1);
    }
}

5.Question:

Factorial

Program:

import java.util.*;

public class Solution{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        long f=1;

        for(int i=1;i<=n;i++)
            f*=i;

        System.out.println(f);
    }
}

6.Question:

Excel Sheet Column Title

Program:

import java.util.*;

public class Solution{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        String s="";

        while(n>0){
            n--;
            s=(char)('A'+n%26)+s;
            n/=26;
        }

        System.out.println(s);
    }
}

7.Question:

Maximum Product of Three Numbers

Program:

import java.util.*;

public class Solution{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        int a[]=new int[n];

        for(int i=0;i<n;i++)
            a[i]=sc.nextInt();

        Arrays.sort(a);

        System.out.println(Math.max(a[0]*a[1]*a[n-1],a[n-1]*a[n-2]*a[n-3]));
    }
}

8.Question:

Climbing Stairs

Program:

import java.util.*;

public class Solution{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();

        int a=1,b=1;
        for(int i=0;i<n;i++){
            int c=a+b;
            a=b;
            b=c;
        }

        System.out.println(a);
    }
}

9.Question:

Self Dividing Numbers

Program:

import java.util.*;

public class Solution{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        int l=sc.nextInt(),r=sc.nextInt();

        for(int i=l;i<=r;i++){
            int t=i;
            boolean ok=true;

            while(t>0){
                int d=t%10;
                if(d==0||i%d!=0){
                    ok=false;
                    break;
                }
                t/=10;
            }

            if(ok)
                System.out.print(i+" ");
        }
    }
}

10.Question:

Add Binary

Program:

import java.util.*;

public class Solution{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        String a=sc.next(),b=sc.next();

        System.out.println(Integer.toBinaryString(
                Integer.parseInt(a,2)+Integer.parseInt(b,2)));
    }
}

11.Question:

Power of Two

Program:

import java.util.*;

public class Solution{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();

        while(n>1 && n%2==0)
            n/=2;

        System.out.println(n==1);
    }
}

