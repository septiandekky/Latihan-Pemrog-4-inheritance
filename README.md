# Latihan-Pemrog-4-inheritance

package latihan;

public class Latihan {

    public static void main(String[] args) {
        Mobil mobil1 = new Mobil();
        mobil1.aa();
        mobil1.bergerak();
        mobil1.mengerem();
        mobil1.berjalanMundur();
        
        Pesawat pesawat1 = new Pesawat();
        pesawat1.ss();
        pesawat1.mengerem();
        pesawat1.terbang();
    }
}

package latihan;

public class Kendaraan {
    private int tanggalProduksi;
    
    public Kendaraan (){
        
    }
    public void bergerak(){
        System.out.println("Kendaraan dapat bergerak");
    }
    public void mengerem(){
        System.out.println("Kendaraan dapat mengerem");
    }
}

package latihan;

public class Mobil extends Kendaraan {
    public Mobil(){
        
    }
    public void aa(){
        System.out.println("Mobil");
    }
    public void berjalanMundur(){
        System.out.println("Mobil dapat berjalan mundur");
    } 
}
package latihan;

public class Pesawat extends Kendaraan {
    public Pesawat(){
        
    }
    public void ss(){
        System.out.println("Pesawat");
    }
    public void terbang(){
        System.out.println("Pesawat dapat terbang");
    }
}
