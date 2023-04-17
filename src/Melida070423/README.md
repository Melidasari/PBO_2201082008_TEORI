MODUL BAB 6
Struktur Kontrol 

fungsi import javax.swing.JOptionPane;
"javax.swing.JOptionPane" adalah kelas yang ada di Java API, yang digunakan untuk menampilkan dialog box pada aplikasi Java. Dialog box dapat digunakan untuk meminta input dari pengguna, menampilkan pesan, dan mengambil keputusan dari pengguna.

Untuk menggunakan kelas JOptionPane, perlu dilakukan import pada awal file Java, seperti contoh berikut:
import javax.swing.JOptionPane;

public class ContohDialogBox {
   public static void main(String[] args) {
      String nama = JOptionPane.showInputDialog("Masukkan nama Anda: ");
      JOptionPane.showMessageDialog(null, "Halo " + nama + "!");
   }
}
Dalam contoh di atas, kelas JOptionPane digunakan untuk menampilkan dialog box input (showInputDialog) untuk meminta pengguna untuk memasukkan nama, dan dialog box pesan (showMessageDialog) untuk menampilkan pesan yang menyapa pengguna.

/// Struktur Kontrol Keputusan 
1. Statement if
Statement-if menentukan sebuah statement (atau blok kode) yang akan dieksekusi jika 
dan hanya jika persyaratan boolean (boolean statement) bernilai true. 
"Statement if" adalah salah satu struktur kontrol pada bahasa pemrograman Java yang digunakan untuk melakukan pengujian kondisi atau ekspresi boolean. Dalam Java, if statement digunakan untuk mengevaluasi kondisi atau ekspresi boolean dan menjalankan blok kode tertentu jika kondisi tersebut benar.

Contoh penggunaan dari statement if di Java adalah sebagai berikut:
int x = 5;

if (x > 0) {
   System.out.println("x adalah bilangan positif");
}
Dalam contoh di atas, jika nilai variabel x lebih besar dari 0, maka statement "x adalah bilangan positif" akan dicetak di konsol. Namun jika nilai x kurang dari atau sama dengan 0, maka statement tersebut tidak akan dicetak.


2. Statement if-else
Statement if-else digunakan apabila kita ingin mengeksekusi sebuah statement dengan 
kondisi true dan statement yang lain dengan kondisi false. 

"Statement if-else" adalah struktur kontrol pada bahasa pemrograman Java yang digunakan untuk menguji kondisi atau ekspresi boolean dan melakukan tindakan yang berbeda tergantung pada hasil evaluasi kondisi tersebut.

Dalam Java, statement if-else menggunakan sintaks berikut:
if (kondisi) {
    // blok kode yang dijalankan jika kondisi benar
} else {
    // blok kode yang dijalankan jika kondisi salah
}
Contoh penggunaan dari statement if-else di Java adalah sebagai berikut:
int x = 5;

if (x > 0) {
   System.out.println("x adalah bilangan positif");
} else {
   System.out.println("x adalah bilangan negatif atau nol");
}
Dalam contoh di atas, jika nilai variabel x lebih besar dari 0, maka statement "x adalah bilangan positif" akan dicetak di konsol. Namun jika nilai x kurang dari atau sama dengan 0, maka statement "x adalah bilangan negatif atau nol" akan dicetak.


3. Statement if-else-if
"Statement if-else-if" adalah struktur kontrol pada bahasa pemrograman Java yang digunakan untuk mengevaluasi beberapa kondisi atau ekspresi boolean dan menjalankan tindakan yang berbeda tergantung pada hasil evaluasi kondisi tersebut.

Dalam Java, statement if-else-if menggunakan sintaks berikut:
if (kondisi1) {
    // blok kode yang dijalankan jika kondisi1 benar
} else if (kondisi2) {
    // blok kode yang dijalankan jika kondisi2 benar
} else if (kondisi3) {
    // blok kode yang dijalankan jika kondisi3 benar
} else {
    // blok kode yang dijalankan jika tidak ada kondisi yang benar
}
Contoh penggunaan dari statement if-else-if di Java adalah sebagai berikut:
int x = 5;

if (x > 0) {
   System.out.println("x adalah bilangan positif");
} else if (x < 0) {
   System.out.println("x adalah bilangan negatif");
} else {
   System.out.println("x adalah nol");
}
Dalam contoh di atas, jika nilai variabel x lebih besar dari 0, maka statement "x adalah bilangan positif" akan dicetak di konsol. Namun jika nilai x kurang dari 0, maka statement "x adalah bilangan negatif" akan dicetak. Jika nilai x adalah 0, maka statement "x adalah nol" akan dicetak.

