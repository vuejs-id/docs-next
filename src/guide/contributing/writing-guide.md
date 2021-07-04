# Panduan Penulisan Dokumentasi Vue

Menulis dokumentasi adalah latihan empati. Kami tidak menggambarkan realitas objektif - *source code* sudah melakukannya. Tugas kami adalah membantu membentuk hubungan antara pengguna dan ekosistem Vue. Panduan yang terus berkembang ini memberikan beberapa aturan dan rekomendasi tentang bagaimana melakukannya secara konsisten di ekosistem Vue.

## Prinsip

- **Sebuah fitur tidak akan dirilis sampai didokumentasikan dengan baik.**
- **Beri perhatian ke kapasitas kognitif pengguna (yaitu kekuatan otak).** Saat pengguna mulai membaca, mereka mulai dengan sejumlah kekuatan otak yang terbatas dan ketika kekuatan itu habis, mereka akan berhenti belajar.
  - Kapasitas kognitif **terkuras lebih cepat** oleh kalimat yang kompleks, harus mempelajari lebih dari satu konsep sekaligus, dan contoh abstrak yang tidak langsung berhubungan dengan pekerjaan pengguna.
  - Kapasitas kognitif **terkuras lebih lambat** ketika kita membantu membuat mereka merasa cerdas secara konsisten, kuat, dan ingin tahu. Memecah hal-hal menjadi bagian-bagian yang mudah dicerna dan memperhatikan alur dokumentasi dapat membantu menjaga mereka tetap dalam keadaan ini.
- **Selalu coba untuk melihat dari sudut pandang pengguna.** Ketika kita memahami sesuatu secara menyeluruh, itu menjadi jelas bagi kita. Ini disebut _kutukan pengetahuan_. Untuk menulis dokumentasi yang baik, cobalah untuk mengingat apa yang pertama kali perlu Anda ketahui saat mempelajari konsep ini. Jargon apa yang perlu Anda pelajari? Bagian mana yang Anda salah pahami? Apa yang butuh waktu lama untuk benar-benar dipahami? Dokumentasi yang baik membantu pengguna di hal-hal yang tepat. Akan sangat membantu untuk berlatih menjelaskan konsep yang ingin didokumentasikan kepada orang-orang secara langsung terlebih dahulu.
- **Jelaskan _masalah_ terlebih dahulu, lalu solusinya.** Sebelum menunjukkan cara kerja sebuah fitur, penting untuk menjelaskan mengapa fitur itu ada. Jika tidak, pengguna tidak akan memiliki konteks untuk mengetahui apakah informasi ini penting bagi mereka (apakah ini masalah yang mereka alami?) atau pengetahuan/pengalaman sebelumnya untuk menghubungkannya.
- **Saat menulis, jangan takut untuk bertanya**, _terutama_ jika Anda takut mereka akan tampak "bodoh". Menjadi orang yang mendapat kritikan itu sulit, tetapi itu satu-satunya cara bagi kita untuk lebih memahami apa yang perlu kita jelaskan.
- **Terlibatlah dalam diskusi fitur.** API terbaik berasal dari pengembangan berbasis dokumentasi, tempat kami membuat fitur yang mudah dijelaskan, daripada mencoba mencari cara untuk menjelaskannya nanti. Mengajukan pertanyaan (terutama pertanyaan "bodoh") lebih awal sering kali membantu mengungkapkan kebingungan, inkonsistensi, dan perilaku bermasalah sebelum diperlukan perubahan besar untuk memperbaikinya.

## Penyusunan

- **Instalasi/Integrasi**: Memberikan gambaran menyeluruh tentang cara mengintegrasikan perangkat lunak ke sebanyak mungkin jenis proyek yang diperlukan.
- **Perkenalan/Memulai**:
  - Memberikan gambaran kurang dari 10 menit tentang masalah yang dipecahkan proyek ini dan mengapa proyek ini ada.
  - Memberikan gambaran kurang dari 30 menit tentang masalah yang dipecahkan proyek ini dan bagaimana caranya, termasuk kapan dan mengapa menggunakan proyek ini serta beberapa contoh kode sederhana. Di bagian akhir, tautkan ke laman Instalasi dan awal Panduan Esensial.
