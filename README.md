# ucgen
import java.util.Scanner;
public class main2 {
    public static void main(String[] args) {
        // değişkenleri oluşturalım
        int a, b, c;
        double cevre, alan, u;

        // kullanıcıdan verileri alalım
        Scanner girdi = new Scanner(System.in);
        System.out.println("1. Kenarı Giriniz: ");
        a = girdi.nextInt();
        System.out.println("2. Kenarı Giriniz: ");
        b = girdi.nextInt();
        System.out.println("3. Kenarı Giriniz: ");
        c = girdi.nextInt();

        // çevrenin formülü
        cevre= (a+b+c);
        System.out.println("Çevre: " + cevre);

       // Üç𝑔𝑒𝑛𝑖𝑛 ç𝑒𝑣𝑟𝑒𝑠𝑖 = 2𝑢 ise 𝑢 = (a+b+c) / 2

        u = (a+b+c) / 2;

        // Heron formulü = Alan*Alan = 𝑢*(𝑢 − 𝑎)*(𝑢 − 𝑏)*(𝑢 − 𝑐)

        alan = Math.sqrt(u * (u - a) * (u - b) * (u - c));
        System.out.println("Ucgenin Alani :" + alan);


    }
}
