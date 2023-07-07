PENJELASAN MODUL 12


package Melida070723;

/**
 *
 * @author Melida Sari

public class Exception {

    public static void main(String[] args) {
        try {
            for (int i = 0; true; i++) {
                System.out.println("args[" + i + "]=" + args[i]);
            }
        } catch (ArrayIndexOutOfBoundsException e) {
            System.out.println("Exception caught:");
            System.out.println(e);
        } finally {
            System.out.println("Quitting...");
        }
    }  
}


Terdapat deklarasi kelas Exception. Nama kelas ini sebaiknya diubah, karena "Exception" adalah nama yang sudah ada dalam bahasa Java untuk kelas-kelas yang terkait dengan penanganan eksepsi. Misalnya, ArrayIndexOutOfBoundsException yang digunakan dalam kode ini adalah salah satu contoh kelas exception bawaan Java.

Di dalam kelas Exception, terdapat method main yang merupakan method utama yang akan dieksekusi saat program dijalankan.

Pada blok try, terdapat perulangan for yang berjalan tanpa batas (true). Di dalam perulangan, kode mencoba mencetak elemen-elemen dari array args dengan menggunakan indeks i. Array args merupakan argumen yang diberikan saat menjalankan program Java dari baris perintah. Namun, karena tidak ada batasan pada perulangan for, pada suatu titik, indeks i akan melampaui panjang array args, sehingga ArrayIndexOutOfBoundsException akan dilempar.

Blok catch digunakan untuk menangkap dan menangani exception yang terjadi. Di sini, exception yang ditangkap adalah ArrayIndexOutOfBoundsException. Ketika exception terjadi, pesan "Exception caught:" akan dicetak, diikuti dengan mencetak informasi tentang exception tersebut (e). Informasi exception berupa pesan yang menjelaskan kesalahan dan traceback.

Blok finally adalah blok yang akan dieksekusi setelah blok try selesai dieksekusi, baik dengan atau tanpa exception. Pada kode ini, pesan "Quitting..." akan dicetak setelah mencetak informasi exception (jika ada) atau setelah perulangan selesai dieksekusi tanpa exception.

Keseluruhan kode ini menunjukkan contoh penggunaan exception handling untuk menangani ArrayIndexOutOfBoundsException yang mungkin terjadi saat mencoba mengakses elemen array di luar batas indeks yang valid.


package Melida070723;

/**
 *
 * @author Melida Sari

public class TestExceptions {

    public static void main(String[] args) {
        try {
            for (int i = 0; true; i++) {
                System.out.println("args[" + i + "]=" + args[i]);
            }
        } catch (ArrayIndexOutOfBoundsException i) {
            System.out.println("Exception caught:");
            System.out.println(i);
            System.out.println("Quitting...");
        }
    }
}


Terdapat deklarasi kelas TestExceptions. Nama kelas ini sesuai dengan nama file yang menyimpannya (TestExceptions.java). Kelas ini berfungsi sebagai tempat untuk mengeksekusi kode.

Di dalam kelas TestExceptions, terdapat method main yang merupakan method utama yang akan dieksekusi saat program dijalankan.

Pada blok try, terdapat perulangan for yang berjalan tanpa batas (true). Di dalam perulangan, kode mencoba mencetak elemen-elemen dari array args dengan menggunakan indeks i. Array args merupakan argumen yang diberikan saat menjalankan program Java dari baris perintah. Namun, karena tidak ada batasan pada perulangan for, pada suatu titik, indeks i akan melampaui panjang array args, sehingga ArrayIndexOutOfBoundsException akan dilempar.

Blok catch digunakan untuk menangkap dan menangani exception yang terjadi. Pada kode ini, exception yang ditangkap diberi nama i (bisa diganti nama yang lebih deskriptif). Ketika exception terjadi, pesan "Exception caught:" akan dicetak, diikuti dengan mencetak informasi tentang exception tersebut (i). Informasi exception berupa pesan yang menjelaskan kesalahan dan traceback.

Setelah mencetak informasi exception, pesan "Quitting..." akan dicetak. Pada kode ini, pesan ini langsung dicetak setelah mencetak informasi exception, tanpa menunggu perulangan selesai dieksekusi.

Keseluruhan kode ini menunjukkan contoh penggunaan exception handling untuk menangani ArrayIndexOutOfBoundsException yang mungkin terjadi saat mencoba mengakses elemen array di luar batas indeks yang valid.


package Melida070723;

/**
 *
 * @author Lenovo

public class HelloWorld {

    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
}


Terdapat deklarasi kelas HelloWorld. Nama kelas ini sesuai dengan nama file yang menyimpannya (HelloWorld.java). Kelas ini berfungsi sebagai tempat untuk mengeksekusi kode.

Di dalam kelas HelloWorld, terdapat method main yang merupakan method utama yang akan dieksekusi saat program dijalankan.

Pada baris ke-6, terdapat perintah System.out.println("Hello World!");. Perintah ini digunakan untuk mencetak pesan "Hello World!" ke konsol. System.out adalah objek yang mewakili output standar, dan println adalah metode untuk mencetak teks diikuti dengan baris baru.

Keseluruhan kode ini adalah program Java yang sederhana yang mencetak pesan "Hello World!" ke konsol. Ini adalah program umum yang sering digunakan sebagai contoh atau latihan awal dalam mempelajari bahasa pemrograman Java.

