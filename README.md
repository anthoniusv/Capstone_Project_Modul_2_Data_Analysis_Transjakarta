# Capstone_Project_Modul_2_Data_Analysis_Transjakarta
Anthonius Valentino B. P. | Purwadhika JCDS Bandung

# A. Latar Belakang Permasalahan
## A.1 Latar Belakang
Jakarta sebagai ibu kota merupakan pusat pemerintahan dan administratif Indonesia, sehingga banyak aktivitas bisnis, pemerintahan, dan ekonomi dilakukan di kota ini. Akibatnya, Jakarta mengalami kepadatan penduduk yang tinggi, yang mengurangi kemudahan mobilitas masyarakat. Kemacetan lalu lintas yang parah akhirnya mendorong kebutuhan akan transportasi publik yang memadai sebagai salah satu kebutuhan mendesak bagi masyarakat yang tinggal atau bekerja di Jakarta.

Ketersediaan sarana dan prasarana transportasi yang mendukung sangat penting, karena secara tidak langsung akan mempengaruhi produktivitas masyarakat. Dengan adanya transportasi publik yang efisien dan andal, masyarakat dapat menghemat waktu dalam perjalanan, mengurangi stres, dan meningkatkan efisiensi penggunaan waktu. Selain itu, transportasi publik yang baik juga dapat mengurangi polusi dan ketergantungan pada kendaraan pribadi, yang pada akhirnya akan memberikan kontribusi positif terhadap lingkungan dan kualitas hidup di Jakarta.

Saat ini terdapat beberapa alternatif moda transportasi umum yang dapat dipilih oleh masyarakat yang beraktivitas di Jakarta mulai dari Transjakarta, konektivitas KRL, MRT dan juga LRT. Salah satu metode transportasi yang populer adalah bus Transjakarta yaitu sistem transportasi bus rapid transit (BRT) pertama di asia tenggara. Artikel dari sindonews.com menyebutkan beberapa alasan mengapa metode transportasi ini populer diantaranya adalah tarif yang terjangkau, ketersediaan halte yang banyak di lokasi-lokasi kota Jakarta, faislitas memadai, tersedianya jalur khusus atau busway, dan terdapat tempat duduk khusus wanita.

Sebagai moda transportasi pilihan masyarakat yang banyak digunakan tentu pemerintah DKI Jakarta sebagai pengelola akan selalu berinovasi untuk meningkatkan mutu dan pelayanan bagi masyarakat. Namun untuk melakukan perbaikan tentu perlu dilakukan langkah awal sehingga perbaikan ataupun pembaharuan dari layanan Transjakarta dapat tepat sasaran sesuai dengan permasalahan yang dihadapi.

Mengenali pola pengguna Transjakarta dapat menjadi langkah awal untuk mengidentifikasi potensi perbaikan atau pembaharuan layanan. Pemahaman terhadap perilaku dan pola pengguna dapat memberikan wawasan yang berharga tentang kebutuhan dan preferensi masyarakat. Misalnya, dengan mengetahui waktu dan rute perjalanan yang paling padat, pemerintah dapat menyesuaikan frekuensi bus dan menambah rute baru yang lebih efisien.

Selain itu, analisis demografis pengguna, seperti usia dan jenis kelamin, dapat membantu dalam merancang layanan yang lebih inklusif dan ramah pengguna. Mengetahui segmen pengguna yang paling sering menggunakan layanan ini juga dapat membantu dalam mengembangkan strategi pemasaran yang lebih efektif.

Dengan demikian, pemahaman yang mendalam terhadap perilaku dan pola perjalanan pengguna Transjakarta adalah kunci untuk melakukan perbaikan yang tepat sasaran, meningkatkan efisiensi, dan memberikan pelayanan yang lebih baik bagi masyarakat.

## A.2. Identifikasi Masalah
Dengan melakukan data analisis diharapkan dapat menjawab pertanyaan sebagai berikut:
1. Insight demografis:
    Melihat apakah terdapat perbedaan pola perjalanan pada kelompok usia dan jenis kelamin pada pengguna Transjakarta
2. Frekuensi perjalanan:
    Menentukan pola intensitas perjalanan dari pengguna Transjakarta dan mengelompokkannya menjadi beberapa segmen. Segmen dari intensitas perjalanan ini kemudian dihubungkan dengan variabel-variabel lainnya untuk melihat bagaimana perilaku pengguna.
3. Pengaruh waktu terhadap perilaku pengguna:
    Menentukan bagaimana korelasi waktu perjalanan dengan faktor-faktor lain seperti demografis pengguna, pola perjalanan, tujuan perjalanan dan lain-lain.
