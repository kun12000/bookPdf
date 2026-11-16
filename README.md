# Buku PDF (Android)

## Cara paling mudah: build otomatis di GitHub (tanpa Android Studio)
1. Buat repository baru di GitHub, lalu unggah seluruh isi folder ini (termasuk folder .github).
2. Buka tab Actions, tunggu workflow "Build APK" selesai (sekitar 5-8 menit).
3. Buka hasil run tersebut, unduh artifact "buku-pdf-apk", ekstrak, dan kirim app-debug.apk ke ponsel.
4. Di Android, izinkan "Instal dari sumber tidak dikenal", lalu buka berkasnya.

## Build lokal (butuh Node 18+, JDK 17, Android SDK)
npm install
npx cap add android
npx cap sync android
cd android && ./gradlew assembleDebug
APK: android/app/build/outputs/apk/debug/app-debug.apk
"# bookPdf" 
