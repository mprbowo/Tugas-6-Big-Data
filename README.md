# Tugas-6-Big-Data
<h2>Tugas </h2>

Silakan selesaikan praktikum tersebut sesuai langkah-langkah sebelumnya, lalu laporkan hasilnya berupa link repository GitHub dengan nama spark-streaming disertai dengan screenshot hasilnya.
Jelaskan perbedaan spark streaming dengan metode stateless dan stateful stream processing ?
Jelaskan masing-masing maksud kode berikut sesuai nomor kodenya pada laporan praktikum Anda!
Nomor Kode

Sintaks

1 sys.argv, sys.stderr, StreamingContext, sc, socketTextStream, reduceByKey, lambda line, awaitTermination

2 nc, lk

3 spark-submit, master, local[*]

4 ssc.checkpoint, parallelize, updateStateByKey, flatMap

5 rdd.take(5), transform, rdd.sortByKey(False)

<h2>Jawab </h2>

1.    - sys.argv: Variabel yang berisi argumen baris perintah saat menjalankan skrip Python.
      - sys.stderr: Saluran standar untuk output kesalahan.
      - StreamingContext: Konteks inti dalam Spark Streaming untuk pemrosesan streaming.
      - sc: SparkContext untuk berinteraksi dengan kluster Spark.
      - socketTextStream: Membuat DStream dari data yang diterima melalui socket.
      - reduceByKey: Menggabungkan nilai-nilai dengan kunci yang sama dalam RDD menggunakan fungsi pengurangan.
      - lambda line: Fungsi anonim dengan satu parameter line.
      - awaitTermination: Meminta StreamingContext agar tetap berjalan hingga pemrosesan streaming selesai.
   
2. - nc, lk: Utilitas netcat untuk membuka koneksi dan mengirim/menerima data melalui jaringan.
3. - spark-submit: Perintah untuk mengirimkan aplikasi Spark ke kluster Spark untuk dieksekusi.
   - master: Argumen untuk menentukan alamat URL atau mode eksekusi kluster Spark.
   - local[*]: Mode eksekusi Spark lokal dengan menggunakan semua core yang tersedia pada mesin.

4. - ssc.checkpoint: Mengatur tempat penyimpanan sementara (checkpoint) untuk operasi pemrosesan streaming stateful.
   - parallelize: Membuat RDD dari koleksi data yang ada di memori dalam bentuk array.
   - updateStateByKey: Memperbarui state (keadaan) pada DStream dengan menggabungkan nilai-nilai yang memiliki kunci yang sama.
   - flatMap: Membagi setiap elemen dalam RDD menjadi beberapa elemen dalam bentuk yang berbeda.

5. - rdd.take(5): Mengambil n elemen pertama dari RDD dan mengembalikannya dalam bentuk list.
   - transform: Menerapkan transformasi pada DStream.
   - rdd.sortByKey(False): Mengurutkan pasangan kunci-nilai dalam RDD berdasarkan kunci secara menurun (descending order).