4. Preferensi rute dan lokasi:
    Menentukan lokasi atau halte yang dapat dijadikan perhatian lebih bagi penyedia layanan Transjakarta, melakukan analisis terhadap rute perjalanan
5. Peluang optimalisasi layanan:
    Jika sudah dibuat analisis terhadap pola perilaku pengguna dapat diberikan masukan kepada pengelola layananan untuk melakukan perhatian lebih atau perbaikan yang dapat tepat guna dan didukung oleh data.

# B. Data Understanding
Berikut merupakan kolom-kolom yang menjadi variabel dalam dataset `Transjakarta.csv`:

| No. | Nama Kolom | Deskripsi |
| ---- | --------- | --------- |
| 1. | **transID** | Unique transaction id for every transaction |
| 2. | **payCardID** | Customers main identifier. The card customers use as a ticket for entrance and exit |
| 3. | **payCardBank** | Customers card bank issuer name |
| 4. | **payCardName** | Customers name that is embedded in the card |
| 5. | **payCardSex** | Customers sex that is embedded in the card |
| 6. | **payCardBirthDate** | Customers birth year |
| 7. | **corridorID** | Corridor ID / Route ID as key for route grouping |
| 8. | **corridorName** | Corridor Name / Route Name contains Start and Finish for each route |
| 9. | **direction** | 0 for Go, 1 for Back. Direction of the route |
| 10. | **tapInStops** | Tap In (entrance) Stops ID for identifying stops name |
| 11. | **tapInStopsName** | Tap In (entrance) Stops Name where customers tap in |
| 12. | **tapInStopsLat** | Latitude of Tap In Stops |
| 13. | **tapInStopsLon** | Longitude of Tap In Stops |
| 14. | **stopStartSeq** | Sequence of the stops, 1st stop, 2nd stops etc. Related to direction |
| 15. | **tapInTime** | Time of tap in. Date and time |
| 16. | **tapOutStops** | Tap Out (Exit) Stops ID for identifying stops name |
| 17. | **tapOutStopsName** | Tap out (exit) Stops Name where customers tap out |
| 18. | **tapOutStopsLat** | Latitude of Tap Out Stops |
| 19. | **tapOutStopsLon** | Longitude of Tap Out Stops |
| 20. | **stopEndSeq** | Sequence of the stops, 1st stop, 2nd stops etc. Related to direction |
| 21. | **tapOutTime** | Time of tap out. Date and time |
| 22. | **payAmount** | The number of what customers pay. Some are free. Some not |

# C. Data Analysis
Proses pengolahan data secara mendetail dapat dilihat pada jupyter notebook.

# D. Summary dan Managerial Implication

**Informasi Umum**
Berdasarkan pengolahan data secara univariat yaitu analisa yang dilakukan berdasarkan satu variabel dan juga bivariat untuk melihat hubungan ataupun keterkaitan satu variabel dengan yang lain baik dari kategori dan numerik, dapat dibuat ringkasan untuk memberikan gambaran umum mengenai pola perilaku dari pengguna Transjakarta pada bulan April 2023. Data menunjukkan bahwa terdapat variasi dalam metode pembayaran, jenis kelamin, kelompok usia, frekuensi perjalanan, serta waktu dan lokasi perjalanan. Analisis ini bertujuan untuk memberikan insight tentang pola perilaku pengguna Transjakarta yang dapat digunakan sebagai dasar untuk menyusun perbaikan dan peningkatan layanan.

**Berdasarkan Metode Pembayaran**
- **Metode Pembayaran Populer:** Mayoritas pengguna Transjakarta menggunakan kartu pembayaran digital yang dikeluarkan Bank DKI, diikuti oleh e-money dari Bank Mandiri. Kerjasama antara Transjakarta dan Bank DKI mungkin menjadi alasan utama di balik tingginya pengguna.
- **Statistika Pembayaran:** Bank DKI juga merupakan pilihan metode pembayaran utama pengguna Transjakarta baik pria maupun wanita. Metode pembayaran yang paling sedikit digunakan oleh wanita adalah metode online, sedangkan pria paling sedikit menggunakan kartu BNI.

**Berdasakan Jenis Kelamin**
- **Proporsi Pengguna:** 53.3% pengguna Transjakart berjenis kelamin perempuan, sementara 46.7% berjenis kelamin laki-laki.
- **Perbedaan Prilaku:** Pengguna perempuan cenderung lebih banyak dalam setiap kategori perjalanan dibandingkan laki-laki, kecuali untuk kategori short distance dimana perbedaanya tidak terlalu besar angkanya.
- **Perjalanan Berdasarkan Waktu:** Pengguna perempuan secara umum lebih banyak jumlahnya dibandingkan laki-laki berdasarkan jam perjalanan kecuali pada jam 5 pagi. Pengguna perempuan cenderung melakukan perjalanan lebih banyak di malam hari dibandingkan laki-laki.

