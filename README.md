# Kombinasyon-Hesaplayan-Program
---
Bu bir [patika.dev](www.patika.dev) projesidir.
```
import java.util.Scanner;
public class kombinasyon {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        int i,r,n,f, sonuc, fn=1, fr=1,ff=1;

        System.out.print("Kümenin elaman sayısını giriniz: ");
        n= input.nextInt();
        System.out.print("Kombinasyonların kaç elemanlı olacağını giriniz: ");
        r=input.nextInt();
        if(r>=n){
            System.out.println("Hatalı giriş yaptınız.");
            return;
        }
        f=n-r;
        for (i=1; i<=n; i++){
            fn = fn*i;
        }
        for (i=1; i<=r; i++){
            fr = fr*i;
        }
        for (i=1;i<=f;i++){
            ff*=i;
        }
        sonuc= fn / (fr * ff);
        System.out.print("Kombinasyon:"+sonuc);

    }
}
```
