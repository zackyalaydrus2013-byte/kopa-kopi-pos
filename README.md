# Kopa Kopi POS 1.0 (Android project)

Project Android Studio berbasis Kotlin + WebView dengan antarmuka POS lokal.

## Fitur prototipe
- Menu dan harga Kopa Kopi sesuai daftar yang diberikan.
- Keranjang dan jumlah gelas.
- Pengaturan gula/es per transaksi (berlaku untuk semua item dalam versi awal).
- Metode pembayaran tunai/QRIS/transfer dan hitung kembalian tunai.
- Simpan riwayat transaksi dan rekap omzet harian di penyimpanan lokal WebView.
- Membuat teks label terpisah untuk setiap gelas, nota, dan tiket barista.
- Tombol berbagi membuka Android share sheet; pilih Fun Print jika aplikasi itu muncul sebagai tujuan yang kompatibel.

## Membuat APK
1. Instal Android Studio pada komputer.
2. Ekstrak ZIP ini.
3. Android Studio > Open > pilih folder `kopa-kopi-pos`.
4. Tunggu Gradle Sync dan instal Android SDK Platform 35 jika diminta.
5. Pilih Build > Build Bundle(s) / APK(s) > Build APK(s).
6. APK debug akan berada di `app/build/outputs/apk/debug/app-debug.apk`.

## Batasan yang belum selesai
- APK belum dibangun/ditandatangani di lingkungan ini karena Android SDK/Gradle tidak tersedia.
- Pengiriman teks melalui Android share sheet sudah disiapkan, tetapi Fun Print/C19 harus diuji di perangkat; tidak ada klaim bahwa pencetakan langsung Bluetooth sudah terintegrasi.
- Label saat ini disiapkan sebagai teks. Ukuran, font, pemotongan, dan layout harus diuji dengan kertas C19.
- Data lokal tersimpan di perangkat. Belum ada sinkronisasi cloud/multi-perangkat, backup, pengelolaan stok, atau pembatalan/refund.
- Versi awal memakai satu set pengaturan gula/es untuk seluruh transaksi; pilihan per gelas akan ditambahkan pada iterasi berikutnya.

## Catatan
Harga menu dan nama varian mengikuti informasi pengguna. Uji transaksi terlebih dahulu sebelum dipakai untuk operasional/keuangan sebenarnya.
