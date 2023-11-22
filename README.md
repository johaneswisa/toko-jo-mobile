# toko_jo

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

Johanes Wisanggeni<br>
2206032425<br>
PBP-F<br>

# Tugas 7 PBP

1. Apa perbedaan utama antara stateless dan stateful widget dalam konteks pengembangan aplikasi Flutter?<br>
Stateless widget adalah widget statis dimana seluruh konfigurasi yang dimuat didalamnya telah diinisiasi sejak awal. Sedangkan Stateful widget berlaku sebaliknya dimana sifatnya adalah dinamis, sehingga widget ini dapat diperbaharui kapanpun dibutuhkan berdasarkan user actions atau ketika terjadinya perubahan data. <br>
Sumber: https://daengweb.id/belajar-flutter-basic-6-stateless-stateful-widget#:~:text=Stateless%20widget%20adalah%20widget%20statis,atau%20ketika%20terjadinya%20perubahan%20data.<br>

2. Sebutkan seluruh widget yang kamu gunakan untuk menyelesaikan tugas ini dan jelaskan fungsinya masing-masing. <br>
MaterialApp: MaterialApp adalah widget yang berfungsi sebagai root widget dari aplikasi Flutter. Ia mengatur konfigurasi umum seperti tema, bahasa, dan navigasi. <br>
Scaffold: Scaffold adalah struktur dasar untuk mengatur tampilan aplikasi Anda. Ia menyediakan lapisan dasar seperti AppBar, body, dan floating action button (FAB).<br>
AppBar: AppBar adalah widget yang menyediakan bilah atas dalam tampilan aplikasi. Ia biasanya berisi judul aplikasi, tombol aksi, dan fungsi navigasi.<br>
SingleChildScrollView:  SingleChildScrollView adalah widget yang memungkinkan kontennya untuk di-scroll jika kontennya melebihi ruang yang tersedia.<br>
Padding: Padding adalah widget yang digunakan untuk menambahkan ruang putih (padding) di sekitar widget anaknya. Ini membantu mengatur tata letak elemen dalam aplikasi.<br>
Column:  Column adalah widget yang mengatur anak-anaknya dalam tata letak kolom vertikal. Ini berguna untuk menata konten dalam satu kolom.<br>
GridView.count: GridView.count adalah widget yang digunakan untuk menampilkan daftar item dalam bentuk grid dengan jumlah baris dan kolom yang tetap.<br>
Text: Text digunakan untuk menampilkan teks di aplikasi Anda. Anda dapat mengatur gaya teks, ukuran, dan warnanya.<br>
Material: Material adalah widget yang digunakan untuk membuat komponen berbasis Material Design, seperti tombol, kartu, dan dialog. Ini memastikan bahwa tampilan aplikasi Anda mengikuti pedoman desain Material Design.<br>
InkWell: InkWell adalah widget yang digunakan untuk membuat area yang dapat ditekan. Ia sering digunakan untuk menangani interaksi pengguna seperti ketika pengguna menyentuh atau mengetuk area.<br>
Container: Container adalah widget yang digunakan untuk mengelola tata letak dan dekorasi dari widget anaknya. Ia adalah wadah serbaguna yang dapat digunakan untuk mengatur tampilan dan mengubah properti seperti warna dan margin.<br>
Icon: Icon adalah widget yang digunakan untuk menampilkan ikon dalam aplikasi Anda. Ia berisi ikon yang sesuai dengan ikon Font Awesome atau Material Icons.<br>
SnackBar: SnackBar adalah widget yang digunakan untuk menampilkan pesan singkat kepada pengguna, biasanya sebagai umpan balik atas tindakan yang dilakukan oleh pengguna.<br>

3. Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step (bukan hanya sekadar mengikuti tutorial) <br>
Pertama-tama saya membuat program flutter baru dengan flutter create dan flutter run, lalu saya merapikan struktur proyek saya dengan memindahkan beberapa baris code dari main.dart ke menu.dart. Lalu saya mengubah tema warna aplikasi dengan colorScheme di main.dart, mengubah sifat widget halaman menu menjadi stateless (dengan mengubah pada bagian ({super.key, required this.title}) menjadi ({Key? key}) : super(key: key);, menghapus final String title; sampai bawah serta tambahkan Widget build, dan hapus fungsi State yang ada dibawah bagian stateless widget). Lalu saya menambahkan teks dan card untuk memperlihatkan barang yang dijual dengan dengan define tipe pada list, dibawah kode MyHomePage({Key? key}) : super(key: key); saya menambahkan barang-barang yang dijual (nama, harga, dan icon barang tersebut), menambahkan code di widget build (tampilan shop dll.) dan membuat widget stateless baru untuk menampilkan card (menyimpan icon dan text, SnackBar on click dll.). <br>
Sumber: https://pbp-fasilkom-ui.github.io/ganjil-2024/docs/tutorial-6#tutorial-getting-started-with-flutter

