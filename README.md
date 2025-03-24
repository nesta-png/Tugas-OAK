# Tugas-latihan OAK

# 1. Jelaskan struktur antar hubungan dan beri contohnya

jawaban :

1. Struktur antar Hubungan bisa disebut sebagai sistem BUS, jadi BUS adalah sebuah subsistem yang mentransfer data atau listrik antar komponen komputer di dalam sebuah komputer atau antar komputer.Pada sistem komputer, bus ini termasuk perangkat internal, kecepatan pengiriman informasi melalui bus ini dilakukan dengan kecepatan tinggi.
   
Contoh :

- PCI ( Pheripheral Component Interconnect )

   bus yang didesain untuk menangani beberapa perangkat keras. PCI juga adalah suatu bandwidth tinggi yang populer, prosesor independent bus itu dapat berfungsi sebagai bus mezzenine atau bus periferal. Standar bus PCI ini dikembangkan oleh konsorsium PCI Special Interest Group yang dibentuk oleh Intel Corporation dan beberapa perusahaan lainnya, pada tahun 1992. Tujuan dibentuknya bus ini adalah untuk menggantikan Bus ISA/EISA yang sebelumnya digunakan dalam komputer IBM PC atau kompatibelnya.
  
- USB ( Universal Serial Bus ) 

   USB merupakan suatu teknologi yang memungkinkan kita untuk menghubungkan alat eksternal (peripheral) seperti scanner, printer, mouse, papan ketik (keyboard), alat penyimpan data (zip drive), flash disk, kamera digital atau perangkat lainnya ke komputer kita. USB sangat mendukung transfer data sebesar 12 Mbps ( juta bit per detik). Komputer (PC) saat ini, umumnya sudah memiliki port USB. Biasanya disediakan minimal 2 port. Jika dibandingkan dengan paralel port dan serial port, penggunaan port USB lebih mudah dalam penggunaannya.
  
- BUS PCI

   Bus yang tidak tergantung prosesor dan berfungsi sebagai bus mezzanine atau bus peripheral. Standar PCI adalah 64 saluran data pada kecepatan 33MHz, laju transfer data 263 MB per detik atau 2,112 Gbps. Keunggulan PCI tidak hanya pada kecepatannya saja tetapi murah dengan keping yang sedikit.
  
- BUS ISA ( Industry Standart Architecture )
  
   Industri computer personal lainnya merespon perkembangan ini dengan mengadopsi standarnya sendiri, bus ISA, yang pada dasarnya adalah bus PC/AT yang beroperasi pada 8,33 MHz. Keuntungannya adalah bahwa pendekatan ini tetap mempertahankan kompatibilitas dengan mesin-mesin dan kartu-kartu yang ada.

 # 2. Bila terlalu banyak modul atau perangkat dihubungkan pada bus maka akan terjadi penurunan kinerja, sebutkan penyebabnya?

 jawaban :

- Habisnya kapasitas transfer Bus sehingga memperlambat data, jadi setiap bus mempunyai lebar bus masing-masing jika kapasitas transfer data disini melebihi maka transfer data akan lambat.
  
- Antrian penggunaan bus semakin panjang, Hal ini sama seperti memperlambat data jika banyak banyaknya penggunaan bus maka data juga lambat data mentransfer.

- Semakin besar delay propagasi untuk mengkoordinasikan penggunaan bus.

# 3. 3. Umumnya perangkat berprioritas paling rendah memiliki waktu tunggu rata-rata yang paling singkat. Dengan dasar ini biasanya CPU diberi perioritas tertinggi pada SBI. Sebutkan alasan perangkat berprioritas 16 memiliki waktu tunggu rata-rata paling rendah? Dibawah kondisi seperti apa keadaan diatas tidak berlaku?

jawaban :

 Perangkat dengan prioritas lebih rendah (misalnya, prioritas 16) mungkin memiliki waktu tunggu rata-rata paling singkat jika sistem menggunakan mekanisme penjadwalan berbasis prioritas. Dalam mekanisme ini, perangkat dengan prioritas lebih tinggi (misalnya, CPU) diberikan akses langsung ke bus atau sumber daya lainnya. Ketika perangkat dengan prioritas lebih tinggi tidak memerlukan akses, perangkat dengan prioritas lebih rendah dapat menggunakan waktu idle ini untuk berkomunikasi, sehingga mengurangi waktu tunggu rata-rata mereka.

Misalnya, dalam sistem bus yang menggunakan penjadwalan prioritas, CPU dengan prioritas tertinggi akan selalu mendapatkan akses pertama ke bus. Namun, ketika CPU tidak memerlukan bus, perangkat dengan prioritas lebih rendah dapat menggunakan bus tanpa banyak penundaan.

- Kondisi Dimana Hal Ini Tidak Berlaku:
  
-Kontensi Tinggi dan Bandwidth Terbatas:

Dalam sistem dengan kontensi tinggi dan bandwidth bus terbatas, perangkat dengan prioritas lebih rendah dapat mengalami waktu tunggu yang lebih lama karena bus sering sibuk melayani perangkat dengan prioritas lebih tinggi.

-Penjadwalan Non-Prioritas:

Jika mekanisme penjadwalan tidak sepenuhnya berbasis prioritas dan menggunakan metode lain seperti round-robin atau time-slicing, waktu tunggu mungkin lebih merata di antara semua perangkat, tanpa memperhatikan prioritas.

-Penggunaan Puncak atau Beban Berat:

Selama periode penggunaan puncak atau di bawah beban berat, bahkan perangkat dengan prioritas lebih rendah mungkin menghadapi waktu tunggu yang meningkat karena permintaan keseluruhan pada bus. Dalam situasi ini, bus mungkin jarang idle, sehingga perangkat dengan prioritas lebih rendah harus menunggu lebih lama.


   
