# Anita
# Basis-Data-Pertemuan-8

# 1. Tampilkan semua isi/record tabel!
SELECT * FROM mahasiswa;

  ![alt text](https://github.com/DzakiAbiyyu/poto/blob/main/1.jpg?raw=true)
# 2. Ubah data tanggal lahir mahasiswa yang bernama Ari menjadi: 1979-08-31!
UPDATE mahasiswa SET tanggal_lahir = '1979-08-31'WHERE nama = 'Ari Santoso';

  ![alt text](https://github.com/DzakiAbiyyu/poto/blob/main/2.jpg?raw=true)
# 3. Tampilkan satu baris / record data yang telah diubah tadi yaitu record dengan nama Ari saja!
SELECT * FROM mahasiswa WHERE nama = 'Ari Santoso';

![alt text](https://github.com/DzakiAbiyyu/poto/blob/main/3.jpg?raw=true)
# 4. Hapus Mahasiswa yang bernama Dina!
DELETE FROM mahasiswa WHERE nama = 'Dina Marlina';

![alt text](https://github.com/DzakiAbiyyu/poto/blob/main/4.jpg?raw=true)
# 5. Tampilkan record atau data yang tanggal kelahirannya lebih dari atau sama dengan 1996-1-2!
SELECT * FROM mahasiswa WHERE tanggal_lahir >= '1996-01-02';

![alt text](https://github.com/DzakiAbiyyu/poto/blob/main/5.jpg?raw=true)
# 6. Tampilkan semua Mahasiswa yang berasal dari Bekasi dan berjenis kelamin perempuan!
SELECT * FROM mahasiswa WHERE kota = 'Bekasi' AND jenis_kelamin = 'Perempuan';

![alt text](https://github.com/DzakiAbiyyu/poto/blob/main/6.jpg?raw=true)
# 7. Tampilkan semua Mahasiswa yang berasal dari Bekasi dengan kelamin laki-laki atau Mahasiswa yang berumur lebih dari 22 tahun dengan kelamin wanita!
SELECT * FROM mahasiswa WHERE (kota = 'Bekasi' AND jenis_kelamin = 'Laki-laki') OR (YEAR(CURRENT_DATE) - YEAR(tanggal_lahir) > 22 AND jenis_kelamin = 'Perempuan');

![alt text](https://github.com/DzakiAbiyyu/poto/blob/main/7.jpg?raw=true)
# 8. Tampilkan data nama dan alamat mahasiswa saja dari tabel tersebut
SELECT nama,kota FROM mahasiswa;

![alt text](https://github.com/DzakiAbiyyu/poto/blob/main/8.jpg?raw=true)
# 9. Tampilkan data mahasiswa terurut berdasarkan nama
SELECT * FROM mahasiswa ORDER BY nama;

![alt text](https://github.com/DzakiAbiyyu/poto/blob/main/9.jpg?raw=true)

Apa bedanya penggunaan BETWEEN dan penggunaan operator >=
dan <= ? 
jawab : Secara singkat:

- `BETWEEN` digunakan untuk menentukan apakah sebuah nilai berada dalam rentang tertentu, termasuk kedua batas rentang.
- Operator `>=` (lebih besar atau sama dengan) digunakan untuk memeriksa apakah nilai lebih besar dari atau sama dengan nilai tertentu.
- Operator `<=` (kurang dari atau sama dengan) digunakan untuk memeriksa apakah nilai kurang dari atau sama dengan nilai tertentu.

Jadi, perbedaan utama adalah `BETWEEN` mencakup kedua batas rentang, sedangkan operator `>=` dan `<=` memeriksa apakah nilai lebih besar dari atau kurang dari batas tersebut.

Berikan kesimpulan anda!
jawab : tugas ini di berikan supaya kita bisa memahami tentang ddl dan databases serta oprator operator di dalam nya.
