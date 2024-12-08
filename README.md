# a-different-pattern
import java.util.Scanner;

public class pattern {
    public pattern() {
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the no. n : ");
        int n = sc.nextInt();
        rec(n, n, true);
    }

    public static void rec(int n, int m, boolean flag) {
        System.out.println("" + m + " ");
        if (flag || n != m) {
            if (flag) {
                if (m - 5 > 0) {
                    rec(n, m - 5, true);
                } else {
                    rec(n, m - 5, false);
                }
            } else {
                rec(n, m + 5, false);
            }

        }
    }
}
