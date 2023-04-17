BAB 1 
Pengenalan Pemrograman Komputer 

penjelasan dari kodingan dibawah ini
public class Hello {
    public static void main (String[] args ){
        System.out.println("Selamat Datang");
    }
}
Kodingan di atas adalah contoh sederhana dari sebuah program Java yang mencetak "Selamat Datang" ke konsol. Berikut adalah penjelasan dari setiap baris kode:

1. public class Hello {: Ini adalah deklarasi kelas Java dengan nama "Hello". Nama kelas harus sesuai dengan nama file Java yang berisi kelas tersebut.

2. public static void main (String[] args ){: Ini adalah method utama (main method) dari program Java. Setiap program Java harus memiliki method utama dan harus memiliki signature yang persis seperti ini. Method utama adalah tempat di mana program dimulai saat dieksekusi.

3. System.out.println("Selamat Datang");: Ini adalah perintah untuk mencetak teks "Selamat Datang" ke konsol. Method println adalah method yang didefinisikan dalam kelas System.out, yang digunakan untuk mencetak teks ke konsol.

}: Ini menutup method utama.

}: Ini menutup kelas.

Jadi, program ini akan mencetak teks "Selamat Datang" ke konsol saat dijalankan.


public class KondisiOperator {
    public static void main (String[] args ){
       String status = "";
       int grade = 80;
       
       //mendapatkan status pelajar
       status = (grade >= 60)?"Passed":"Fail";
       
       //print status
       System.out.println(status);
    }
}
Program di atas merupakan contoh penggunaan operator kondisi (ternary operator) dalam bahasa pemrograman Java. Berikut adalah penjelasan dari setiap baris kode:

public class KondisiOperator {: Ini adalah deklarasi kelas Java dengan nama "KondisiOperator". Nama kelas harus sesuai dengan nama file Java yang berisi kelas tersebut.

public static void main (String[] args ){: Ini adalah method utama (main method) dari program Java. Setiap program Java harus memiliki method utama dan harus memiliki signature yang persis seperti ini. Method utama adalah tempat di mana program dimulai saat dieksekusi.

String status = "";: Ini adalah deklarasi variabel status dengan tipe data String dan nilai awal kosong ("").

int grade = 80;: Ini adalah deklarasi variabel grade dengan tipe data int dan nilai awal 80.

status = (grade >= 60)?"Passed":"Fail";: Ini adalah contoh penggunaan operator kondisi (ternary operator) dalam Java. Jika nilai dari variabel grade lebih besar atau sama dengan 60, variabel status akan diisi dengan string "Passed", jika tidak, variabel status akan diisi dengan string "Fail".

System.out.println(status);: Ini adalah perintah untuk mencetak nilai dari variabel status ke konsol.

}: Ini menutup method utama.

}: Ini menutup kelas.

Jadi, program ini akan mencetak nilai "Passed" ke konsol karena nilai dari variabel grade (80) lebih besar dari atau sama dengan 60. Jika nilai variabel grade diubah menjadi 50, maka nilai dari variabel status akan menjadi "Fail" karena nilai grade tidak mencukupi untuk lulus.


///Apa yang Disebut Bahasa Pemrograman?
Bahasa pemrograman adalah teknik komunikasi standar untuk mengekspresikan 
instruksi kepada komputer. Layaknya bahasa manusia, setiap bahasa memiliki tata tulis 
dan aturan tertentu. 
Bahasa pemrograman memfasilitasi seorang programmer untuk secara spesifik apa yang 
akan dilakukan oleh komputer selanjutnya, bagaimana data tersebut disimpan dan 
dikirim, dan apa yang akan dilakukan apabila terjadi kondisi yang variatif. 
Bahasa pemrograman dapat diklasifikasikan menjadi tingkat rendah, menengah, dan 
tingkat tinggi. Pergeseran tingkat dari rendah menuju tinggi menunjukkan kedekatan 
terhadap ”bahasa manusia”. 

///Alur Pembuatan Program 
1 Definisi Permasalahan
2 Analisa Permasalahan 
3 Desain Algoritma dan Representasi 
4 Pengkodean, Uji Coba dan Pembuatan Dokumentasi


BAB 2 
Pengenalan Bahasa JAVA


///Sejarah Singkat JAVA
Pada 1991, sekelompok insinyur Sun dipimpin oleh Patrick Naughton dan James 
Gosling ingin merancang bahasa komputer untuk perangkat konsumer seperti cable 
TV Box. Karena perangkat tersebut tidak memiliki banyak memori, bahasa harus 
berukuran kecil dan mengandung kode yang liat. Juga karena manufaktur – 
manufaktur berbeda memilih processor yang berbeda pula, maka bahasa harus 
bebas dari manufaktur manapun. Proyek diberi nama kode ”Green”. 
Kebutuhan untuk fleksibilitas, kecil, liat dan kode yang netral terhadap platform 
mengantar tim mempelajari implementasi Pascal yang pernah dicoba. Niklaus Wirth, 
pencipta bahasa Pascal telah merancang bahasa portabel yang menghasilkan 
intermediate code untuk mesin hipotesis. Mesin ini sering disebut dengan mesin 
maya (virtual machine). Kode ini kemudian dapat digunakan di sembarang mesin 
yang memiliki interpreter. Proyek Green menggunakan mesin maya untuk mengatasi 
isu utama tentang netral terhadap arsitektur mesin. 
Karena orang – orang di proyek Green berbasis C++ dan bukan Pascal maka 
kebanyakan sintaks diambil dari C++, serta mengadopsi orientasi objek dan bukan 
prosedural. Mulanya bahasa yang diciptakan diberi nama ”Oak” oleh James Gosling 
yang mendapat inspirasi dari sebuah pohon yang berada pada seberang kantornya, 
namun dikarenakan nama Oak sendiri merupakan nama bahasa pemrograman yang 
telah ada sebelumnya, kemudian SUN menggantinya dengan JAVA. Nama JAVA 
sendiri terinspirasi pada saat mereka sedang menikmati secangkir kopi di sebuah 
kedai kopi yang kemudian dengan tidak sengaja salah satu dari mereka 
menyebutkan kata JAVA yang mengandung arti asal bijih kopi. Akhirnya mereka 
sepakat untuk memberikan nama bahasa pemrograman tersebut dengan nama Java. 
Produk pertama proyek Green adalah Star 7 (*7), sebuah kendali jarak jauh yang 
sangat cerdas. Dikarenakan pasar masih belum tertarik dengan produk konsumer 
cerdas maka proyek Green harus menemukan pasar lain dari teknologi yang 
diciptakan. Pada saat yang sama, implementasi WWW dan Internet sedang 
mengalami perkembangan pesat. Di lain pihak, anggota dari proyek Green juga 
menyadari bahwa Java dapat digunakan pada pemrograman internet, sehingga 
penerapan selanjutnya mengarah menjadi teknologi yang berperan di web.


