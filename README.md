# NyiurCare Releases

Repositori rilis publik untuk pembaruan otomatis aplikasi Android **NyiurCare** dari menu **Tentang Aplikasi → Versi Aplikasi**.

## Cara Menerbitkan Pembaruan Baru

1. Bangun file APK rilis dari proyek utama aplikasi NyiurCare, misalnya:
   `flutter build apk --release --target-platform android-arm64 --split-debug-info=build/symbols --build-name=1.0.3 --build-number=4038`
2. Ganti nama hasil build menjadi `NyiurCare-1.0.3.apk`.
3. Buka tab **Releases → Draft a new release** di repositori ini:
   - Isi tag versi, misalnya `v1.0.3` atau `v1.0.3+4038`.
   - Tulis catatan perubahan di kolom deskripsi rilis. Tambahkan `[wajib]` di awal catatan bila pengguna wajib memperbarui aplikasi.
   - Lampirkan file `.apk` pada rilis tersebut lalu klik **Publish release**.
4. Perbarui nilai `version_name`, `version_code`, `apk_url`, dan `changelog` pada [latest.json](latest.json) bila perlu agar cadangan manifest tetap sinkron dengan rilis terbaru.