- **Panduan**: Buat pengguna merasa pintar, kuat, dan ingin tahu, lalu pertahankan kondisi ini agar pengguna mempertahankan motivasi dan kapasitas kognitif untuk terus belajar lebih banyak. Laman panduan dimaksudkan untuk dibaca secara berurutan, jadi umumnya harus diurutkan dari rasio daya/usaha tertinggi ke terendah.
  - **Esensial**: Seharusnya tidak diperlukan lebih dari 5 jam untuk membaca Esensial, meskipun lebih pendek lebih baik. Tujuannya adalah untuk memberikan 20% pengetahuan yang akan membantu pengguna menangani 80% kasus penggunaan. Esensial dapat menautkan ke panduan yang lebih lanjut dan API, meskipun, dalam banyak kasus, Anda harus menghindari pemberian tautan tersebut. Ketika memberikan tautan, Anda juga perlu memberikan konteks sehingga pengguna mengetahui apakah mereka harus mengikuti tautan ini pada bacaan pertama mereka. Kalau tidak begitu, banyak pengguna yang akhirnya menghabiskan kapasitas kognitif mereka untuk melompat-lompat, mencoba mempelajari keseluruhan aspek fitur sebelum melanjutkan, dan sebagai hasilnya, tidak pernah menyelesaikan bacaan Esensial yang pertama. Ingatlah bahwa membaca dengan lancar lebih penting daripada menyeluruh. Kami ingin memberi orang-orang informasi yang mereka butuhkan untuk menghindari pengalaman yang membuat frustrasi, tetapi mereka selalu dapat kembali dan membaca lebih lanjut, atau mencari di Google masalah yang kurang umum kalau mereka menemukannya.
  - **Lanjutan**: Meskipun Esensial membantu orang menangani ~80% kasus penggunaan, panduan berikutnya membantu pengguna mencapai 95% kasus penggunaan, ditambah informasi yang lebih mendetail tentang fitur yang bukan esensial (misalnya transisi, animasi), fitur untuk kenyamanan yang lebih kompleks (misalnya mixin, arahan khusus), dan peningkatan pengalaman pengembang (misalnya BEJ, plugin). 5% terakhir dari kasus penggunaan yang lebih khusus, kompleks, dan/atau rentan terhadap penyalahgunaan akan diserahkan ke buku petunjuk dan referensi API, yang dapat ditautkan dari panduan lanjutan ini.
- **Referensi/API**: Menyediakan daftar fitur-fitur yang lengkap, termasuk informasi jenis, deskripsi masalah yang dipecahkan oleh masing-masing fitur, contoh setiap kombinasi opsi, serta tautan ke panduan, buku petunjuk, dan sumber daya internal lainnya yang memberikan detail lebih lanjut. Tidak seperti laman lain, laman ini tidak dimaksudkan untuk dibaca secara berurutan, sehingga banyak detail yang dapat diberikan. Referensi ini juga harus lebih mudah dibaca secara sepintas daripada panduan, jadi formatnya harus lebih seperti entri kamus dan bukan format panduan yang bercerita.
- **Migrasi**:
  - **Versi**: Saat perubahan penting dibuat, sebaiknya sertakan daftar lengkap perubahan, termasuk penjelasan mendetail tentang alasan perubahan itu dibuat dan cara memigrasikan proyek dari versi sebelumnya.
  - **Dari proyek lain**: Bagaimana perangkat lunak ini dibandingkan dengan perangkat lunak serupa? Ini penting untuk membantu pengguna memahami masalah tambahan apa yang mungkin kita pecahkan atau ciptakan untuk mereka, dan sejauh mana mereka dapat mentransfer pengetahuan yang sudah mereka miliki.
- **Panduan Gaya**: Pasti ada beberapa bagian penting dalam pengembangan yang memerlukan keputusan tetapi bukan inti dari API. Panduan gaya ini memberikan rekomendasi yang terdidik dan terdogma untuk membantu memandu keputusan-keputusan ini. Rekomendasi ini tidak boleh diikuti begitu saja, tetapi dapat membantu tim menghemat waktu dengan menyelaraskan detail yang lebih kecil.
- **Buku Petunjuk**: Panduan dalam buku petunjuk ditulis dengan asumsi pengguna telah akrab dengan Vue dan ekosistemnya. Masing-masing buku petunjuk adalah dokumen yang sangat terstruktur yang menjelaskan beberapa detail implementasi umum yang mungkin dihadapi oleh pengembang Vue.

## Penulisan & Tatabahasa

### Gaya

