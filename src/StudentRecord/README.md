
PENJELASAN STUDENT RECORD

//Pertama

public class StudentRecord {

    private String name;
    private String address;
    private int age; 
    private double mathGrade; 
    private double englishGrade; 
    private double scienceGrade; 
    private double average;
    private char nilaiAngka;
    
    private static int studentCount;
    
    public StudentRecord()
    {
        //area penulisan kode
        studentCount++;
    }
    
    public StudentRecord(String temp){ 
        this.name = temp; 
        studentCount++;
    } 
    public StudentRecord(String name, String address){ 
        this.name = name; 
        this.address = address; 
        studentCount++;
    } 
    public StudentRecord(double mGrade, double eGrade, double sGrade){ 
        mathGrade = mGrade; 
        englishGrade = eGrade; 
        scienceGrade = sGrade; 
        studentCount++;
    }
    
    public String getName() {
        return name;
    }
    
    public void setName(String name){
        this.name = name;
    }
    
    public String getAddress() {
        return address;
    }
    
    public void setAddress(String address){
        this.address = address;
    }
    
    public int getAge(){
        return age;
    }
    
    public void setAge(int age){
        this.age = age;
    }
    
    public double getMathGrade() {
        return mathGrade;
    }
    
    public void setMathGrade(double mathGrade){
        this.mathGrade = mathGrade;
    }
    
    public double getEnglishGrade(){
        return englishGrade;
    }
    
    public void setEnglishGrade(double englishGrade){
        this.englishGrade = englishGrade;
    }
    
    public double getScienceGrade(){
        return scienceGrade;
    }
    
    public void setScienceGrade(double scienceGrade){
        this.scienceGrade = scienceGrade;
    }
    
    public double getAverage(){
        average = (mathGrade + englishGrade + scienceGrade) / 3;
        return average;
    }
    
    public static int getStudentCount (){
        return studentCount;
    }
    
    public void print( String temp ){ 
        System.out.println("Name:" + name); 
        System.out.println("Address:" + address); 
        System.out.println("Age:" + age); 
        } 
        public void print(double eGrade, double mGrade, double sGrade) {
        System.out.println("Name:" + name); 
        System.out.println("Math Grade:" + mGrade); 
        System.out.println("English Grade:" + eGrade); 
        System.out.println("Science Grade:" + sGrade); 
        }

     public char getNilaiAngka (){
        if(average > 80){
            nilaiAngka='A';
        }
        else if(average > 65){
            nilaiAngka='B';
        }
        else if(average > 55){
            nilaiAngka='C';
        }
        else if(average > 40){
            nilaiAngka='D';
        }
        else if(average > 0){
            nilaiAngka='E';
        }
        return nilaiAngka;
    }  
}


Kode di atas adalah kelas Java yang disebut StudentRecord, yang merepresentasikan data dari seorang siswa. Ada beberapa variabel yang disimpan di dalam kelas, seperti nama, alamat, umur, dan nilai untuk tiga pelajaran: matematika, bahasa Inggris, dan sains. Ada juga variabel untuk menyimpan nilai rata-rata siswa dan nilai huruf siswa.

Beberapa metode yang tersedia untuk mengakses dan mengubah nilai dari variabel tersebut, seperti getName(), getAddress(), getAge(), getMathGrade(), setMathGrade(), getEnglishGrade(), setEnglishGrade(), getScienceGrade(), dan setScienceGrade(). Ada juga metode getAverage() yang menghitung rata-rata dari nilai tiga pelajaran dan mengembalikan nilai tersebut. Terakhir, ada metode getNilaiAngka() yang mengembalikan nilai huruf siswa berdasarkan nilai rata-rata siswa.

Ada juga variabel static bernama studentCount yang menghitung jumlah instance dari kelas StudentRecord yang telah dibuat. Terdapat empat constructor dengan parameter yang berbeda, yang digunakan untuk membuat instance dari kelas ini dengan nilai yang berbeda untuk variabel-variabel yang telah ditentukan. Ada juga dua metode print yang digunakan untuk mencetak informasi siswa ke konsol.


//Kedua


public class StudentRecordExample {

    public static void main(String[] args){
        StudentRecord annaRecord = new StudentRecord();
        annaRecord.setName("Anna");
        annaRecord.setAddress("Padang");
        annaRecord.setAge(23);
        annaRecord.setMathGrade(80);
        annaRecord.setEnglishGrade(70);
        annaRecord.setScienceGrade(80);
        
        
        //Tampilkan 
        System.out.println("Nama                :"+annaRecord.getName());
        System.out.println("Alamat              :"+annaRecord.getAddress());
        System.out.println("Umur                :"+annaRecord.getAge());
        System.out.println("Matematika          :"+annaRecord.getMathGrade());
        System.out.println("B Inggris           :"+annaRecord.getEnglishGrade());
        System.out.println("Ilmu Pengetahuan    :"+annaRecord.getScienceGrade());
        System.out.println("Rata-Rata Nilai     :"+annaRecord.getAverage());
        
        StudentRecord aliRecord = new StudentRecord();
        aliRecord.setName("Ali");
        aliRecord.setAddress("Padang");
        aliRecord.print("");
        aliRecord.print(80,70,80);
        
        
        StudentRecord budiRecord = new StudentRecord("Budi","Bukittinggi");
        budiRecord.print("");
        System.out.println("Jumlah Siswa   :"+
                StudentRecord.getStudentCount());
    }
}


Program di atas adalah contoh penggunaan kelas StudentRecord yang berisi informasi tentang data siswa. Kelas tersebut memiliki beberapa atribut seperti nama, alamat, usia, nilai matematika, bahasa Inggris, dan ilmu pengetahuan, serta atribut untuk menghitung jumlah siswa yang dibuat.

Kelas StudentRecord memiliki beberapa metode seperti konstruktor, setter dan getter untuk mengatur dan mengambil nilai atribut siswa, metode untuk menghitung nilai rata-rata dan nilai akhir dalam bentuk huruf, dan juga metode cetak untuk menampilkan informasi siswa.

Kelas StudentRecordExample berfungsi sebagai contoh penggunaan kelas StudentRecord. Pada program ini, terdapat tiga objek yang dibuat yaitu annaRecord, aliRecord, dan budiRecord. Objek tersebut digunakan untuk mengatur dan mengambil informasi siswa, serta menampilkan hasil dari pengolahan data yang dilakukan dengan metode yang telah disediakan oleh kelas StudentRecord.
