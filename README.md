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


