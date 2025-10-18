# LAPORAN PRAKTIKUM PEMROGRAMAN BERORIENTASI OBJEK (PBO)

## Topik Praktikum

**Mengunduh dan Memasang Plugin iReport serta Implementasi Laporan Menggunakan JasperReports**

Laporan praktikum ini mendokumentasikan langkah-langkah instalasi plugin **iReport** dan **JdesktopLayout** pada NetBeans serta implementasi pembuatan laporan menggunakan **JasperReports**.

---

## Detail Laporan

| Kategori | Detail |
| :--- | :--- |
| **Mata Kuliah** | Pemrograman Berorientasi Objek (PBO) |
| **Dosen Pengampu** | Bayu Adhi Nugroho, Ph.D. |
| **Penyusun** | Husain Asrarillah (09020624035) |
| **Program Studi** | Sistem Informasi |
| **Fakultas** | Sains dan Teknologi |
| **Universitas** | Universitas Islam Negeri Sunan Ampel Surabaya |
| **Tahun** | 2025 |

---

## 🛠️ Pemasangan iReport dan JdesktopLayout (Plugin NetBeans)

Bagian ini menjelaskan langkah-langkah untuk memasang plugin yang diperlukan di IDE NetBeans.

### Persiapan Awal

1.  Pastikan sudah mengunduh dan mengekstrak file `iReportPlugin` dan `JdekstopLayout`.

### Langkah-langkah Instalasi

1.  Menambahkan file yang sudah diunduh pada NetBeans:
    * (Menu) `Tools` ➔ `Plugin`.
    
    <img width="686" height="297" alt="image" src="https://github.com/user-attachments/assets/39680bdd-7eb6-48f0-ae30-e71720d9c106" />

2.  Pada menu **Plugins**, pilih tab **Downloaded** ➔ Klik **Add Plugins**.
    <img width="663" height="353" alt="image" src="https://github.com/user-attachments/assets/58fb835a-dd80-49d1-92a5-70b1dad411c3" />

3.  Pilih dan cari file `.nbm` (`iReportPlugin`) dan `JdesktopLayout`. Klik **Open** lalu klik **Install**. NetBeans akan meminta **Restart** ulang.
    <img width="756" height="456" alt="image" src="https://github.com/user-attachments/assets/bf56b1f5-a837-4014-a6c9-4b634a7c7bc1" />
    
4.  Untuk memastikan plugin sudah diinstal, buka menu **Installed**. Jika sudah ada keempat *plug-in* JasperReports, pastikan statusnya **Activate**.
    <img width="827" height="508" alt="image" src="https://github.com/user-attachments/assets/83d51649-0649-4d04-97cf-77d3b402ae63" />

5.  Setelah instalasi berhasil, **Welcome Windows** iReport Plugin akan muncul.
    <img width="819" height="460" alt="image" src="https://github.com/user-attachments/assets/ff90e2c3-c29f-4c3c-aa4f-eab251ad9d46" />

---

## 📄 Membuat JasperReport

Berikut adalah langkah-langkah untuk membuat dan mengimplementasikan laporan menggunakan JasperReports.

### Pembuatan File Laporan

1.  Pada folder *project*, klik kanan lalu `New` ➔ `Report Wizard`.
    *(Jika belum ada, klik `other` lalu cari `Report` dan pilih `Report Wizard`)*.
    <img width="523" height="347" alt="image" src="https://github.com/user-attachments/assets/a200416c-29d9-411f-bf7c-58d665725041" />

2.  Memilih *layout* atau *template* yang diinginkan.
    
    <img width="566" height="411" alt="image" src="https://github.com/user-attachments/assets/687840ef-43b6-4933-b020-cf323dfc668d" />

3.  Beri nama File lalu `Next`.
    
    <img width="596" height="437" alt="image" src="https://github.com/user-attachments/assets/70acc28c-b0ec-4205-8c39-edd47be276c1" />

4.  Menghubungkan ke Database.
    
    <img width="539" height="649" alt="image" src="https://github.com/user-attachments/assets/9723ee48-9273-49f0-a697-c6b82201c666" />

5.  Mengisi data koneksi sesuai arahan lalu `Next`.
    
    <img width="611" height="751" alt="image" src="https://github.com/user-attachments/assets/c2693069-f0f7-42ac-85bd-f10c698138bd" />

6.  Isi **Query SQL** yang terkoneksi dengan NetBeans, lalu klik `Next`.
    <img width="727" height="696" alt="image" src="https://github.com/user-attachments/assets/48e45022-2d96-4d39-aac6-87f0ef5fbf9a" />

7.  Pindahkan seluruh *field* data dari kiri ke kanan (atau sesuai kebutuhan), lalu `Next`.
    <img width="756" height="542" alt="image" src="https://github.com/user-attachments/assets/1b809807-d9d9-46d4-a81f-61962907a33b" />

8.  Langsung `Next` (melanjutkan langkah *Grouping*).
    <img width="711" height="510" alt="image" src="https://github.com/user-attachments/assets/d9e40b1a-dbff-4fb7-b5c1-026b9fce6500" />

9.  `Finish`.
    
    <img width="711" height="524" alt="image" src="https://github.com/user-attachments/assets/2e58b775-90f2-489e-aed2-41ec399947ce" />

10. **Desain tampilan laporan** sesuai keinginan di editor iReport.
    <img width="810" height="476" alt="image" src="https://github.com/user-attachments/assets/a61149b0-c946-42da-a590-12a80a3bfc92" />


### Implementasi pada Program Utama

1.  Pada program utama (**JFrame**), tambahkan tombol **"CETAK"**.
    <img width="745" height="611" alt="image" src="https://github.com/user-attachments/assets/56363040-9958-462b-8b19-30a873fe60c3" />

2.  Berikan **Kode Action** pada tombol tersebut agar bekerja dengan baik untuk memanggil laporan.
    **Implementasi Kode Action**
    <img width="919" height="613" alt="image" src="https://github.com/user-attachments/assets/298024f2-b6e2-47eb-a05c-1ed2522c90d7" />

3.  Setelah menekan tombol Cetak yang sudah berlogika, akan muncul **Tampilan Jasper Reports** (laporan yang telah dibuat).|
    <img width="928" height="616" alt="image" src="https://github.com/user-attachments/assets/ee7f4296-4c60-4031-a967-1c95d280198f" />
