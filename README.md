# Latihan: Setup Environment dan Hello World (Kotlin Multiplatform)

Dokumentasi ini berisi langkah-langkah instalasi environment, pembuatan proyek Kotlin Multiplatform (KMP), hingga pengubahan teks nama dan eksekusi pada target aplikasi.

---

## 1. Unduh Installer Android Studio
Mengunduh file installer resmi Android Studio (`android-studio-quail4-windows.exe`) dari situs resmi [developer.android.com](https://developer.android.com).

![1. Download Android Studio](PAM.1.1.png)

---

## 2. Instalasi Android Studio
Jalankan file `.exe` yang telah diunduh dan ikuti wizard instalasi hingga selesai (*Completing Android Studio Setup*).

![2. Setup Finished](PAM.1.2.png)

---

## 3. Instal Plugin Kotlin Multiplatform
Buka Android Studio, masuk ke menu **Plugins** > **Marketplace**, lalu cari dan instal plugin **Kotlin Multiplatform**.

![3. Install KMP Plugin](PAM.1.3.png)

---

## 4. Generate Proyek via Kotlin Multiplatform Wizard
Akses web [kmp.jetbrains.com](https://kmp.jetbrains.com/) untuk membuat template proyek baru dengan konfigurasi berikut:
* **Project Name**: `FirstKotlinProject`
* **Project ID**: `org.example.project`
* **Target Platform**: Android, iOS, Desktop

![4. KMP Wizard Setup](PAM.1.4.png)

---

## 5. Open Project & Sync Gradle
Ekstrak file proyek hasil download, lalu buka folder tersebut menggunakan Android Studio. Tunggu proses **Gradle Sync** dan indexing hingga selesai.

![5. Project Structure in Android Studio](PAM.1.5.png)

---

## 6. Modifikasi Teks Pesan Nama
Buka file `GreetingUtil.kt` (pada direktori `shared/src/commonMain/kotlin/org/example/project/`) dan ubah return value dari fungsi `sayHello` menjadi string nama Anda:

```kotlin
fun sayHello(to: String): String =
    "Hello, Galih Sigit Satrio!"
