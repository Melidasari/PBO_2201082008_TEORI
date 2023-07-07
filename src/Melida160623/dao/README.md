PENJELASAN TENTANG PACKAGE DAO

DISINI TERDAPAT BEBERAPA CLASS


package Melida160623.dao;

import Melida160623.model.Anggota;

import java.util.List;

public interface AnggotaDao {

    void insert(Anggota Anggota);
    void update(int index, Anggota anggota);
    void delete(int index);
    Anggota getAnggota(int index);
    List<Anggota> getAll();
    
}

Antarmuka AnggotaDao mendefinisikan beberapa metode yang harus diimplementasikan oleh kelas-kelas yang mengimplementasikan antarmuka ini.

Metode insert(Anggota anggota) digunakan untuk memasukkan objek Anggota ke dalam penyimpanan data.

Metode update(int index, Anggota anggota) digunakan untuk memperbarui objek Anggota pada indeks tertentu di dalam penyimpanan data.

Metode delete(int index) digunakan untuk menghapus objek Anggota pada indeks tertentu dari penyimpanan data.

Metode getAnggota(int index) digunakan untuk mengambil objek Anggota pada indeks tertentu dari penyimpanan data.

Metode getAll() digunakan untuk mengambil semua objek Anggota yang tersimpan dalam penyimpanan data dan mengembalikannya dalam bentuk daftar (list).

Antarmuka AnggotaDao bertindak sebagai kontrak yang menyatakan operasi-operasi yang harus disediakan oleh implementasi DAO (Data Access Object) untuk mengakses dan memanipulasi data terkait anggota. Kelas-kelas yang mengimplementasikan antarmuka ini akan memberikan implementasi sesuai dengan logika bisnis dan sumber data yang digunakan.


package Melida160623.dao;

import java.util.List;

import java.util.ArrayList;

import Melida160623.model.Anggota;

public class AnggotaDaoImpl implements AnggotaDao {

   private List<Anggota> data = new ArrayList<>();
    
   public AnggotaDaoImpl(){
       data.add(new Anggota ("A001","Melida Sari","Padang","P"));
       data.add(new Anggota ("A002","Arrasya","Padang","L"));
       data.add(new Anggota ("A003","Asrivo","Sijunjung","P"));
   }
   
    public void insert(Anggota anggota) {
        data.add(anggota);
    }
    public void update(int index, Anggota anggota){
        data.set(index, anggota);
    }
    public void delete(int index){
        data.remove(index);
    }
    public Anggota getAnggota(int index){
        return data.get(index);
    }
    public List<Anggota> getAll(){
        return data;
    }
}


Kelas AnggotaDaoImpl mengimplementasikan semua metode yang didefinisikan dalam antarmuka AnggotaDao.

Konstruktor AnggotaDaoImpl digunakan untuk menginisialisasi data awal dalam List data. Pada contoh ini, data awal berupa tiga objek Anggota yang ditambahkan ke dalam data.

Metode insert(Anggota anggota) digunakan untuk memasukkan objek Anggota ke dalam List data.

Metode update(int index, Anggota anggota) digunakan untuk memperbarui objek Anggota pada indeks tertentu di dalam List data.

Metode delete(int index) digunakan untuk menghapus objek Anggota pada indeks tertentu dari List data.

Metode getAnggota(int index) digunakan untuk mengambil objek Anggota pada indeks tertentu dari List data.

Metode getAll() digunakan untuk mengambil semua objek Anggota yang tersimpan dalam List data dan mengembalikannya dalam bentuk daftar (list).

Implementasi AnggotaDaoImpl ini menyediakan operasi CRUD (Create, Read, Update, Delete) untuk mengakses dan memanipulasi data anggota.

Data anggota disimpan dalam List data sebagai penyimpanan sementara dalam contoh ini, namun bisa digantikan dengan sumber data yang sesuai seperti basis data atau sistem penyimpanan lainnya.

