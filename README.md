# ebobEkokWhileLoop
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        int n1, n2;

        Scanner input = new Scanner(System.in);
        System.out.println("1. sayiyi giriniz : ");
        n1 = input.nextInt();

        System.out.println("2. sayiyi giriniz : ");
        n2 = input.nextInt();

        System.out.println("*******EBOB Hesabi**********");
        int ebob = 1;
        int i = n1;
        while (i >= 1) {
            if (n1 % i == 0 && n2 % i == 0) {
                ebob = i;
                System.out.println(n1 + " ve " + n2 + " ebob " + "degeri : " + ebob);
                break;
            } else {
                i--;
            }
        }

        System.out.println("*******EKOK Hesabi**********");
        int ekok;

        int k = n2;


        while (n2 <= (n1 * n2)) {
            if (k % n1 == 0 && k % n2 == 0) {
                ekok = k;
                System.out.println(n1 + " ve " + n2 + " ekok " + "degeri : " + ekok);
                break;
            } else {
                k++;
            }
        }


    }
}