///Apa itu Teknologi JAVA?
1 Sebuah Bahasa Pemrograman
Sebagai sebuah bahasa pemrograman, Java dapat membuat seluruh bentuk aplikasi, 
desktop, web dan lainnya, sebagaimana dibuat dengan menggunakan bahasa 
pemrograman konvensional yang lain. 
Java adalah bahasa pemrograman yang berorientasi objek (OOP) dan dapat 
dijalankan pada berbagai platform sistem operasi. Perkembangan Java tidak hanya 
terfokus oada satu sistem operasi, tetapi dikembangkan untuk berbagai sistem 
operasi dan bersifat open source. 

2 Sebuah Development Environment
Sebagai sebuah peralatan pembangun, teknologi Java menyediakan banyak tools : 
compiler, interpreter, penyusun dokumentasi, paket kelas dan sebagainya. 

3 Sebuah Aplikasi 
Aplikasi dengan teknologi Java secara umum adalah aplikasi serbt a guna yang dapat 
dijalankan pada seluruh mesin yang memiliki Java Runtime Environment (JRE). 

4 Sebuah Deployment Environment 
Terdapat dua komponen utama dari Deployment Environment. Yang pertama adalah 
JRE, yang terdapat pada paket J2SDK, mengandung kelas – kelas untuk semua 
paket teknologi Java yang meliputi kelas dasar dari Java, komponen GUI dan 
sebagainya. Komponen yang lain terdapat pada Web Browser. Hampir seluruh Web 
Browser komersial menyediakan interpreter dan runtime environment dari teknologi 
Java.


///Mengapa Mempelajari JAVA?
Berdasarkan white paper resmi dari SUN, Java memiliki karakteristik berikut : 
1. Sederhana (Simple) 
Bahasa pemrograman Java menggunakan Sintaks mirip dengan C++ namun 
sintaks pada Java telah banyak diperbaiki terutama menghilangkan 
penggunaan pointer yang rumit dan multiple inheritance. Java juga 
menggunakan automatic memory allocation dan memory garbage collection. 
2. Berorientasi objek (Object Oriented) 
Java mengunakan pemrograman berorientasi objek yang membuat program 
dapat dibuat secara modular dan dapat dipergunakan kembali. Pemrograman 
berorientasi objek memodelkan dunia nyata kedalam objek dan melakukan 
interaksi antar objek-objek tersebut. 
3. Terdistribusi (Distributed) 
Java dibuat untuk membuat aplikasi terdistribusi secara mudah dengan adanya 
libraries networking yang terintegrasi pada Java. 
4. Interpreted 
Program Java dijalankan menggunakan interpreter yaitu Java Virtual Machine 
(JVM). Hal ini menyebabkan source code Java yang telah dikompilasi menjadi
Java bytecodes dapat dijalankan pada platform yang berbeda-beda. 
5. Robust 
Java mempuyai reliabilitas yang tinggi. Compiler pada Java mempunyai 
kemampuan mendeteksi error secara lebih teliti dibandingkan bahasa 
pemrograman lain. Java mempunyai runtime-Exception handling untuk 
membantu mengatasi error pada pemrograman. 
6. Secure 
Sebagai bahasa pemrograman untuk aplikasi internet dan terdistribusi, Java 
memiliki beberapa mekanisme keamanan untuk menjaga aplikasi tidak 
digunakan untuk merusak sistem komputer yang menjalankan aplikasi 
tersebut. 
7. Architecture Neutral 
Program Java merupakan platform independent. Program cukup mempunyai 
satu buah versi yang dapat dijalankan pada platform berbeda dengan Java 
Virtual Machine. 
8. Portable 
Source code maupun program Java dapat dengan mudah dibawa ke platform 
yang berbeda-beda tanpa harus dikompilasi ulang. 
9. Performance 
Performance pada Java sering dikatakan kurang tinggi. Namun performance 
Java dapat ditingkatkan menggunakan kompilasi Java lain seperti buatan Inprise, Microsoft ataupun Symantec yang menggunakan Just In Time 
Compilers (JIT). 
10. Multithreaded 
Java mempunyai kemampuan untuk membuat suatu program yang dapat 
melakukan beberapa pekerjaan secara sekaligus dan simultan. 
11. Dynamic 
Java didesain untuk dapat dijalankan pada lingkungan yang dinamis. Perubahan 
pada suatu class dengan menambahkan properties ataupun method dapat 
dilakukan tanpa menggangu program yang menggunakan class tersebut.