- **Tajuk harus menjelaskan masalah**, bukan solusi. Contoh tajuk yang kurang efektif seperti "Menggunakan props", karena menjelaskan solusi. Tajuk yang lebih baik adalah "Meneruskan Data ke Komponen Anak dengan Props", karena memberikan konteks masalah yang dipecahkan dengan menggunakan props. Pengguna tidak akan memperhatikan penjelasan suatu fitur sampai mereka mengetahui mengapa/kapan mereka menggunakannya.
- **Saat Anda memberikan pengetahuan, nyatakan** di awal dan tautkan ke sumber daya untuk pengetahuan yang kurang umum yang Anda kira.
- **Perkenalkan hanya satu konsep baru pada satu waktu bila memungkinkan** (termasuk teks dan contoh kode). Bahkan jika banyak orang dapat memahami ketika Anda memperkenalkan lebih dari satu konsep, akan ada banyak juga yang tidak paham - dan bahkan mereka yang paham akan lebih terkuras kapasitas kognitifnya.
- **Hindari blok konten khusus untuk tips dan peringatan jika memungkinkan.** Biasanya lebih baik untuk memadukannya secara lebih alami ke dalam konten utama, misalnya dengan membangun contoh untuk mendemonstrasikan *edge case*.
- **Jangan sertakan lebih dari dua tips dan peringatan yang terjalin per laman.** Jika Anda menemukan bahwa lebih dari dua tips diperlukan dalam satu laman, pertimbangkan untuk menambahkan bagian peringatan untuk mengatasi masalah ini. Panduan ini dimaksudkan untuk dibaca langsung, dan tips dan peringatan dapat menjadi membingungkan atau mengalihkan perhatian seseorang yang mencoba memahami konsep dasarnya.
- **Hindari saran yang terkesan memengaruhi** (misalnya "Anda harus melakukan X, karena itu praktik terbaik" atau "X adalah yang terbaik karena memberi Anda pemisahan penuh dari masalah"). Sebaliknya, tunjukkan dengan contoh masalah tertentu yang manusiawi yang disebabkan dan/atau dipecahkan oleh suatu pola.
- **Saat memutuskan apa yang akan diajarkan terlebih dahulu, pikirkan pengetahuan apa yang akan memberikan rasio kekuatan/usaha terbaik.** Itu berarti mengajarkan apa pun yang akan membantu pengguna memecahkan kesulitan terbesar atau jumlah masalah terbesar, dengan upaya yang relatif sedikit untuk dipelajari. Ini membantu orang yang belajar menjadi merasa pintar, kuat, dan ingin tahu, sehingga kapasitas kognitif mereka akan terkuras lebih lambat.
- **Kecuali konteksnya memberikan templat untai atau sistem *build*, hanya tulis kode yang berfungsi di lingkungan perangkat lunak ini (misalnya Vue, Vuex, dll.).**
- **Perlihatkan, jangan hanya beri tahu.** Misalnya, "Untuk menggunakan Vue di sebuah laman, Anda dapat menambahkan ini ke HTML Anda" (lalu tunjukkan tag skrip), alih-alih "Untuk menggunakan Vue di sebuah laman, Anda dapat menambahkan elemen skrip dengan atribut src, yang nilainya harus berupa tautan ke sumber yang disusun Vue".
- **Sebisa mungkin hindari humor (untuk dokumentasi berbahasa Inggris)**, terutama referensi sarkasme dan budaya pop, karena tidak dapat diterjemahkan dengan baik lintas budaya.
- **Jangan pernah memberikan konteks yang lebih kompleks dari yang seharusnya.**
- **Dalam kebanyakan kasus, utamakan tautan antar bagian dokumentasi daripada mengulangi konten yang sama di beberapa bagian.** Beberapa pengulangan dalam konten memang tidak dapat dihindari dan bahkan penting sebagai pembelajaran. Namun, terlalu banyak pengulangan juga membuat dokumen lebih sulit dipelihara, karena perubahan di API akan memerlukan perubahan di banyak tempat dan membuatnya jadi mudah untuk melewatkan sesuatu. Ini memang keseimbangan yang sulit untuk dicapai.
- **Spesifik lebih baik daripada generik.** Misalnya, contoh komponen `<BlogPost>` lebih baik daripada `<ComponentA>`.
- **Yang dikenali lebih baik daripada yang tidak diketahui.** Misalnya, contoh komponen `<Blog Post>` lebih baik daripada `<Currency Exchange Settings>`.
- **Jadilah relevan secara emosional.** Penjelasan dan contoh yang berhubungan dengan sesuatu yang dialami dan diperhatikan seseorang akan selalu lebih efektif.
- **Selalu utamakan bahasa yang lebih sederhana dan terus terang daripada bahasa yang rumit atau jargon.** Misalnya:
  - "Anda dapat menggunakan Vue dengan elemen skrip" alih-alih "untuk memulai penggunaan Vue, satu opsi yang mungkin adalah dengan memasukkannya melalui elemen skrip HTML"
  - "*function* yang mengembalikan *function*" alih-alih "*function* yang berurutan lebih tinggi"
