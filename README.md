# Jarkom Modul 1 Lapres Kelompok T05
### Anggota Kelompok :
- M. Mikail Dwi K.          [05311840000028]
- Dimas Pramudya H.         [05311840000037]

## Soal Dan Penyelesaian
## A. Display Filter

### No. 1 
Sebutkan webserver yang digunakan pada ***"testing.mekanis.me"!***
- Penyelesaian :

Buka file **soal_jarkom_modul_no1-5,10.pcapng**, lalu ketik pada <i>display filter</i> 

```http.host == "testing.mekanis.me"```, maka akan muncul <i>web server</i> yang digunakan pada ***testing.mekanis.me***
![Screenshot (80)](https://user-images.githubusercontent.com/55182072/95986209-d5605e80-0e4f-11eb-9a98-e5916e7cc4de.png)

### No. 2 
Simpan gambar **"Tim_Kunjungan_Kerja_BAKN_DPR_RI_ke_Sukabumi141436.jpg"**!
- Penyelesaian :

Buka file **soal_jarkom_modul_no1-5,10.pcapng**, lalu selanjutnya pilih <i>file</i>, dan selanjutnya pilih <i>Export Object</i> kedalam <i>HTTP</i>
![Screenshot (83)](https://user-images.githubusercontent.com/55182072/95986520-56b7f100-0e50-11eb-863a-650f5257b50c.png)

Lalu selanjutnya, cari **HTTP Object*** yang mempunyai <i>file name</i> **"Tim_Kunjungan_Kerja_BAKN_DPR_RI_ke_Sukabumi141436.jpg"** lalu save
![Screenshot (84)](https://user-images.githubusercontent.com/55182072/95986843-cfb74880-0e50-11eb-89a8-645692fc943b.png)

Maka akan didapatkan gambar seperti dibawah ini
![Tim_Kunjungan_Kerja_BAKN_DPR_RI_ke_Sukabumi141436](https://user-images.githubusercontent.com/55182072/95986915-e8276300-0e50-11eb-9622-0d39f7282fec.jpg)


### No. 3 
Cari username dan password ketika login di "ppid.dpr.go.id"!
- Penyelesaian :
Buka file **soal_jarkom_modul_no1-5,10.pcapng**, lalu ketik pada <i>display filter</i>
```http.request and http.host == "ppid.dpr.go.id"```, lalu cari yang method nya ```POST```
![Screenshot (87)](https://user-images.githubusercontent.com/55182072/95991674-43f4ea80-0e57-11eb-8d48-a88a5625ca76.png)

Setelah itu bisa didapatkan ```username``` dan ```password``` ketika login di situs PPID DPR RI, yang bernama ```username``` : "10pemuda" dan ```passwordnya``` : "guncangdunia"
![Screenshot (88)](https://user-images.githubusercontent.com/55182072/95992059-ba91e800-0e57-11eb-974a-21a794dc5b85.png)

### No. 4
Temukan paket dari **web-web** yang menggunakan **basic authentication** method!
- Penyelesaian :

Buka file **soal_jarkom_modul_no1-5,10.pcapng**, lalu ketik pada <i>display filter</i>
```http.authbasic``` selanjutnya akan ditemukan paket dari web-web
![Screenshot (90)](https://user-images.githubusercontent.com/55182072/95992922-adc1c400-0e58-11eb-8001-3d7d05e7220d.png)

### No. 5
Ikuti perintah di aku.pengen.pw! Username dan password bisa didapatkan dari file .pcapng!
- Penyelesaian :

Buka file **soal_jarkom_modul_no1-5,10.pcapng**, lalu ketik pada <i>display filter</i>
```http.host == "aku.pengen.pw" and http.request.method == GET and http.authbasic``` lalu cari ```GET``` nya. Setelah itu bisa didapatkan ```username``` dan ```password``` untuk masuk ke ```aku.pengen.pw```. ```username``` nya adalah "kakakgamtenk" dan ```passwordnya``` "hartatahtabermuda"
![Screenshot (93)](https://user-images.githubusercontent.com/55182072/95995273-77d20f00-0e5b-11eb-987d-91dcb78b9a30.png)

Setelah itu kita login di web ```aku.pengen.pw``` dan bisa didapatkan hasil
![Screenshot (91)](https://user-images.githubusercontent.com/55182072/95995466-b5cf3300-0e5b-11eb-82e7-2121a5265545.png)

### No. 6
Seseorang menyimpan file zip melalui FTP dengan nama "Answer.zip". Simpan dan Buka file ***"Open This.pdf"*** di ***Answer.zip.*** Untuk mendapatkan password zipnya, temukan dalam file ***zipkey.txt*** (passwordnya adalah isi dari file txt tersebut).
- Penyelesaian :

Buka file **soal_jarkom_modul_no6,7,9.pcapng**, lalu ketik pada <i>display filter</i>
```ftp-data contains "Answer.zip"``` lalu di paket yang paling atas, klik kanan lalu pilih ```follow TCP Stream```
![Screenshot (101)](https://user-images.githubusercontent.com/55182072/95998162-c8973700-0e5e-11eb-8752-142d13828e50.png)

Selanjutnya, streamnya dikurangi 1 menjadi 12 yang awalnya 13, lalu save as data sebagai ```raw```
![Screenshot (102)](https://user-images.githubusercontent.com/55182072/95998428-098f4b80-0e5f-11eb-925b-62a4b160596a.png)

lalu, dari data ```raw``` tersebut, di save as menjadi ```zip```
![Screenshot (103)](https://user-images.githubusercontent.com/55182072/95998597-393e5380-0e5f-11eb-977f-791d0f748445.png)





### No. 7 
Ada 500 file zip yang disimpan ke FTP Server dengan nama 1.zip, 2.zip, ..., 500.zip. Salah satunya berisi pdf yang berisi puisi. Simpan dan Buka file pdf tersebut.
Your Super Mega Ultra Rare Hint = nama pdf-nya ***"Yes.pdf"***
- Penyelesaian :

### No. 8 
Cari objek apa saja yang didownload ***(RETR)*** dari koneksi FTP dengan Microsoft FTP Service!
- Penyelesaian :

### No. 9
Cari username dan password ketika login FTP pada localhost!
- Penyelesaian :

Buka file **soal_jarkom_modul_no6,7,9.pcapng**, lalu ketik pada <i>display filter</i>
```ip.src == 127.0.0.1 && ftp``` lalu klik kanan pilih ```follow TCP Stream```
![Screenshot (121)](https://user-images.githubusercontent.com/55182072/96012453-50d10880-0e6e-11eb-9edc-3aa03cda77a4.png)

Setelah itu, bisa diketahui bahwa ```username``` dan ``` passwordnya```
![Screenshot (122)](https://user-images.githubusercontent.com/55182072/96012580-71995e00-0e6e-11eb-9ea3-3649779ff05c.png)

Bisa disimpulkan bahwa ```username``` nya adalah dhana dan ```password``` nya adalah dhana123

### No. 10 
Cari file .pdf di wireshark lalu download dan buka file tersebut!
    ***clue: "25 50 44 46"*** 
- Penyelesaian :

Buka file **soal_jarkom_modul_no1-5,10.pcapng**, lalu ketik pada <i>display filter</i> 
```tcp contains 25:50:44:46``` lalu klik kanan pada paket yang ada, pilih ```Follow TCP Stream```
![Screenshot (126)](https://user-images.githubusercontent.com/55182072/96014199-4ca5ea80-0e70-11eb-83f7-db42e4a663dd.png)

Lalu, selanjutnya pada data tersebut klik simpan sebagai ```raw``` dengan ```streams``` 15
![Screenshot (128)](https://user-images.githubusercontent.com/55182072/96014522-af978180-0e70-11eb-8dc8-8b09ac35ddf1.png)

Lalu, jika data sudah disimpan sebagai ```raw``` selanjutnya kita menyimpan data tersebut dengan format file ```pdf```
![Screenshot (130)](https://user-images.githubusercontent.com/55182072/96014878-16b53600-0e71-11eb-89ab-71cb8be564df.png)

Selanjutnya, kita bisa mendapatkan file ```pdf``` yang sudah di download dengan isi :
![Screenshot (132)](https://user-images.githubusercontent.com/55182072/96015027-482e0180-0e71-11eb-9454-67213be5d8f8.png)


## B. Capture Filter
### No. 11
Filter sehingga wireshark hanya mengambil paket yang mengandung port 21!
- Penyelesaian :

Buka program ***Wireshark*** lalu klik ```Capture Filter``` dan ketikkan ```port 21```
![Screenshot (105)](https://user-images.githubusercontent.com/55182072/96004018-14e57580-0e65-11eb-8263-6c7adf4fb8f8.png)
Disini tampak kosong, karena tidak ada yang membuka ```port 21```

### No. 12
Filter sehingga wireshark hanya mengambil paket yang berasal dari port 80!
- Penyelesaian :

Buka program ***Wireshark*** lalu klik ```Capture Filter``` dan ketikkan ```src port 80```
![Screenshot (107)](https://user-images.githubusercontent.com/55182072/96004756-f764db80-0e65-11eb-873a-d8cdfe091bd6.png)

Tampak beberapa paket yang keluar dari ```port 80``` jika kita membuka suatu website


### No. 13
Filter sehingga wireshark hanya menampilkan paket yang menuju port 443!
- Penyelesaian :

Buka program ***Wireshark*** lalu klik ```Capture Filter``` dan ketikkan ```src port 443```
![Screenshot (109)](https://user-images.githubusercontent.com/55182072/96005172-65110780-0e66-11eb-9606-23bfde6683dd.png)

### No. 14
Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!
- Penyelesaian :

Langkah pertama yaitu, membuka ```command prompt``` untuk mendapatkan IP kita, dengan mengketikkan ```ipconfig```
![Screenshot (111)](https://user-images.githubusercontent.com/55182072/96005485-ae615700-0e66-11eb-9a87-85ea92f78f2f.png)

Lalu ```copy``` IP yang tampil pada ```IPv4 Address```, selanjutnya buka program ***Wireshark*** lalu klik ```Capture Filter``` dan ketikkan ```src [IP yang sudah didapatkan tadi]``` Misal : ```src  192.168.0.147```
![Screenshot (113)](https://user-images.githubusercontent.com/55182072/96006001-3a737e80-0e67-11eb-92a9-3f824078e119.png)

Berguna untuk meng ```capture``` paket data yang tujuannya ke IP kita

### No. 15
Filter sehingga wireshark hanya mengambil paket yang tujuannya ke monta.if.its.ac.id!
- Penyelesaian :

Langkah pertama yaitu, membuka ```command prompt``` untuk mendapatkan IP ***monta.if.its.ac.id*** kita harus mengketikkan ```ping monta.if.its.ac.id```
![Screenshot (115)](https://user-images.githubusercontent.com/55182072/96006449-b4a40300-0e67-11eb-9ca1-67652fb1c386.png)

IP ```monta.if.its.ac.id``` adalah ```103.94.190.11```

Jika sudah didapat alamat IP nya, selanjutnya buka program ***Wireshark*** lalu klik ```Capture Filter``` dan ketikkan ```host 103.94.190.11 ```
![Screenshot (117)](https://user-images.githubusercontent.com/55182072/96006953-37c55900-0e68-11eb-85ab-1b79ba0ecaa1.png)

Berguna untuk meng ```capture``` paket data yang tujuannya ke ```monta.if.its.ac.id```