**Berdasarkan Kelompok Usia**
- **Berdasarkan Kelompok Usia:** Mayoritas pengguna Transjakarta adalah dewasa (19-59 tahun), diikuti oleh anak/remaja (di bawah 18 tahun) dan lansia (di atas 60 tahun).
- **Perbedaan Perilaku:** Lansia dengan jenis kelamin laki-laki lebih banyak menggunakan Transjakarta dibandingkan perempuan. Lansia cenderung menggunakan Transjakarta sebagai moda transportasi umum.
- **Metode Pembayaran:** Kartu Bank DKI dominan di semua kelompok usia, dengan perbedaan di pilihan kedua dimana lansia lebih memilih Flazz BCA dibandingkan e-money

**Berdasarkan Frekuensi Perjalanan**
- **Kategori Penggunaan:** Frequent Traveler (lebih dari 15 hari/bulan), Occasional Traveler (6-15 hari/bulan), dan Rare Traveler (kurang dari 6 hari/bulan).
- **Proporsi Penggunaan:** Mayoritas pengguna adalah Frequent Traveler, menunjukkan bahwa Transjakarta adalah moda transportasi utama bagi pengguna.
- **Workday and Weekend Comparison:** Mayoritas pengguna pada Weekday atau hari kerja adalah Frequent Traveler, namun pada akhir pekan jumlah Frequent Traveler yang menggunakan Transjakarta tidak ada sama sekali. Pengguna pada hari Sabtu dan Minggu didominasi Rare Traveler
- **Jarak Perjalanan:** Frequent Traveler memiliki median jarak perjalanan paling kecil, sedangkan Occasional Traveler memiliki median jarak terbesar,
- **Durasi Perjalanan:** Occasional Traveler cenderung menempuh perjalanan dengan durasi terlama dengan median 78.55 menit.

**Berdasarkan Waktu Perjalanan**
- **Waktu Sibuk:** Puncak keramaian terjadi pada jam 6 pagi dan 17 sore. Sementara periode dengan jumlah penumpang sedikit terjadi pada periode pukul 10 pagi dampai 15 sore.
- **Durasi Perjalanan Waktu:** Pagi hari memiliki median durasi perjalanan paling kecil, sementara sore dan malah hari memiliki durasi perjalanan yang lebih panjang,
- **Hari Perjalanan:** Pengguna lebih banyak melakukan perjalanan pada hari kerja dibandingkan akhir pekan, Yaitu tertinggi pada hari Jumat.

**Berdasarkan Lokasi Perjalanan**
- **Lokasi Populer:** Jakarta Selatan dan Jakarta Barat adalah lokasi tap-in dan tap-out dengan pengguna paling banyak, sementara paling sedikit terjadi di luar Jakarta.
- **Rute Populer:** Rute yang paling banyak digunakan adalah Rusun Kapuk Muara -> Penjaringan, diikuti dengan rute sebaliknya Penjaringan -> Rusun Kapuk Muara.
- **Pola Tap-In dan Tap-Out:** Mayoritas pengguna melakukan tap-in di pagi hari terutama di Jakarta Barat dan Selatam. Tap-out paling banyak terjadi di sore hari, menunjukkan pola perjalanan pulang kerja

**Berdasarkan Jarak Perjalanan**
- **Kategori Jarak:** Perjalanan dikelompokkan menjadi Short (<= 1 km), Medium (1 - 3.5 km), dan long ( > 3.5 km). Mayoritas perjalanan berada dalam kategori Medium distance, sementara Long distance paling sedikit.
- **Kategori Kelompok Usia:** Pengguna dalam kategori usia dewasa paling banyak disetiap ketegori jarak.

**Berdasarkan Durasi Perjalanan**
- **Kategori Durasi:** Perjalanan dikelompokkan menjadi Short (<= 50 menit), Medium (50-100 menit), dan Long (> 100 menit). Mayoritas pengguna berada dalam kategori Medium Travel Duration.
- **Perbandingan Durasi:** Durasi perjalanan pada pagi hari lebih singkat dibandingkan sore dan malam hari.

Analisis lanjutan, managerial implication sampai kesimpulan secara mendetail dapat dilihat pada jupyter notebook.