- **Hindari penggunaan bahasa yang terkesan menggampangkan**, seperti "mudah", "hanya", "jelas", dll. Untuk referensi, lihat [Words To Avoid in Educational Writing](https://css-tricks.com/words-avoid-educational-writing/).

### Tatabahasa

- **Hindari penggunaan singkatan** dalam penulisan dan contoh kode (misalnya `attribute` lebih baik daripada `attr`, `message` lebih baik daripada `msg`), kecuali jika Anda secara khusus merujuk singkatan dalam API (misalnya `$attrs `). Simbol singkatan yang disertakan pada keyboard standar (misalnya `@`, `#`, `&`) boleh digunakan.
- **Saat merujuk contoh berikutnya secara langsung, gunakan titik dua (`:`) untuk mengakhiri kalimat**, bukan titik (`.`).
- **Gunakan koma Oxford** (misalnya "a, b, dan c" alih-alih "a, b dan c"). ![Mengapa koma Oxford itu penting](/images/oxford-comma.jpg)  
  - Sumber: [The Serial (Oxford) Comma: When and Why To Use It](https://www.inkonhand.com/2015/10/the-serial-oxford-comma-when-and-why-to-use-it/)
- **Saat mereferensikan nama sebuah proyek, gunakan nama yang merujuk pada proyek itu sendiri sebagaimana adanya.** Misalnya, "webpack" dan "npm" keduanya harus menggunakan huruf kecil karena itulah yang dirujuk oleh dokumentasinya.
- **Gunakan Kapitalisasi Judul untuk tajuk** - setidaknya untuk saat ini, karena itulah yang kami gunakan di seluruh dokumentasi. Ada penelitian yang menunjukkan bahwa kapitalisasi kalimat (hanya kata pertama dari judul yang dimulai dengan huruf kapital) sebenarnya lebih mudah dibaca dan juga mengurangi kognitif ekstra untuk penulis dokumentasi, karena mereka tidak harus mencoba mengingat apakah menggunakan huruf besar untuk kata-kata seperti "dan", "dengan", dan "tentang".
- **Jangan menggunakan emoji (kecuali dalam diskusi).** Emoji terkesan lucu dan ramah, tetapi dapat menjadi pengalih perhatian dalam dokumentasi dan beberapa emoji bahkan bisa punya arti yang berbeda dalam budaya yang berbeda.

## Iterasi & Komunikasi

- **Keunggulan berasal dari iterasi/pengulangan.** Draf pertama selalu buruk, tetapi menulisnya termasuk bagian penting dari proses. Sangat sulit untuk menghindari perkembangan yang lambat dari Buruk -> Cukup Baik -> Baik -> Hebat -> Menginspirasi -> Luar Biasa.
- **Tunggu sampai sesuatu itu "Bagus" sebelum dipublikasikan.** Komunitas akan membantu Anda lebih jauh.
- **Cobalah untuk tidak bersikap defensif saat menerima umpan balik.** Tulisan kita bisa sangat pribadi bagi kita, tetapi jika kita kesal dengan orang-orang yang membantu kita membuatnya lebih baik, mereka akan berhenti memberi umpan balik atau mulai membatasi umpan balik yang mereka berikan.
- **Koreksi karya Anda sendiri sebelum menunjukkannya kepada orang lain.** Jika Anda menunjukkan seseorang sebuah pekerjaan yang memiliki banyak kesalahan ejaan/tata bahasa, Anda akan mendapatkan umpan balik tentang tata bahasa/kesalahan ejaan alih-alih umpan balik yang lebih berharga tentang apakah tulisan yang Anda buat sudah sesuai dengan tujuan Anda.
- **Saat Anda meminta masukan dari orang lain, beri tahu pengulas:**
  - **apa yang sedang Anda coba lakukan**
  - **apa yang Anda takuti**
  - **seperti apa keseimbangan yang ingin Anda capai**
- **Ketika seseorang melaporkan masalah, hampir selalu memang ada masalah**, meskipun solusi yang mereka ajukan tidak tepat. Tetap ajukan pertanyaan lanjutan untuk mempelajari lebih lanjut.
- Orang perlu merasa aman untuk mengajukan pertanyaan saat berkontribusi/meninjau konten. Inilah cara Anda dapat melakukannya:
  - **Berterima kasih kepada orang-orang atas kontribusi/ulasan mereka, bahkan jika Anda merasa kesal.** Misalnya:
    - "Pertanyaan bagus!"
    - "Terima kasih telah meluangkan waktu untuk menjelaskan. 🙂"
    - "Ini sebenarnya disengaja, tapi terima kasih telah meluangkan waktu untuk berkontribusi. 😊"
  - **Dengarkan apa yang orang katakan dan ulangi jika Anda tidak yakin bahwa Anda memahaminya dengan benar.** Ini dapat membantu memvalidasi perasaan dan pengalaman orang, sekaligus juga memahami kalau _Anda_ memahami _mereka_ dengan benar.
  - **Gunakan banyak emoji yang positif dan berempati.** Lebih baik terlihat sedikit aneh daripada terlihat kasar atau tidak sabar.
  - **Komunikasikan aturan/batasan dengan ramah.** Jika seseorang berperilaku kasar/tidak pantas, tanggapi hanya dengan keramahan dan kedewasaan, tetapi juga jelaskan bahwa perilaku ini tidak dapat diterima dan apa yang akan terjadi (sesuai dengan kode perilaku) jika mereka terus berperilaku buruk.

### Tips, Info, Peringatan, dan Penyorotan Baris

Kami memiliki beberapa gaya khusus untuk menunjukkan sesuatu yang layak disorot dengan cara tertentu. Ini diambil [dari halaman ini](https://v3.vuejs.org/guide/doc-style-guide.html#alerts). **Gaya-gaya ini tidak boleh terlalu sering digunakan.**

Ada godaan tertentu untuk menyalahgunakan gaya ini, karena seseorang dapat dengan mudah menambahkan perubahan di dalam sebuah informasi. Namun, ini memecah aliran membaca pengguna, dan dengan demikian, hanya boleh digunakan dalam keadaan khusus. Sebisa mungkin, kita harus berusaha membuat narasi dan alur di dalam halaman untuk menghargai beban kognitif pembaca.

Dalam situasi apa pun, 2 peringatan tidak boleh digunakan berdampingan, itu menjadi tanda bahwa kita tidak bisa menjelaskan konteks dengan cukup baik.

### Berkontribusi

Kami menghargai PR (*Pull Request*) yang kecil dan terfokus. Jika Anda ingin membuat perubahan yang sangat besar, harap komunikasikan dengan anggota tim sebelum melakukan *pull request*. Berikut adalah [tulisan yang merinci mengapa ini sangat penting](https://www.netlify.com/blog/2020/03/31/how-to-scope-down-prs/) agar kami dapat bekerja dengan baik di tim ini. Harap dipahami bahwa meskipun kami selalu menghargai kontribusi, pada akhirnya kami harus memprioritaskan apa yang terbaik untuk proyek secara keseluruhan.

## Sumber 

### Perangkat Lunak

- [Grammarly](https://www.grammarly.com/): Aplikasi desktop dan ekstensi browser untuk memeriksa ejaan dan tata bahasa (meskipun pemeriksaan tata bahasa tidak menangkap semuanya dan terkadang menunjukkan kesalahan). **Khusus untuk yang berbahasa Inggris**.
- [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker): Sebuah ekstensi untuk Kode VS yang membantu Anda memeriksa ejaan dalam markdown dan contoh kode.

### Buku

- [On Writing Well](https://www.amazon.com/Writing-Well-30th-Anniversary-Nonfiction-ebook/dp/B0090RVGW0) (lihat [kutipan populer](https://www.goodreads.com/work/quotes/1139032-on-writing-well-the-classic-guide-to-writing-nonfiction))
- [Bird by Bird](https://www.amazon.com/Bird-Some-Instructions-Writing-Life/dp/0385480016) (lihat [kutipan populer](https://www.goodreads.com/work/quotes/841198-bird-by-bird-some-instructions-on-writing-and-life))
- [Cognitive Load Theory](https://www.amazon.com/Cognitive-Explorations-Instructional-Performance-Technologies/dp/144198125X/)
