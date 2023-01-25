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
public class donguler {
public static void main(String[] args) {
    
    int a[][]={{1,2,3,4},
               {6,4,23,12},
               {45,37,81,86}
              };
    
           for(int i=0;i<a.length;i++){ 
               int toplam=0;
               for(int j=0;j<a[i].length;j++){
                  toplam+=a[i][j]; 
               }System.out.println(i+". satırın toplamı:"+toplam);
               
           }
      
     
          
}
      }
````
### 10 elemanlı string dizisi içinde en uzun stringi ve uzunluğunu bulan program
````
public class donguler {
public static void main(String[] args) {
    
    String a[]={"Ali","Mustafa","Fatih","Furkan","Ahmet","Serdar","Cemal","Esra","Evindar","Ozan"};
           int en_uzun=0;
           String deger=null;
           
           for(int i=0;i<a.length;i++){
               if(a[i].length()>en_uzun){
                   en_uzun=a[i].length();
                   deger=a[i];
                   
               }
           }System.out.println("Bu dizideki en uzun string:"+deger+" dir ve uzunlugu "+en_uzun+" dir.");
     
          
}
      }
    
````
### Vize notu girilmiş olan bir a dizisi ve final notu girilmiş bir b dizisinde geçen ve kalan toplam öğrenci sayısını veren program.
````
import java.util.Scanner;

public class donguler {
public static void main(String[] args) {
    
    int a[]={23,45,65,78,54,60,87};
    int b[]={65,23,65,12,98,45,35};
      
         int gecen_sayisi=0;
         int kalan_sayisi=0;
         for(int i=0;i<a.length;i++){
             if(b[i]<50){
                 kalan_sayisi++;
             }else{
                double c=a[i]*0.4+b[i]*0.6;
                if(c>=50){
                    gecen_sayisi++;
                }
             }   
         }System.out.println("Bu öğrencilerden "+gecen_sayisi+" kadar öğrenci geçti ve "
                                 +kalan_sayisi+" kadar öğrencide kaldı.");
      
````
### Girilmiş olan bir dizideki asal sayıları bulup ekrana yazan ve kaç adet olduğunu yazan programı yazınız.
````
public class donguler {
public static void main(String[] args) {
    
    int a[]={23,45,65,78,54,60,87,43,19,7,5};
    int sayac=0;
    int asal_sayac=0;
          for(int i=0;i<a.length;i++){
              sayac=0;
              for(int j=2;j<a[i];j++){
                 
                  if(a[i]%j==0){
                      sayac++;
                      
                  }
                    }if(sayac==0){
                      System.out.println(a[i]+" asal bir sayıdır.");
                      asal_sayac++;
                  }
              }
         System.out.println("Toplam "+asal_sayac+" tane asal sayı vardır");
   }
      
  }
````
