penjelasan tentang class AnggotaController



package Melida160623.controller;

import Melida160623.view.FormAnggota;

import Melida160623.model.Anggota;

import Melida160623.dao.AnggotaDaoImpl;

import Melida160623.dao.AnggotaDao;

import java.util.*;

import javax.swing.table.DefaultTableModel;

/**
 *
 * @author Lenovo
 */

public class AnggotaController {

    FormAnggota view;
    Anggota anggota;
    AnggotaDao dao;
    
    public AnggotaController(FormAnggota view) {
    
        this.view = view;
        dao = new AnggotaDaoImpl();
    }
    
    public void clearForm(){
        view.getTxtKodeAnggota().setText("");
        view.getTxtNamaAnggota().setText("");
        view.getTxtAlamat().setText("");
        view.getCboJenisKelamin().removeAllItems();
        view.getCboJenisKelamin().addItem("L");
        view.getCboJenisKelamin().addItem("P");
    }
    
    public void tampil(){
        DefaultTableModel tabelModel = (DefaultTableModel) view.getTabelAnggota().getModel();
        tabelModel.setRowCount(0);
        List<Anggota> List = dao.getAll();
        for (Anggota a : List){
            Object[] row = {
                a.getKodeAnggota(),
                a.getNamaAnggota(),
                a.getAlamat(),
                a.getJenisKelamin()
            };
            tabelModel.addRow(row);
        }
    }
}



Package dan Import:

Package: Melida160623.controller adalah package (paket) yang mengorganisir kelas-kelas terkait pengendalian atau kontrol dalam aplikasi.
Import: Baris-baris yang dimulai dengan import adalah pernyataan untuk mengimpor kelas-kelas yang diperlukan dalam kelas AnggotaController. Dalam kodingan ini, beberapa kelas yang diimpor adalah FormAnggota (kelas yang ada dalam package Melida160623.view), Anggota (kelas yang ada dalam package Melida160623.model), AnggotaDaoImpl dan AnggotaDao (kelas-kelas yang ada dalam package Melida160623.dao), DefaultTableModel (kelas yang ada dalam package javax.swing.table), serta java.util.* (package yang berisi utilitas-utilitas standar Java).
Deklarasi kelas:

kotlin
Copy code
public class AnggotaController {
    // ...
}
Ini adalah deklarasi kelas AnggotaController. Semua kode untuk pengendalian anggota (memberikan aksi, mengambil data, dll.) akan ditempatkan di dalam kelas ini.

Variabel instance:

sql
Copy code
FormAnggota view;
Anggota anggota;
AnggotaDao dao;
Bagian ini mendeklarasikan tiga variabel instance yaitu view, anggota, dan dao yang akan digunakan dalam kelas AnggotaController. Variabel view adalah objek FormAnggota yang akan digunakan untuk mengakses komponen-komponen GUI, anggota adalah objek Anggota yang akan digunakan untuk menyimpan data anggota, dan dao adalah objek AnggotaDao yang akan digunakan untuk mengakses data anggota dari sumber data (misalnya database).

Konstruktor:

arduino
Copy code
public AnggotaController(FormAnggota view) {
    this.view = view;
    dao = new AnggotaDaoImpl();
}
Ini adalah konstruktor kelas AnggotaController yang menerima objek FormAnggota sebagai argumen. Konstruktor ini menginisialisasi variabel view dengan nilai yang diberikan (menghubungkan objek AnggotaController dengan tampilan/form yang sesuai) dan menginisialisasi variabel dao dengan sebuah instance dari kelas AnggotaDaoImpl (implementasi dari AnggotaDao).

Metode clearForm():

scss
Copy code
public void clearForm(){
    view.getTxtKodeAnggota().setText("");
    view.getTxtNamaAnggota().setText("");
    view.getTxtAlamat().setText("");
    view.getCboJenisKelamin().removeAllItems();
    view.getCboJenisKelamin().addItem("L");
    view.getCboJenisKelamin().addItem("P");
}
Ini adalah metode clearForm() yang digunakan untuk mengosongkan form pada objek view. Metode ini menghapus teks dari beberapa komponen dalam objek view (seperti TxtKodeAnggota, TxtNamaAnggota, TxtAlamat) dan mengatur ulang komponen combo box (`C
