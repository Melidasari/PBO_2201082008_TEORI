PENJELASAN TENTANG PACKAGE MODEL


public class Anggota {

    private String kodeAnggota;
    private String namaAnggota;
    private String alamat;
    private String jenisKelamin;

    public Anggota(String kodeAnggota, String namaAnggota, String alamat, String jenisKelamin) {
        this.kodeAnggota = kodeAnggota;
        this.namaAnggota = namaAnggota;
        this.alamat = alamat;
        this.jenisKelamin = jenisKelamin;
    }

    public String getKodeAnggota() {
        return kodeAnggota;
    }

    public void setKodeAnggota(String kodeAnggota) {
        this.kodeAnggota = kodeAnggota;
    }

    public String getNamaAnggota() {
        return namaAnggota;
    }

    public void setNamaAnggota(String namaAnggota) {
        this.namaAnggota = namaAnggota;
    }

    public String getAlamat() {
        return alamat;
    }

    public void setAlamat(String alamat) {
        this.alamat = alamat;
    }

    public String getJenisKelamin() {
        return jenisKelamin;
    }

    public void setJenisKelamin(String jenisKelamin) {
        this.jenisKelamin = jenisKelamin;
    }
    
}


Kelas Anggota memiliki beberapa atribut, yaitu kodeAnggota, namaAnggota, alamat, dan jenisKelamin. Atribut-atribut ini digunakan untuk menyimpan informasi tentang seorang anggota.

Konstruktor Anggota digunakan untuk menginisialisasi objek Anggota dengan memberikan nilai awal pada atribut-atribut kodeAnggota, namaAnggota, alamat, dan jenisKelamin.

Setiap atribut memiliki metode getter dan setter. Metode getter digunakan untuk mengambil nilai dari atribut, sedangkan metode setter digunakan untuk mengubah nilai dari atribut.

Metode getKodeAnggota() mengembalikan nilai dari atribut kodeAnggota.

Metode setKodeAnggota(String kodeAnggota) digunakan untuk mengatur nilai dari atribut kodeAnggota.

Metode getNamaAnggota() mengembalikan nilai dari atribut namaAnggota.

Metode setNamaAnggota(String namaAnggota) digunakan untuk mengatur nilai dari atribut namaAnggota.

Metode getAlamat() mengembalikan nilai dari atribut alamat.

Metode setAlamat(String alamat) digunakan untuk mengatur nilai dari atribut alamat.

Metode getJenisKelamin() mengembalikan nilai dari atribut jenisKelamin.

Metode setJenisKelamin(String jenisKelamin) digunakan untuk mengatur nilai dari atribut jenisKelamin.

Kelas Anggota digunakan untuk merepresentasikan data anggota dalam aplikasi dan memberikan kemampuan untuk mengakses dan memanipulasi informasi tersebut.