Dalam multiple else-if blocks, blok kode yang dijalankan pertama kali adalah yang sesuai dengan kondisi pertama yang benar. Jika tidak ada kondisi yang benar, maka blok kode yang dijalankan adalah blok terakhir dalam else block.


4. Statement switch 
Cara lain untuk membuat percabangan adalah dengan menggunakan kata kunci switch. 
Dengan menggunakan switch kita bisa melakukan percabangan dengan persyaratan 
yang beragam.
"Statement switch" adalah struktur kontrol pada bahasa pemrograman Java yang digunakan untuk mengevaluasi ekspresi atau nilai dan menjalankan blok kode tertentu tergantung pada nilai tersebut.
Contoh penggunaan dari statement switch di Java adalah sebagai berikut:
int nilai = 3;

switch (nilai) {
   case 1:
      System.out.println("Nilai Anda adalah 1");
      break;
   case 2:
      System.out.println("Nilai Anda adalah 2");
      break;
   case 3:
      System.out.println("Nilai Anda adalah 3");
      break;
   default:
      System.out.println("Nilai Anda tidak sesuai");
}
Dalam contoh di atas, ekspresi nilai adalah variabel integer "nilai" yang memiliki nilai 3. Karena nilai tersebut sama dengan case ketiga dalam switch statement, maka blok kode "Nilai Anda adalah 3" akan dicetak di konsol.

Jika nilai tidak sama dengan case mana pun dalam switch statement, maka blok kode dalam default statement akan dijalankan.

Penting untuk dicatat bahwa setiap blok kode case harus diakhiri dengan break statement, untuk menghentikan switch statement setelah case yang cocok ditemukan. Jika tidak ada break statement, maka switch statement akan terus dievaluasi hingga akhir atau hingga ditemukan break statement.



///Struktur Kontrol Perulangan

1. while loop
Statement while loop adalah statement atau blok statement yang diulang-ulang sampai 
mencapai kondisi yang cocok. 
"While loop" adalah struktur pengulangan pada bahasa pemrograman Java yang digunakan untuk mengeksekusi blok kode secara berulang selama kondisi yang diberikan masih terpenuhi atau bernilai true.
Contoh penggunaan dari while loop di Java adalah sebagai berikut:
int i = 0;

while (i < 5) {
   System.out.println("Nilai i adalah " + i);
   i++;
}
Dalam contoh di atas, nilai variabel i akan dicetak di konsol selama nilai i kurang dari 5. Setiap kali blok kode dalam while loop dieksekusi, nilai i akan bertambah 1, sehingga loop akan berhenti saat nilai i mencapai 5.

Kondisi dalam while loop harus dievaluasi sebagai boolean. Jika kondisi awal bernilai false, maka blok kode dalam while loop tidak akan pernah dieksekusi. Jika kondisi selalu bernilai true, maka while loop akan berjalan secara tak terbatas, yang disebut sebagai "infinite loop". Oleh karena itu, pastikan bahwa kondisi yang diberikan akhirnya akan bernilai false setelah beberapa iterasi.


2. do-while loop 
Do-while loop mirip dengan while-loop. Statement di dalam do-while loop akan 
dieksekusi beberapa kali selama kondisi bernilai true. 
Perbedaan antara while dan do-while loop adalah dimana statement di dalam do-while 
loop dieksekusi sedikitnya satu kali. 
"Do-while loop" adalah struktur pengulangan pada bahasa pemrograman Java yang digunakan untuk mengeksekusi blok kode secara berulang selama kondisi yang diberikan masih terpenuhi atau bernilai true, tetapi dengan satu perbedaan utama dari while loop, yaitu bahwa do-while loop akan mengeksekusi blok kode setidaknya satu kali bahkan jika kondisi awal bernilai false.
Contoh penggunaan dari do-while loop di Java adalah sebagai berikut:
int i = 0;

do {
   System.out.println("Nilai i adalah " + i);
   i++;
} while (i < 5);
Dalam contoh di atas, nilai variabel i akan dicetak di konsol setidaknya sekali karena blok kode dalam do-while loop akan dieksekusi sebelum kondisi diuji. Setiap kali blok kode dalam do-while loop dieksekusi, nilai i akan bertambah 1, sehingga loop akan berhenti saat nilai i mencapai 5.

