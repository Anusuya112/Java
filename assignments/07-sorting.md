1.Question:

Merge Sorted Array.

Program:

import java.util.*;

class Main {

    public static void main(String[] args) {
    
        int[] a={1,2,3,0,0,0}, b={2,5,6};
        
        for(int i=0;i<3;i++) a[i+3]=b[i];
        Arrays.sort(a);
        
        System.out.println(Arrays.toString(a));
    }
}

Output:

[1, 2, 2, 3, 5, 6]

=== Code Execution Successful ===

2.Question:

Majority Element

Program:

class Main {

    public static void main(String[] args) {
        int[] a={2,2,1,1,1,2,2};
        int ans=0,count=0;

        for(int x:a){
            if(count==0) ans=x;
            if(x==ans) count++;
            else count--;
        }

        System.out.println(ans);
    }
}

Output:

2

=== Code Execution Successful ===

3.Question:

Contains Duplicate

Program:

import java.util.*;

class Main {

    public static void main(String[] args) {
        int[] a={1,2,3,1};
        
        HashSet<Integer> s=new HashSet<>();
        
        for(int x:a)
        
            if(!s.add(x)){System.out.println(true);return;}
        System.out.println(false);
    }
}

Output:

true

=== Code Execution Successful ===

4.Question:

Missing Number

Program:

class Main {

    public static void main(String[] args) {
        int[] a = {3,0,1};
        int sum = a.length * (a.length + 1) / 2;

        for (int x : a)
            sum -= x;

        System.out.println(sum);
    }
}

Output:

2

=== Code Execution Successful ===

5.Question:

Intersection of Two Arrays

Program:

import java.util.*;

class Main {
    public static void main(String[] args) {
        int[] a = {4,9,5};
        int[] b = {9,4,9,8,4};

        HashSet<Integer> s = new HashSet<>();

        for (int x : a)
            s.add(x);

        for (int x : b)
            if (s.remove(x))
                System.out.print(x + " ");
    }
}

Output:

9 4 

=== Code Execution Successful ===

