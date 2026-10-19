# Paket Android Asset Management

Paket ini mengubah aplikasi HTML menjadi proyek Android menggunakan Capacitor.

## Cara cepat melalui GitHub
1. Buat repository GitHub baru.
2. Ekstrak ZIP lalu unggah seluruh isi folder ini ke repository.
3. Buka tab **Actions** > **Build Android APK** > **Run workflow**.
4. Setelah selesai, buka hasil workflow dan unduh artifact **Asset-Management-debug-apk**.
5. Ekstrak artifact, lalu instal `app-debug.apk` pada handphone Android.

## Cara melalui Android Studio
Syarat: Node.js, JDK, dan Android Studio.

```bash
npm install
npx cap add android
npx cap sync android
npx cap open android
```

Di Android Studio pilih **Build > Build APK(s)**.

## Setiap kali HTML diperbarui
Ganti `www/index.html`, kemudian jalankan:

```bash
npx cap sync android
```

## Izin Android
Paket meminta izin kamera dan lokasi. Periksa izin aplikasi melalui Pengaturan Android jika kamera atau GPS tidak berjalan.

## Identitas aplikasi
- Nama: Asset Management
- Package ID: com.hartono.assetmanagement
- Minimum Android mengikuti versi Capacitor yang digunakan.
