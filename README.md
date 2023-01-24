# Java-dizi
----
### 5 indisli tanımlanan bir diziye klavyeden girilen sayıları atama ve sonrasında ekrana yazdıran programı yazınız.
````
import java.util.Scanner;

public class donguler {
public static void main(String[] args) {
     int a[]=new int[5];
      Scanner m=new Scanner(System.in);
      System.out.println("Lütfen 5 adet sayı giriniz:");
           for(int i=0;i<a.length;i++){
               int b=m.nextInt();
               a[i]=b;
           }
           for(int i=0;i<a.length;i++){
               System.out.println(a[i]);
           }

}
      }
````
### Klavyeden girilen 20 indisli bir dizide en  büyük sayıyı bulan ve indisini yazan programı yazınız.
````
import java.util.Scanner;

public class donguler {
public static void main(String[] args) {
     int a[]=new int[20];
      Scanner m=new Scanner(System.in);
      System.out.println("Lütfen 20 adet sayı giriniz:");
      int  enb=0;
      int deger=0;
           for(int i=0;i<a.length;i++){
               int b=m.nextInt();
               a[i]=b;
           }
           for(int i=0;i<a.length;i++){
              if(enb<a[i]){
                 enb=a[i];
                 deger=i;
              }
           }System.out.println("En büyük sayı:"+enb+" ve "+deger+". indistedir.");

}
      }
````
### Klavyeden girilen 10 indisli bir dizinin toplamını ve ortalamasını bulan programı yapınız.
````
import java.util.Scanner;

public class donguler {
public static void main(String[] args) {
     int a[]=new int[10];
      Scanner m=new Scanner(System.in);
      System.out.println("Lütfen 10 adet sayı giriniz:");
      int  toplam=0;
      int d=0;
           for(int i=0;i<a.length;i++){
               int b=m.nextInt();
               a[i]=b;
           }
           for(int i=0;i<a.length;i++){
              toplam+=a[i];
           }double ortalama=toplam/10.0;
           System.out.println("Klavyeden giriilen sayıların toplamı:"+toplam+" ve ortalamlası:"+ortalama);
}
      }
````
### İki boyutlu sayısal  bir dizide satırların toplamını veren  programı yazınız.
````
