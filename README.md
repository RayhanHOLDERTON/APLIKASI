GlobalPulse 🌐

Aplikasi berita internasional berbasis Android yang menyajikan berita global terkini lengkap dengan asisten AI bernama MIKA (Media Informasi Kecerdasan Artificial) untuk membantu pengguna memahami berita dunia.


Fitur Utama


Berita Internasional — Menampilkan berita dan artikel dari berbagai penjuru dunia, dikelompokkan per kategori.
Kalender Ekonomi — Menyajikan jadwal dan data peristiwa ekonomi global.
MIKA AI Assistant — Asisten berita berbasis AI (Google Gemini 2.5 Flash) yang dapat menjawab pertanyaan seputar berita internasional, konflik global, dan analisis ekonomi dalam Bahasa Indonesia.
Detail Berita — Halaman detail untuk membaca artikel secara lengkap.



Teknologi yang Digunakan

KomponenTeknologiBahasaKotlinPlatformAndroid (Native)AI EngineGoogle Gemini 2.5 Flash APINetworkingRetrofit2 + OkHttp3AsyncKotlin CoroutinesUIAndroidX + Material Design


Struktur Aplikasi

com.example.globalpulse
├── SplashActivity       # Layar splash saat aplikasi pertama dibuka
├── MainActivity         # Layar utama dengan daftar berita & kategori
├── DetailActivity       # Halaman detail artikel berita
└── AiActivity           # Halaman chat dengan asisten AI MIKA

Fragments:


HomeFragment — Beranda dengan feed berita terkini
CategoryFragment — Berita berdasarkan kategori
EconomicCalendarFragment — Kalender dan peristiwa ekonomi global



Informasi APK

AtributNilaiPackage Namecom.example.globalpulseVersi1.0 (build 1)Min AndroidAndroid 7.0 (API 24)Target AndroidAndroid 14 (API 34)Compile SDKAndroid 14 (API 34)


Izin Aplikasi

IzinKeteranganINTERNETDiperlukan untuk mengambil data berita dan menghubungi API Gemini


Cara Instalasi (Sideload APK)


Aktifkan "Install from Unknown Sources" di pengaturan Android Anda:

Buka Pengaturan → Keamanan → Instal Aplikasi Tidak Dikenal



Transfer file base_APK.apk ke perangkat Android Anda.
Buka file manager, temukan file APK, lalu ketuk untuk menginstal.
Ikuti petunjuk instalasi di layar.



Catatan: APK ini ditandai sebagai debug build. Untuk distribusi publik, gunakan release build yang telah ditandatangani.




Konfigurasi API Key

Asisten AI MIKA menggunakan Google Gemini API. API key dikonfigurasi di dalam file asset assets/mika_ai.html:

javascriptconst API_KEY = 'YOUR_GEMINI_API_KEY_HERE';

Ganti nilai tersebut dengan API key Anda sendiri yang didapat dari Google AI Studio.


⚠️ Perhatian Keamanan: Jangan menyematkan API key langsung di dalam kode atau aset untuk aplikasi produksi. Gunakan backend server sebagai proxy untuk melindungi key Anda.




Persyaratan Sistem


Android 7.0 (Nougat) atau lebih baru
Koneksi internet aktif
Ruang penyimpanan minimal ~15 MB



Lisensi

Proyek ini dikembangkan sebagai aplikasi contoh (com.example). Hak cipta disesuaikan dengan kebijakan pengembang.
