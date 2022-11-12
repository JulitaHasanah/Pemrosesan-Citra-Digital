> Nama : Julita Hasanah <br>

> Nim : 2110131120005

<br>

<h1 align="center"><b>Steganografi dan Image Enhancement</b></h1><br>

## **Stegalografi**

---

<p align="justify">Steganografi adalah sebuah metode dalam pemrosesan citra digital untuk menyembunyikan suatu data rahasia ke dalam sebuah citra.<br></p>
Data yang disembunyikan dapat berupa:

<img width="200" align="left" style="margin:25px" src="img/cover_stego.png"><br><br>

- Gambar
- Teks
- Suara
- Dll

<br><br><br>

### **Bagaimana Langkah Steganografi ?**

Adapun langkah-langkah yang dilakukan dalam menerapkan metode
steganografi adalah:

- Ubah citra warna ke dalam citra grayscale.
- Ubah pesan yang akan disisipkan ke dalam bentuk biner.
- Cek untuk setiap piksel yang ada pada citra, dan lakukan:
- Ambil nilai LSB pada citra
- Ambil nilai bit pesan yang akan disisipkan
- Jika nilai sama, tambahkan 0 ke dalam citra output, jika tidak tambahkan 1.
- Simpan gambar.

<br><br>

## **Image Enhancement**

---

<p align="justify">Image Enhancement adalah perbaikan kualitas citra yang bertujuan agar hasilnya lebih sesuai untuk tampilan atau analisis citra lebih lanjut. Misalnya, Anda dapat menghilangkan noise, mempertajam, atau mencerahkan gambar, sehingga lebih mudah untuk mengidentifikasi fitur utama.<br>

<img width="200" height="230" align="left" style="margin:25px" src="img/noisy.png">
<img width="200" height="230" align="left" style="margin:25px" src="img/gelap.png">
<img width="200" height="230" align="left" style="margin:25px" src="img/blurv.png"><br>
<img width="300" hegiht="200" align="left" style="margin:25px" src="img/blur.png">
<img width="300" hegiht="200" align="left" style="margin:25px" src="img/dark.png">

<br><br><br><br><br><br><br>
<br><br><br><br><br><br><br>
<br><br><br><br><br><br><br>
<br><br><br><br>

<p align="justify">Berdasarkan ranah (domain) operasinya, metode-metode untuk perbaikan kualitas citra dapat dikelompokkan menjadi dua kategori:</p>

1. Image enhancement dalam ranah spasial (Spatial Domain)
2. Image enhancement dalam ranah frekuensi (Frequency Domain)

<br>

### **1. Spatial Domain**<br>

<img width="300" style="margin:25px" src="img/spatial.png"><br>
Metode-metode image enhancement dalam ranah spasial dilakukan dengan memanipulasi secara langsung pixel-pixel di dalam citra.

- Misalkan :

  - f(x,y) : citra input
  - g(x,y) : citra output
  - T adalah operator terhadap f

- Metode pemroseran citra dalam ranah spasial dinyatakan seagai :
  g(x,y) = T[f(x,y)]

- T bisa beroperasi pada satu pixel, sekelompok pixel bertetangga, atau keseluruhan pixel di dalam citra.

- Jadi, metode dalam ranah spasial dapat dilakukan pada araa titik (pixel), aras lokal, dan aras global

<img width="500"  style="margin:25px" src="img/aras.png"><br>

<br>

### **2. Frequency Domain**<br>

Misalnya menggunakan Fourier Transform<br>
<img width="400" style="margin:10px" src="img/frequency.png"><br>

- Misalkan :

  - f ' (x,y) : citra hasil operasi
  - T(u,v) : citra konvolusi
  - R(u,v) : citra asli

- Metode pemroseran citra dalam ranah frekuensi dinyatakan sebagai :<br>
  f ' (u,v) = T(u,v) R(u,v)

<p align="justify">Metode-metode image enhancement dalam ranah frekuensi dilakukan dengan mengubah citra terlebih dahulu dari ranah spasial keranah frekuensi, baru kemudian memanipulasi nilai-nilai frekuens tersebut.<br><br>
Masing-masing ranah operasi digunakan untuk tujuan spesifik, karena tidak semua perbaikan citra dapat dilakukan dalam ranah spasial.</p>
<br>

Proses-proses yang termasuk kedalam perbaikan kualitas citra:

- Pengubahan kecerahan gambar (image brightening)
- Citra negatif (image negatives)
- Peregangan kontras (contrast stretching)
- Pengubahan histogram citra.
- Pelembutan citra (image smoothing)
- Penajaman (sharpening) tepi(edge).
- Pewarnaan semu(pseudocolouring)
- Pengubahan geometrik
- dll

<br>
