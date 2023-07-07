PENJELASAN TENTANG Teori 230623


package Melida230623


public abstract class MakhlukHidup {

    public void bernafas(){
        System.out.println("Bernafas");
    }
    public abstract void jalan();
}

MakhlukHidup adalah sebuah kelas abstrak, ditandai dengan kata kunci abstract sebelum kata kunci class. Kelas abstrak tidak dapat diinstansiasi langsung, tetapi digunakan sebagai kerangka untuk kelas-kelas turunannya.

Terdapat sebuah metode bernama bernafas() yang tidak dinyatakan sebagai abstrak. Metode ini memiliki implementasi yang telah ditentukan, yaitu mencetak "Bernafas" ke konsol.

Terdapat sebuah metode abstrak bernama jalan(). Metode ini tidak memiliki implementasi di dalam kelas MakhlukHidup dan dinyatakan sebagai abstrak dengan tidak memiliki blok tubuh ({}). Metode abstrak harus didefinisikan ulang (override) di kelas turunannya.

Metode bernafas() adalah metode biasa yang dapat diwarisi oleh kelas turunan, sedangkan metode jalan() adalah metode abstrak yang harus diimplementasikan oleh kelas turunan.

Kelas abstrak digunakan sebagai kerangka untuk kelas-kelas turunannya. Kelas turunan yang mewarisi MakhlukHidup harus mengimplementasikan metode abstrak jalan() dengan menyediakan implementasi sesuai kebutuhan.


public class Manusia extends MakhlukHidup {

    public void jalan(){
        System.out.println("Berjalan Manusia");
    }
    
    public static void main(String[] args) {
        Manusia m = new Manusia();
        m.bernafas();
        m.jalan();
    }
}


Manusia adalah sebuah kelas yang meng-extend kelas MakhlukHidup, menunjukkan bahwa Manusia merupakan turunan dari MakhlukHidup.

Terdapat metode jalan() yang diimplementasikan dari kelas abstrak MakhlukHidup. Dalam implementasi ini, metode mencetak "Berjalan Manusia" ke konsol.

Metode main() adalah metode yang akan dijalankan saat program dimulai. Di dalam metode ini, objek Manusia dengan nama m dibuat.

Metode bernafas() dari kelas MakhlukHidup diwarisi oleh kelas Manusia, sehingga metode ini dapat dipanggil pada objek m.

Metode jalan() dari kelas Manusia dipanggil pada objek m, sehingga metode ini akan mencetak "Berjalan Manusia" ke konsol.

Ketika program dijalankan, outputnya akan mencetak "Bernafas" (dari metode bernafas()) dan "Berjalan Manusia" (dari metode jalan()) ke konsol.


public class PersegiPanjang implements Relation{

    private float panjang;
    private float lebar;

    public PersegiPanjang() {
    }

    public PersegiPanjang(int panjang, int lebar) {
    
        this.panjang = panjang;
        this.lebar = lebar;
    }
    
    public float getLuas(){
        return panjang * lebar;
    }
    
    public float getKeliling(){
        return (2*panjang)+(2*lebar);
    }

    @Override
    public boolean isGreater(Object a, Object b) {
        float luas_a = ((PersegiPanjang) a).getLuas();
        float luas_b = ((PersegiPanjang) b).getLuas();
        return luas_a > luas_b;
    }

    @Override
    public boolean isLess(Object a, Object b) {
        float luas_a = ((PersegiPanjang) a).getLuas();
        float luas_b = ((PersegiPanjang) b).getLuas();
        return luas_a < luas_b;
    }

    @Override
    public boolean isEqual(Object a, Object b) {
        float luas_a = ((PersegiPanjang) a).getLuas();
        float luas_b = ((PersegiPanjang) b).getLuas();
        return luas_a == luas_b;
    }
    
    public static void main(String[] args) {
        PersegiPanjang p1 = new PersegiPanjang(5, 2);
        PersegiPanjang p2 = new PersegiPanjang(4, 3);
        Relation r = new PersegiPanjang();
        System.out.println("Luas p1 > luas p2" + r.isGreater(p1, p2) );
        System.out.println("Luas p1 < luas p2" + r.isLess(p1, p2) );
    }
    
}


PersegiPanjang adalah sebuah kelas yang mengimplementasikan antarmuka Relation.

Terdapat dua atribut privat yaitu panjang dan lebar yang merepresentasikan panjang dan lebar persegi panjang.

Terdapat beberapa konstruktor, termasuk konstruktor default dan konstruktor dengan parameter panjang dan lebar.

Metode getLuas() digunakan untuk menghitung luas persegi panjang dengan mengalikan panjang dengan lebar.

Metode getKeliling() digunakan untuk menghitung keliling persegi panjang.

Metode isGreater(Object a, Object b), isLess(Object a, Object b), dan isEqual(Object a, Object b) diimplementasikan dari antarmuka Relation. Metode-metode ini membandingkan luas persegi panjang a dan b dengan menggunakan metode getLuas().

Di dalam metode main(), dua objek PersegiPanjang dengan panjang dan lebar yang berbeda dibuat. Objek r dari tipe Relation juga dibuat dengan menggunakan polimorfisme.

Metode isGreater() dan isLess() dari objek r dipanggil dengan mengirimkan objek p1 dan p2 sebagai argumen. Hasil perbandingan luas persegi panjang dicetak ke konsol.

Ketika program dijalankan, outputnya akan mencetak hasil perbandingan luas persegi panjang antara p1 dan p2 ke konsol.


public interface Relation {

    public boolean isGreater( Object a, Object b); 
    public boolean isLess( Object a, Object b); 
    public boolean isEqual( Object a, Object b);
    
}


Antarmuka Relation mendefinisikan tiga metode yang harus diimplementasikan oleh kelas-kelas yang mengimplementasikan antarmuka ini, yaitu isGreater, isLess, dan isEqual.

Metode isGreater memiliki dua parameter bertipe Object (objek). Metode ini bertugas membandingkan dua objek dan mengembalikan nilai boolean yang menyatakan apakah objek pertama lebih besar daripada objek kedua.

Metode isLess juga memiliki dua parameter bertipe Object. Metode ini bertugas membandingkan dua objek dan mengembalikan nilai boolean yang menyatakan apakah objek pertama lebih kecil daripada objek kedua.

Metode isEqual juga memiliki dua parameter bertipe Object. Metode ini bertugas membandingkan dua objek dan mengembalikan nilai boolean yang menyatakan apakah objek pertama sama dengan objek kedua.

Antarmuka Relation berfungsi sebagai kontrak yang menyatakan bahwa kelas-kelas yang mengimplementasikan antarmuka ini harus menyediakan implementasi untuk metode-metode tersebut. Dengan mengimplementasikan antarmuka Relation, kelas-kelas tersebut dapat membandingkan objek-objek dan menentukan hubungan relasional di antara mereka.



