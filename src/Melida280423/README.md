 PENJELASA LATIHAN MODUL 8
 
 
 public class Latihan8_soal1 {
 
     public static void main ( String[] args){
     
        for(int i=0; i<=4; i++)
        System.out.println("\n" +args[i]);
         
    }
}


Kode di atas adalah program Java yang mencetak nilai yang diinputkan ke dalam array args. Program tersebut memiliki satu method, yaitu main, yang berisi perulangan for dengan penghitung i yang dimulai dari 0 dan berakhir pada 4. Setiap kali perulangan dijalankan, program akan mencetak elemen array args dengan indeks i dan mengakhiri baris dengan memanggil System.out.println(). Dalam hal ini, karakter \n digunakan untuk membuat baris baru sebelum mencetak nilai dari elemen array.

Sebagai contoh, jika kita menjalankan program tersebut dengan argumen "hello", "world", "java", "programming", "is", maka program akan mencetak nilai argumen tersebut dalam baris baru, yaitu:

hello
world
java
programming
is


Namun, perlu diingat bahwa program akan menghasilkan error jika kita tidak memberikan cukup argumen saat menjalankan program atau jika memberikan terlalu banyak argumen. Sehingga sebaiknya memperhatikan jumlah argumen yang diberikan saat menjalankan program.
