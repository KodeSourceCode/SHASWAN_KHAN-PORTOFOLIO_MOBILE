# Portofolio

## 1. Perkenalan

- **Vue**: library frontend untuk membuat antarmuka interaktif dengan komponen.
- **Vite**: build tool dan dev server yang sangat cepat untuk proyek modern (termasuk Vue).
- **Capacitor**: bridge yang mengubah aplikasi web menjadi aplikasi mobile (Android/iOS).

## 2. Progres Harian

- Hari 1 — fokus: instalasi Vue + Vite, lalu praktek bongkar-pasang komponen di `src/components`.

```sh
npm create vue@latest
cd <project-name>
npm install
npm run dev
```

- Hari 2 — fokus: perubahan `src/App.vue`, penggunaan vue router, dan instalasi tailwind.

```sh
npm install tailwindcss @tailwindcss/vite
```

- Hari 3 — fokus:

* Menggunakan tailwind
* Menggunakan komponen dengan memanfaatkan props dan slot
* Memanfaatkan asset di folder `/public`
* Melengkapi isi `src/views`

- Hari 4 — fokus:

* Menginstall jdk26
* Instalasi capacitor
* Konfigurasi opsi pengembang lalu Koneksi adb
* Membangun android app menggunakan capacitor

```sh
npm install @capacitor/core @capacitor/android
npx cap init
npx cap add android
npx cap sync android
npx cap run android
```

## 3. Catatan

- Jalankan `npm run dev` lalu buka alamat dev server di browser untuk melihat progres.

- Install Capacitor CLI sekali saja di laptop

```sh
npm i -g @capacitor/cli
```

- Kalau pakai nirkabel pastikan berada di jaringan yang sama, Pastikan ip dan port tidak typo

```sh
adb connect <IP_HP>:<PORT_HP>
adb devices
```

- Selalu jalankan `npx cap sync android` setiap kali melakukan build web sebelum `npx cap run android`.
