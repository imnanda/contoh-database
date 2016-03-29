# Daftar Isi #

<br />
![http://lh6.ggpht.com/_ofnZnO0EGzU/SY7XH87I1jI/AAAAAAAABEY/njeGyBpLMdU/s288/phi_minimart_logo.png](http://lh6.ggpht.com/_ofnZnO0EGzU/SY7XH87I1jI/AAAAAAAABEY/njeGyBpLMdU/s288/phi_minimart_logo.png)


Catatan:
Gunakan _Compatibility View_ jika Anda menggunakan browser Internet Explorer 8 pada saat melihat halaman ini. Atau gunakan browser Firefox 3 dan Google Chrome untuk tampilan yang lebih baik.

# Pendahuluan #

<table border='0'>
<tr>
<td valign='top'>
<b>"PHI-Minimart"</b> adalah contoh database menggunakan skenario retailer bernama PHI-Minimart yang memiliki cabang yang tersebar di seluruh Indonesia. Pada tanggal 2 February 2009 ini kami merilis PHI-Minimart versi 0.1.<br>
</td>
<td>
<a href='http://code.google.com/p/sampledata/wiki/FormulirKontribusiNamaSupplier'><img src='http://lh5.ggpht.com/_ofnZnO0EGzU/SY27bs1FkrI/AAAAAAAABD4/gN0Gtd2uyQA/s288/butuh_kontributor_box.png' /></a>
</td>
</tr>
</table>

Pada versi ini fokus contoh data adalah pada modul penjualan sangat sederhana namun cukup digunakan untuk melihat data dalam berbagai dimensi yaitu :
  * dimensi waktu
  * performa cabang
  * performa karyawan
  * performa produk

# Deskripsi Tabel #

PHI-Minimart 0.1 terdiri tabel-tabel berikut :
  * **Tabel Master**
    * **ms\_kategori** : data kategori produk
    * **ms\_produk** : data produk
    * **ms\_harga\_harian** : daftar harga harian untuk tiap produk dan  tiap cabang
    * **ms\_cabang** : data cabang PHI-Minimart di seluruh Indonesia
    * **ms\_kota** :  data kota domisili PHI-Minimart
    * **ms\_propinsi** : data propinsi seluruh Indonesia
    * **ms\_karyawan** : data karyawan PHI-Minimart
  * **Tabel Transaksi**
    * **tr\_penjualan** : merupakan transaksi penjualan yang mencatat tanggal transaksi, di cabang mana transaksi dilakukan

# Instalasi Di MySQL #

Untuk instalasi di MySQL silahkan kunjungi halaman berikut ini : [http://mysql.phi-integration.com/instalasi/contoh-data-phi-minimart](http://mysql.phi-integration.com/instalasi/contoh-data-phi-minimart)

# Roadmap / Tahap Pengembangan #

## Tahap 1 ##
  * Penyelesaian **_master table_** yang berorientasi ke penjualan (produk, master harga, cabang / toko, dan lain-lain)
  * Generasi data untuk transaksi penjualan sederhana (tanpa nomor faktur) menggunakan [Kettle](http://kettle.pentaho.org)
  * Difokuskan hanya ke sejumlah cabang untuk memperkecil ukuran database (realisasi : 3 cabang)

![http://lh6.ggpht.com/_ofnZnO0EGzU/ScjzQC19N5I/AAAAAAAABLc/Su70_XkzyP0/s640/kettle_phi_minimart_v01.png](http://lh6.ggpht.com/_ofnZnO0EGzU/ScjzQC19N5I/AAAAAAAABLc/Su70_XkzyP0/s640/kettle_phi_minimart_v01.png)

## Tahap 2 ##
  * Penyelesaian **_master table_** yang berorientasi ke rantai pasokan / _supply chain_ (vendor, gudang, barcode / kode UPC, dan sebagainya)
  * Perbaikan nama supplier supaya lebih "natural"
  * Manajemen order yang lengkap mulai pemesanan, pembelian, pengantaran / delivery, dan _inventory_
  * Generasi data transaksi _supply chain_ menggunakan [Kettle](http://kettle.pentaho.org)
  * Memindahkan hosting project ke http://code.google.com/p/contoh-database

## Tahap 3 ##
  * Penyempurnaan transaksi


# Diagram Struktur Table / EER (Extended Entity-Relationship) #

![http://contoh-database.googlecode.com/svn/trunk/phi-minimart/images/schema_eerd_from_editor.png](http://contoh-database.googlecode.com/svn/trunk/phi-minimart/images/schema_eerd_from_editor.png)

# Download #

  * Untuk versi MySQL 5 download [disini](http://sampledata.googlecode.com/files/phi_minimart_mysql_v0.1.tar.gz).
