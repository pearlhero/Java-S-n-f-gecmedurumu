# Java-S-n-f-gecmedurumu
Java-Sınıfıgecmedurumu

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        int mat, fizik, turkce, kimya, muzik;

        Scanner input = new Scanner(System.in);

        System.out.print("Matematik notunuz: ");
        mat = input.nextInt();
        if ((mat < 0) || (mat > 100)) {
            System.out.println("Hatalı not girdiniz!Lütfen yeniden deneyiniz.");
        } else {
            mat = mat;
        }

        System.out.print("Fizik notunuz: ");
        fizik = input.nextInt();
        if ((fizik < 0) || (fizik > 100)) {
            System.out.println("Hatalı not girdiniz!Lütfen yeniden deneyiniz.");
        } else {
            fizik = fizik;

            System.out.print("Türkçe notunuz: ");
            turkce = input.nextInt();
            if ((turkce < 0) || (turkce > 100)) {
                System.out.println("Hatalı not girdiniz!Lütfen yeniden deneyiniz.");
            } else {
                turkce = turkce;

                System.out.print("Kimya notunuz: ");
                kimya = input.nextInt();
                if ((kimya < 0) || (kimya > 100)) {
                    System.out.println("Hatalı not girdiniz!Lütfen yeniden deneyiniz.");
                } else {
                    kimya = kimya;

                    System.out.print("Müzik notunuz: ");
                    muzik = input.nextInt();
                    if ((muzik < 0) || (muzik > 100)) {
                        System.out.println("Hatalı not girdiniz!Lütfen yeniden deneyiniz.");
                    } else {
                        muzik = muzik;
                    }
                    double avarage = ((mat + fizik + turkce + kimya + muzik) / 5);
                    if (avarage <= 55) {
                        System.out.println("Sınıfta kaldınız.Seneye tekrar görüşürüz.");
                    } else {
                        System.out.println("Tebrikler! Sınıfı geçtiniz!");
                    }
                    System.out.println("Ortalamanız : " + avarage);
                }

            }
        }
    }
}
