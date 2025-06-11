# **MitigasiKita: Sistem Peringatan Dini Gempa & Tsunami Berbasis Web**

![MitigasiKita Logo](https://raw.githubusercontent.com/lizia20/mitigasi-kita/main/src/assets/logo.png)

[cite_start]**MitigasiKita** adalah sebuah sistem peringatan dini berbasis web yang dirancang untuk meningkatkan kesiapsiagaan masyarakat Indonesia terhadap risiko bencana gempa bumi dan tsunami. [cite_start]Proyek ini dikembangkan oleh tim **CC25-CF278** dalam program Capstone Project Coding Camp 2025 dengan dukungan dari Dicoding dan DBS Foundation.

[![Project Status](https://img.shields.io/badge/status-100%25%20Selesai-brightgreen)](#)
[![Deployment](https://img.shields.io/badge/deployment-Vercel%20%26%20Railway-blue)](#tautan-deployment--repositori)
[![Technology](https://img.shields.io/badge/technology-PWA%20%7C%20React%20%7C%20Node.js-informational)](#arsitektur-dan-tumpukan-teknologi)

---

### **Tautan Penting**

- **[Aplikasi Langsung (Live Demo)](https://mitigasikita-application.vercel.app/)**
- **[Presentasi Video (10 Menit)](https://www.youtube.com/watch?v=your-video-link)**

---

### **Daftar Isi**

1.  [Latar Belakang](#latar-belakang)
2.  [Fitur Utama](#fitur-utama)
3.  [Arsitektur dan Tumpukan Teknologi](#arsitektur-dan-tumpukan-teknologi)
4.  [Cara Menggunakan Aplikasi](#cara-menggunakan-aplikasi)
5.  [Tautan Deployment & Repositori](#tautan-deployment--repositori)
6.  [Tim Pengembang](#tim-pengembang)
7.  [Ucapan Terima Kasih](#ucapan-terima-kasih)

---

### **Latar Belakang**

[cite_start]Indonesia, yang terletak di wilayah Cincin Api Pasifik, menghadapi tantangan besar terkait bencana gempa bumi dan tsunami. [cite_start]Seringkali, informasi peringatan dini yang ada bersifat umum dan kurang spesifik terhadap lokasi pengguna. [cite_start]MitigasiKita hadir untuk menjembatani kesenjangan ini dengan menyediakan prediksi risiko *real-time* yang diolah menggunakan teknologi *Machine Learning* berdasarkan lokasi spesifik pengguna.

### **Fitur Utama**

* [cite_start]**📈 Prediksi Risiko Real-Time**: Menghasilkan tingkat risiko gempa dan tsunami (Aman, Waspada, Berbahaya) lengkap dengan *confidence level* dari model *Machine Learning*.
* [cite_start]**🗺️ Peta Interaktif**: Memungkinkan pengguna memilih lokasi prediksi melalui daftar kota yang tersedia.
* [cite_start]**📚 Edukasi Bencana**: Menyediakan panduan praktis dan informatif mengenai kesiapsiagaan sebelum, saat, dan setelah gempa bumi serta tsunami.
* [cite_start]**👤 Akun Pengguna Personal**: Memberikan manfaat personalisasi, termasuk penyimpanan riwayat prediksi untuk analisis risiko jangka panjang di lokasi yang sering dipantau.
* [cite_start]**📱 Antarmuka Responsif**: Desain yang dioptimalkan untuk pengalaman pengguna yang mulus di berbagai perangkat, mulai dari desktop hingga *mobile*.
* [cite_start]**⚡ Progressive Web App (PWA)**: Aplikasi dapat diakses dengan fungsionalitas terbatas bahkan dalam kondisi offline, memastikan informasi penting tetap tersedia saat dibutuhkan.

### **Arsitektur dan Tumpukan Teknologi**

Proyek ini dibangun dengan pendekatan lintas disiplin yang mengintegrasikan *Machine Learning*, *Frontend*, dan *Backend*.

* **🤖 Machine Learning**
    * [cite_start]**Arsitektur Model**: *Deep Neural Network* (DNN) dibangun menggunakan TensorFlow dan Keras untuk klasifikasi risiko.
    * [cite_start]**Pipeline Data**: Data geologi dan cuaca dari BMKG dan Open-Meteo diproses melalui *cleaning*, imputasi, dan normalisasi.
    * [cite_start]**Deployment Model**: Model `.tflite` di-deploy sebagai RESTful API untuk inferensi cepat.

* **🖥️ Frontend**
    * [cite_start]**Framework**: React.js dengan *module bundler* Vite.
    * [cite_start]**Styling**: Tailwind CSS untuk desain yang modern dan responsif.
    * [cite_start]**Progressive Web App (PWA)**: Memenuhi semua karakteristik wajib PWA untuk memberikan pengalaman penggunaan aplikasi native, termasuk fungsionalitas saat koneksi terbatas.

* **⚙️ Backend**
    * [cite_start]**Framework**: Express.js dengan bahasa pemrograman TypeScript.
    * [cite_start]**Arsitektur**: *Layered Architecture* untuk kode yang terstruktur dan mudah dikelola.
    * [cite_start]**Database & ORM**: Menggunakan Prisma Client sebagai *Object Relational Mapping* (ORM) yang terhubung ke database.

### **Cara Menggunakan Aplikasi**

1.  [cite_start]**Akses Aplikasi**: Buka [https://mitigasikita-application.vercel.app/](https://mitigasikita-application.vercel.app/) melalui browser modern seperti Google Chrome atau Firefox.
2.  **Dapatkan Prediksi Risiko**:
    * [cite_start]Navigasi ke halaman **Peta Risiko**.
    * [cite_start]Pilih lokasi Anda dari daftar *dropdown* atau masukkan nama kota.
    * [cite_start]Klik tombol **"Prediksi"**.
    * [cite_start]Hasil prediksi, termasuk status, magnitudo gempa, potensi tsunami, dan cuaca akan ditampilkan.
3.  **Simpan Riwayat (Perlu Akun)**:
    * [cite_start]Daftar atau *Login* ke akun Anda.
    * [cite_start]Setelah mendapatkan hasil prediksi, klik **"Simpan ke Riwayat"**.
    * [cite_start]Akses semua riwayat prediksi Anda melalui menu **"Riwayat"** untuk memantau pola risiko.

### **Tautan Deployment & Repositori**

* **Aplikasi Frontend**: [https://mitigasikita-application.vercel.app/](https://mitigasikita-application.vercel.app/)
* **API Backend**: [https://mitigasi-kita-app-backend-production.up.railway.app/](https://mitigasi-kita-app-backend-production.up.railway.app/)
* **API Model ML**: [https://earthquake-tsunami-model-api-production.up.railway.app/](https://earthquake-tsunami-model-api-production.up.railway.app/)
<br>

* **Repositori GitHub**:
    * [Frontend (React.js)](https://github.com/lizia20/mitigasi-kita)
    * [Backend (Node.js)](https://github.com/zainalsaputra/mitigasi-kita-app-backend)
    * [Machine Learning (Notebook)](https://github.com/CCoupse/mitigasi-kita-machine-learning)
    * [Model API](https://github.com/zainalsaputra/earthquake-tsunami-model-api)

---

### **Tim Pengembang (CC25-CF278)**
[cite_start][cite: 77]
* **Machine Learning (ML)**
    * Dearmawan - Universitas Mikroskil
    * Julianti - Universitas Mikroskil
    * Zainal Saputra - Institut Teknologi Sains dan Kesehatan RS dr Soepraoen
* **Frontend & Backend (FEBE)**
    * Puput Purwaningsih - Universitas Nurdin Hamzah
    * Aprilia Nurhaliza - Universitas Pendidikan Indonesia
    * Andres Junika Putra - Universitas Mercu Buana Yogyakarta

### **Ucapan Terima Kasih**

[cite_start]Kami mengucapkan terima kasih yang tulus kepada para mentor kami, **Ibu Indriati** dan **Bapak Andika Renda Pribadi** [cite: 146, 149][cite_start], serta kepada **Dicoding** dan **DBS Foundation** atas semua dukungan, bimbingan, dan kesempatan yang diberikan selama pengembangan proyek ini.