# Tugas 8 PBP

1. Jelaskan perbedaan antara Navigator.push() dan Navigator.pushReplacement(), disertai dengan contoh mengenai penggunaan kedua metode tersebut yang tepat!
Navigator.push(): Metode ini digunakan untuk menambahkan sebuah route baru ke dalam tumpukan (stack) route navigasi. Ketika Navigator.push() dipanggil, layar baru ditambahkan ke atas layar saat ini di dalam stack, sehingga pengguna dapat kembali ke layar sebelumnya dengan tombol "back" atau fungsi serupa. Navigator.pushReplacement(): Metode ini digunakan untuk menambahkan route baru ke dalam stack dan secara otomatis menghapus layar sebelumnya dari stack. Hal ini berarti bahwa ketika menggunakan Navigator.pushReplacement(), layar sebelumnya tidak dapat diakses lagi dari layar yang baru ditambahkan ke dalam stack. Contoh penggunaan keduanya: Navigator.push() untuk memunculkan form untuk mensubmit data diri kemudian bisa kembali ke layar utama, sedangkan Navigator.pushReplacement() untuk menggantikan halaman setelah register dengan halaman utama, user tidak kembali ke register page. 

2. Jelaskan masing-masing layout widget pada Flutter dan konteks penggunaannya masing-masing!
Container<br>
Konteks Penggunaan: Container adalah widget yang serbaguna dan dapat digunakan untuk menyesuaikan tata letak, dekorasi, padding, margin, dan transformasi dari child widget di dalamnya. Ini memungkinkan untuk membuat UI yang sangat disesuaikan dan fleksibel.

Column<br>
Konteks Penggunaan: Column adalah layout widget yang mengatur child widget dalam satu kolom vertikal. Cocok digunakan saat ingin menyusun widget secara vertikal seperti daftar, form, atau komponen lainnya.

Row<br>
Konteks Penggunaan: Row adalah layout widget yang mengatur child widget dalam satu baris horizontal. Sangat berguna untuk menyusun widget secara horizontal seperti tombol navigasi, ikon, atau elemen UI yang terletak berdampingan.

Stack<br>
Konteks Penggunaan: Stack adalah layout widget yang memungkinkan child widget untuk tumpang tindih (overlap). Widget diatur relatif terhadap satu sama lain dan berguna saat ingin menempatkan widget di atas atau di bawah widget lain secara bebas.

ListView<br>
Konteks Penggunaan: ListView adalah layout widget yang digunakan ketika ingin menampilkan daftar item yang dapat di-scroll. Berguna untuk membuat daftar yang panjang, seperti daftar pesan, daftar kontak, atau konten dengan banyak item.

GridView<br>
Konteks Penggunaan: GridView adalah layout widget yang digunakan untuk menampilkan daftar item dalam bentuk grid (kotak-kotak). Cocok digunakan untuk menampilkan koleksi item dalam grid, seperti galeri foto atau tata letak komponen yang berulang.

Wrap<br>
Konteks Penggunaan: Wrap adalah layout widget yang mengatur child widget dalam baris-baris horizontal atau kolom-kolom vertikal, memungkinkan child widget untuk melanjutkan ke baris/kolom berikutnya ketika mencapai batas lebar/tinggi yang ditentukan.

Expanded & Flexible<br>
Konteks Penggunaan: Expanded dan Flexible digunakan dalam Row, Column, atau Flex widget untuk memberikan child widget ruang yang fleksibel dalam pengaturan layout. Expanded mengisi ruang yang tersisa, sementara Flexible memberikan properti untuk mengatur fleksibilitas widget.

3. Sebutkan apa saja elemen input pada form yang kamu pakai pada tugas kali ini dan jelaskan mengapa kamu menggunakan elemen input tersebut!

Elemen input yang digunakan: TextFormField; TextFormField adalah widget di Flutter yang digunakan untuk membuat sebuah input field (kotak input) yang memungkinkan pengguna untuk memasukkan teks atau data lainnya. Digunakan untuk memungkinkan pengguna memasukkan data dan validasi.

4. Bagaimana penerapan clean architecture pada aplikasi Flutter?

Clean Architecture pada aplikasi Flutter mengikuti prinsip-prinsip desain arsitektur perangkat lunak yang membagi aplikasi menjadi beberapa lapisan dengan batasan-batasan tertentu. Clean Architecture memisahkan logika bisnis dari kode-kode infrastruktur, sehingga memudahkan pengujian, pemeliharaan, dan pengembangan aplikasi. penerapan Clean Architecture dapat dilakukan dengan mengorganisir kode ke dalam beberapa lapisan utama:
Domain Layer, deskripsi: Ini adalah lapisan teratas yang berisi logika bisnis, aturan, entitas, dan objek nilai dari aplikasi.
Repository Layer, deskripsi: Lapisan ini berfungsi sebagai penghubung antara domain layer dan lapisan data.
Data Source Layer, deskripsi: Berisi implementasi spesifik terhadap sumber data eksternal seperti API services, database, local storage, dll.
Presentation Layer, deskripsi: Lapisan ini berfungsi untuk menangani tampilan dan interaksi pengguna.

5. Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step! (bukan hanya sekadar mengikuti tutorial)

Saya membuat class leftDrawer pada left_drawer.dart yang memiliki button untuk ke main page, dan tambah item yang ditambahkan fungsi navigator.push() ketika tombol ditekan, lalu leftDrawer tersebut dipasang ke menu dan halaman form untuk navigasi. Setelah itu, saya membuat file shoplist_form.dart yang berisi class stateful yang menerima input dari user dengan menggunakan TextFormField yang akan dilakukan validasi input ketika tombol save ditekan,  Setelah itu saya melakukan refactoring dengan memindahkan file-file ke folder screens dan widgets.

# Tugas 9 PBP
1. Apakah bisa kita melakukan pengambilan data JSON tanpa membuat model terlebih dahulu? Jika iya, apakah hal tersebut lebih baik daripada membuat model sebelum melakukan pengambilan data JSON?<br>
2. Jelaskan fungsi dari CookieRequest dan jelaskan mengapa instance CookieRequest perlu untuk dibagikan ke semua komponen di aplikasi Flutter.<br>
3. Jelaskan mekanisme pengambilan data dari JSON hingga dapat ditampilkan pada Flutter.<br>
4. Jelaskan mekanisme autentikasi dari input data akun pada Flutter ke Django hingga selesainya proses autentikasi oleh Django dan tampilnya menu pada Flutter.<br>
5. Sebutkan seluruh widget yang kamu pakai pada tugas ini dan jelaskan fungsinya masing-masing.<br>
6. Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step! (bukan hanya sekadar mengikuti tutorial).<br>

Jawaban:
1. Ya, kita bisa memasukkan data-data JSON ke dalam map atau list. Tetapi kita kehilangan kejelasan dan tipe yang didefinisikan dengan baik. Membutuhkan perhatian ekstra untuk mengelola dan memproses data.<br>

2. Objek http.Cookie dalam Flutter digunakan untuk merepresentasikan atau memanipulasi cookie HTTP. Cookie ini dapat digunakan dalam permintaan HTTP untuk mengelola informasi otentikasi, sesi, atau data lainnya yang dapat disimpan pada sisi klien.

Adapun alasan mengapa instance http.Cookie atau objek serupa perlu dibagikan ke semua komponen di aplikasi Flutter terkait dengan pengaturan dan manajemen cookie yang terkait dengan permintaan HTTP yang dilakukan dari berbagai komponen.<br>

3. Pengambilan Data JSON: Ambil data dari sumber JSON seperti API atau file lokal dalam format JSON. <br>
Konversi Data JSON ke Objek Dart: Gunakan fungsi jsonDecode() dari paket dart:convert untuk mengubah string JSON menjadi objek Dart seperti Map atau List.<br>
Gunakan Data dalam Aplikasi Flutter: Gunakan objek Dart yang dihasilkan dari data JSON untuk menampilkan informasi di dalam widget Flutter seperti Text, ListView, GridView, atau widget lainnya sesuai kebutuhan. <br>

4.Input Data Akun di Flutter: Pengguna memasukkan informasi login (nama pengguna dan kata sandi) dalam aplikasi Flutter.<br>
Permintaan Autentikasi ke Django: Aplikasi Flutter mengirimkan permintaan HTTP ke backend Django dengan informasi login.<br>
Penanganan Permintaan di Django: Django memproses informasi login, menggunakan fungsi autentikasi seperti authenticate() dan login().<br>
Tanggapan dari Django: Django memberikan respons ke Flutter berdasarkan hasil autentikasi, menyampaikan keberhasilan atau kegagalan login.<br>
Penanganan Respons di Flutter: Berdasarkan respons Django, Flutter menavigasi pengguna ke menu jika login berhasil atau menampilkan pesan kesalahan jika gagal<br>

5. SizedBox Widget: Memberikan jarak antara widget TextField username dan password<br>
TextField Widget: Menerima input username dan password untuk autentikasi<br>
ElevatedButton Widget: Melakukan submission pada autentikasi dan saat melakukan create item dengan django<br>

6. Saya membuat aplikasi authentication pada aplikasi django, lalu menambahkan function berdecorator @csrf_exempt di views.py untuk melakukan login dan logout yang memberikan response JSON, lalu pada app flutter saya membuat halaman login, lalu di app flutter saya membuat sebuah model item yang digunakan untuk fetch data dari web service django. Tombol lihat item saya buat agar memiliki fungsionalitas untuk menampilkan data-data dari response web service django, tombol logout saya beri fungsionalitas untuk melakukan logout dengan menggunakan function  logout yang ada di views.py app authentication (app django). Dependencies yang diperlukan yaitu django-cors-headers, pbp_django_auth, http, provider.