Seperti halnya while loop, kondisi dalam do-while loop harus dievaluasi sebagai boolean. Jika kondisi awal bernilai false, maka blok kode dalam do-while loop akan dieksekusi sekali, tetapi tidak akan dieksekusi lagi jika kondisi tetap bernilai false setelah itu.


3. for loop 
"For loop" adalah struktur pengulangan pada bahasa pemrograman Java yang digunakan untuk mengeksekusi blok kode secara berulang selama kondisi yang diberikan masih terpenuhi atau bernilai true, dengan menginisialisasi sebuah variabel, mengevaluasi kondisi, dan melakukan operasi iterasi dalam satu baris kode.
Contoh penggunaan dari for loop di Java adalah sebagai berikut:
for (int i = 0; i < 5; i++) {
   System.out.println("Nilai i adalah " + i);
}
Dalam contoh di atas, variabel i diinisialisasi dengan nilai 0, kemudian kode dalam loop akan dieksekusi selama nilai i kurang dari 5, dan setiap kali blok kode dalam loop dieksekusi, nilai i akan bertambah 1.

Kondisi dalam for loop juga harus dievaluasi sebagai boolean. Jika kondisi awal bernilai false, maka blok kode dalam for loop tidak akan pernah dieksekusi.



///Branching Statements 

1. break tstatement
"Break statement" adalah pernyataan yang digunakan pada bahasa pemrograman Java untuk menghentikan loop secara paksa. Ketika break statement dieksekusi dalam loop, maka program akan keluar dari loop, dan akan melanjutkan eksekusi pada pernyataan setelah loop.

Contoh penggunaan dari break statement di Java adalah sebagai berikut:
for (int i = 0; i < 5; i++) {
   if (i == 3) {
      break;
   }
   System.out.println("Nilai i adalah " + i);
}
Dalam contoh di atas, loop for akan dieksekusi selama nilai i kurang dari 5. Namun, ketika nilai i sama dengan 3, maka break statement akan dieksekusi dan program akan keluar dari loop for. Oleh karena itu, dalam contoh di atas, kode dalam loop for akan mencetak nilai i hingga i sama dengan 2 saja, dan setelah itu program akan melanjutkan eksekusi pada pernyataan setelah loop.

Break statement juga dapat digunakan dalam switch statement untuk menghentikan eksekusi case saat kondisi yang sesuai ditemukan.


2.  Continue statement 
"Continue statement" adalah pernyataan yang digunakan pada bahasa pemrograman Java untuk melanjutkan loop ke iterasi berikutnya tanpa mengeksekusi bagian dari loop yang ada di bawah continue statement pada iterasi saat ini.

Contoh penggunaan dari continue statement di Java adalah sebagai berikut:
for (int i = 0; i < 5; i++) {
   if (i == 2) {
      continue;
   }
   System.out.println("Nilai i adalah " + i);
}
Dalam contoh di atas, loop for akan dieksekusi selama nilai i kurang dari 5. Namun, ketika nilai i sama dengan 2, maka continue statement akan dieksekusi dan program akan melompat ke iterasi berikutnya tanpa mengeksekusi bagian dari loop yang ada di bawah continue statement pada iterasi saat ini. Oleh karena itu, dalam contoh di atas, kode dalam loop for akan mencetak semua nilai i kecuali nilai 2.

Continue statement biasanya digunakan dalam situasi di mana program harus mengabaikan beberapa nilai atau kondisi tertentu dalam loop, tetapi tetap melanjutkan eksekusi loop ke iterasi berikutnya.


3. Return statement 
"Return statement" adalah pernyataan yang digunakan pada bahasa pemrograman Java untuk mengembalikan nilai dari sebuah fungsi atau metode dan menghentikan eksekusi dari fungsi tersebut.

Return statement dapat digunakan dengan atau tanpa nilai pengembaliannya, tergantung pada jenis data yang dikembalikan oleh fungsi. Jika sebuah fungsi tidak mengembalikan nilai apapun, maka return statement dapat digunakan tanpa nilai pengembaliannya, seperti contoh berikut:
public void printNama(String nama) {
   System.out.println("Nama saya adalah " + nama);
   return;
}
Dalam contoh di atas, fungsi printNama menerima sebuah argumen nama dan mencetaknya ke konsol, dan tidak mengembalikan nilai apapun. Return statement digunakan untuk menghentikan eksekusi fungsi setelah kode mencetak argumen nama ke konsol.
