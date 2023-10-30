Cara membuat tabel mahasiswa menggunakan database polban

  1. Buka SQL Shell (psql), lalu login.
  
  ![image](https://github.com/Vools24/pertemuan2-basis-data/assets/148308642/dca9a559-efc4-46e8-ac7a-ef0ae2fc240d)
  ![image](https://github.com/Vools24/pertemuan2-basis-data/assets/148308642/1cfcb56a-40dc-4eeb-a1b6-7577213db24e)

  2. Check database dengan syntax: \l
  ![image](https://github.com/Vools24/pertemuan2-basis-data/assets/148308642/f3058b70-2422-4f9f-b9b1-8644159b6785)

  3. Masuk kedalam database polban dengan syntax berikut: \c polban
  ![image](https://github.com/Vools24/pertemuan2-basis-data/assets/148308642/f667b7d9-2325-4925-8842-6844af3f6092)

  4. Membuat tabel dengan CREATE TABLE mahasiswa (
    nim VARCHAR(10),
    nama VARCHAR(50),
    gender VARCHAR(10),
    alamat VARCHAR(100),
    asal_tempat VARCHAR(50),
    tanggal_lahir DATE,
    tahun_masuk INTEGER,
    nomor_handphone VARCHAR(15)
);

  5. Memasukkan data pada database yang telah dibuat dengan syntax: INSERT INTO mahasiswa (column1, columnN) VALUES (value1, valueN);
     INSERT INTO mahasiswa (nim, nama, gender, alamat, asal_tempat, tanggal_lahir, tahun_masuk, nomor_handphone) 
VALUES 
    ('221331048', 'Muhamad Rivaldyansyah', 'L', 'Cimahi', 'Bandung', '2004-04-15', 2022, '62882002067632'),
    ('221331033', 'Afiq Rasydan', 'L', 'Cimahi', 'Cimahi', '2004-10-08', 2022, '6281221020386'),
    ('221331034', 'Alvian Pradentra Kelana', 'L', 'Bandung', 'Karanganyar', '2003-12-16', 2022, '6288229288184'),
    ('221331035', 'Arham Surya Balad', 'L', 'Garut', 'Garut', '2003-03-08', 2022, '62895359421468'),
    ('221331036', 'Aulia Nisa', 'P', 'Garut', 'Garut', '2004-04-03', 2022, '6289662951338'),
    ('221331037', 'Dava Ikhsan Reyvan', 'L', 'Cimahi', 'Bandung', '2004-05-04', 2022, '627776561658'),
    ('221331038', 'Denis Maulana Wahyudi', 'L', 'Ciwidey', 'Bandung', '2003-08-10', 2022, '6285320035623'),
    ('221331039', 'Dewi Yulia Puspita Sari', 'P', 'Bandung', 'Bandung', '2003-07-04', 2022, '62895366920715'),
    ('221331040', 'Dikri Nugraha', 'L', 'Cimahi', 'Bandung', '2003-05-26', 2022, '62881023421454'),
    ('221331041', 'Faidillah Abdul Aziz', 'L', 'Cimahi', 'Bandung', '2004-09-16', 2022, '6282119303577'),
    ('221331042', 'Ferina Najwa', 'P', 'Rancaekek', 'Bandung', '2004-06-09', 2022, '62881022750960'),
    ('221331043', 'Ghiyats Ar-Rizgi', 'L', 'Cirebon', 'Cirebon', '2004-05-07', 2022, '6287721287963'),
    ('221331044', 'Ifathya Farah Azhari', 'P', 'Padalarang', 'Cirebon', '2002-06-26', 2022, '6289652235671'),
    ('221331045', 'Indah Safitri', 'P', 'Bandung', 'Bandung', '2005-01-02', 2022, '6281312714975'),
    ('221331046', 'Jane Wilham Aziz Fadhillah', 'L', 'Bandung', 'Bandung', '2004-03-13', 2022, '6285864524634'),
    ('221331047', 'Michele Filius Patris Arep Sinuor', 'L', 'Cimahi', 'Bandung', '2004-04-16', 2022, '6282130935243'),
    ('221331049', 'Muhammad Akmal Alfarisi', 'L', 'Bandung', 'Bandung', '2004-12-13', 2022, '625156797943'),
    ('221331050', 'Muhammad Azzam Khalif Hasanudin', 'L', 'Baleendah', 'Bandung', '2003-10-05', 2022, '6283824314243'),
    ('221331051', 'Nabil Herandika Chikal Hidayat', 'L', 'Padalarang', 'Bandung', '2003-10-10', 2022, '6289521008072'),
    ('221331052', 'Nadifi Islami Putri', 'P', 'Bandung', 'Bandung', '2022-09-28', 2022, '6282115473201');
    (221331053, 'Nike Julian Nensi', 'P', 'Bandung', 'Subang', '2003-07-29', 2022, '6281914674294'),
    (221331054, 'R. Samsam Muhammad Raafi', 'L', 'Tasikmalaya', 'Tasikmalaya', '2003-08-09', 2022, '6282120052723'),
    (221331055, 'Rafi Dzulfikar', 'L', 'Jakarta', 'Jakarta', '2003-11-03', 2022, '6281280777153'),
    (221331056, 'Rani Nur Fitriani', 'P', 'Tasikmalaya', 'Tasikmalaya', '2004-10-10', 2022, '6282317950575'),
    (221331057, 'Rezza Mediani Fadilah', 'P', 'Sukabumi', 'Sukabumi', '2004-12-03', 2022, '6281399347551'),
    (221331058, 'Rifan Aghni Al Farisan', 'L', 'Tasikmalaya', 'Tasikmalaya', '2003-08-09', 2022, '6285930305254'),
    (221331059, 'Rio Febrian', 'L', 'Sumedang', 'Sumedang', '2004-02-22', 2022, '6287802596170'),
    (221331060, 'Rizki Ramadhan Yusuf', 'L', 'Cimahi', 'Bandung', '2002-11-09', 2022, '62895412860621'),
    (221331061, 'Syagira Afifah', 'P', 'Cimahi', 'Bandung', '2003-09-01', 2022, '6285795669915'),
    (221331062, 'Taufig Rahman', 'L', 'Banten', 'Banten', '2004-10-10', 2022, '6281384364760'),
    (221331063, 'Wina Apriliani', 'P', 'Tasikmalaya', 'Tasikmalaya', '2004-04-04', 2022, '6285559244868');

  6. Menampilan data pada database mahasiswa dengan syntax: SELECT * FROM mahasiswa;
      Tampilan pada sql
        ![image](https://github.com/Vools24/pertemuan2-basis-data/assets/148308642/f0118b18-5c85-4f33-9974-e208cd6f6fa0)
      Tampilan pada DBeaver
         ![image](https://github.com/Vools24/pertemuan2-basis-data/assets/148308642/20796f0a-398a-4416-91f3-5be25677204e)
      Tampilan pada PgAdmin4
        ![image](https://github.com/Vools24/pertemuan2-basis-data/assets/148308642/4b5eb5ac-9e50-4d1f-bdd7-3ac04f014680)

