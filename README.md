import java.util.Scanner;

public class Main1 {


    public static void main() {

    
     //Java ile gidilen mesafeye (KM) göre taksimetre tutarını ekrana yazdıran programı yazın.
        //
        //Taksimetre KM başına 2.20 TL tutmaktadır.
        //Minimum ödenecek tutar 20 TL'dir. 20 TL altında ki ücretlerde yine 20 TL alınacaktır.
        //Taksimetre açılış ücreti 10 TL'dir.

        double km,kmbasi=2.20,toplam,baslangic=10;
        Scanner input = new Scanner(System.in);
        System.out.print("Gitmek istediğiniz km tutarını giriniz:  ");
        km = input.nextDouble();
        
        toplam=km*kmbasi;
        toplam+=baslangic;

        toplam= (toplam<20) ? 20 : toplam;
        System.out.println("toplam tutar: "+toplam);

    }
}
