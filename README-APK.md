# Build APK Absen Alert dengan GitHub Actions

1. Upload seluruh isi folder project ini ke root repository GitHub (jangan upload folder luarnya sebagai satu folder).
2. Pastikan `.github/workflows/android-apk.yml` ikut ter-upload.
3. Buka tab **Actions** → workflow **Build Absen Alert APK** → **Run workflow**. Build juga berjalan otomatis setiap push ke branch `main`.
4. Tunggu status workflow hijau.
5. Buka hasil run, bagian **Artifacts**, lalu download `Absen-Alert-APK`.
6. Ekstrak ZIP artifact dan install `app-debug.apk` di Android. Jika diminta, izinkan instalasi dari sumber tersebut.

Catatan: ini debug APK untuk uji coba/pribadi, bukan release bertanda tangan Play Store. Ini membungkus web app dengan Capacitor. Alarm ketika aplikasi ditutup/HP sleep belum dijamin; perlu integrasi native Android (AlarmManager dan notifikasi) untuk kebutuhan tersebut. Data tersimpan lokal.
