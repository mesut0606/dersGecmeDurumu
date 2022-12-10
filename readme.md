Ders Geçme Notu

Ders notu 1-100 arasında değer almaz ise o notu ortalamaya dahil etmiyor

import java.util.Scanner;

public class Main {
public static void main(String[] args) {
int mat, fizik, türkce, kimya, muzik;
int toplamnot = 0, toplamders = 0;


        Scanner input = new Scanner(System.in);

        System.out.println("Matematik notunu giriniz:");
        mat = input.nextInt();

        if ((mat >= 0) && (mat <= 100)) {
            toplamnot += mat;
            toplamders++;
        }

        System.out.println("Fizik notunu giriniz:");
        fizik = input.nextInt();
        if ((fizik >= 0) && (fizik <= 100)) {
            toplamnot += fizik;
            toplamders++;
        }


        System.out.println("Türkçe notunu giriniz:");
        türkce = input.nextInt();
        if ((türkce >= 0) && (türkce <= 100)) {
            toplamnot += türkce;
            toplamders++;
        }

        System.out.println("Kimya notunu giriniz:");
        kimya = input.nextInt();
        if ((kimya >= 0) && (kimya <= 100)) {
            toplamnot += kimya;
            toplamders++;
        }

        System.out.println("Müzik notunu giriniz:");
        muzik = input.nextInt();
        if ((muzik >= 0) && (muzik <= 100)) {
            toplamnot += muzik;
            toplamders++;
        }

        double avarage = (toplamnot/toplamders);

        if (avarage >= 55) {
            System.out.println("Ortalama:" + avarage);
            System.out.println("Sınıfı Geçtiniz");
        } else {
            System.out.println("Ortalama:" + avarage);
            System.out.println("Sınıfta kaldınız!!!!");
        }

    }
}

