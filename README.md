# MitigasiKita: Sistem Peringatan Dini Gempa & Tsunami Berbasis Web

![MitigasiKita Logo](logo-app.png)

MitigasiKita adalah sebuah sistem peringatan dini berbasis web yang dirancang untuk meningkatkan kesiapsiagaan masyarakat Indonesia terhadap risiko bencana gempa bumi dan tsunami. Proyek ini dikembangkan oleh tim CC25-CF278 dalam program Capstone Project Coding Camp 2025 dengan dukungan dari Dicoding dan DBS Foundation.

## Tautan Penting
- **Aplikasi Langsung (Live Demo):** [https://mitigasikita-application.vercel.app/](https://mitigasikita-application.vercel.app/)

## Daftar Isi
- [Latar Belakang]
- [Fitur Utama]
- [Arsitektur dan Tumpukan Teknologi]
- [Cara Menggunakan Aplikasi]
- [Tautan Deployment & Repositori]
- [Tim Pengembang (CC25-CF278)]
- [Ucapan Terima Kasih]

## Latar Belakang
Indonesia, yang terletak di wilayah Cincin Api Pasifik, menghadapi tantangan besar terkait bencana gempa bumi dan tsunami. Seringkali, informasi peringatan dini yang ada bersifat umum dan kurang spesifik terhadap lokasi pengguna. MitigasiKita hadir untuk menjembatani kesenjangan ini dengan menyediakan prediksi risiko real-time yang diolah menggunakan teknologi Machine Learning berdasarkan lokasi spesifik pengguna.

## Fitur Utama
- 📈 **Prediksi Risiko Real-Time:** Menghasilkan tingkat risiko gempa dan tsunami (Aman, Waspada, Berbahaya) lengkap dengan confidence level dari model Machine Learning.
- 🗺️ **Peta Interaktif:** Memungkinkan pengguna memilih lokasi prediksi melalui daftar kota yang tersedia.
- 📚 **Edukasi Bencana:** Menyediakan panduan praktis dan informatif mengenai kesiapsiagaan sebelum, saat, dan setelah gempa bumi serta tsunami.
- 👤 **Akun Pengguna Personal:** Memberikan manfaat personalisasi, termasuk penyimpanan riwayat prediksi untuk analisis risiko jangka panjang di lokasi yang sering dipantau.
- 📱 **Antarmuka Responsif:** Desain yang dioptimalkan untuk pengalaman pengguna yang mulus di berbagai perangkat, mulai dari desktop hingga mobile.
- ⚡ **Progressive Web App (PWA):** Aplikasi dapat diakses dengan fungsionalitas terbatas bahkan dalam kondisi offline, memastikan informasi penting tetap tersedia saat dibutuhkan.

## Arsitektur dan Tumpukan Teknologi
Proyek ini dibangun dengan pendekatan lintas disiplin yang mengintegrasikan Machine Learning, Frontend, dan Backend.

### 🤖 Machine Learning
- **Arsitektur Model:** Deep Neural Network (DNN) dibangun menggunakan TensorFlow dan Keras untuk klasifikasi risiko.
- **Pipeline Data:** Data geologi dan cuaca dari BMKG dan Open-Meteo diproses melalui cleaning, imputasi, dan normalisasi.
- **Deployment Model:** Model .tflite di-deploy sebagai RESTful API untuk inferensi cepat.

### 🖥️ Frontend
- **Framework:** React.js dengan module bundler Vite.
- **Styling:** Tailwind CSS untuk desain yang modern dan responsif.
- **Progressive Web App (PWA):** Memenuhi semua karakteristik wajib PWA untuk memberikan pengalaman penggunaan aplikasi native, termasuk fungsionalitas saat koneksi terbatas.

### ⚙️ Backend
- **Framework:** Express.js dengan bahasa pemrograman TypeScript.
- **Arsitektur:** Layered Architecture untuk kode yang terstruktur dan mudah dikelola.
- **Database & ORM:** Menggunakan Prisma Client sebagai Object Relational Mapping (ORM) yang terhubung ke database.

## Cara Menggunakan Aplikasi
1. **Akses Aplikasi:** Buka [https://mitigasikita-application.vercel.app/](https://mitigasikita-application.vercel.app/) melalui browser modern seperti Google Chrome atau Firefox.
2. **Dapatkan Prediksi Risiko:**
   - Navigasi ke halaman Peta Risiko.
   - Pilih lokasi Anda dari daftar dropdown atau masukkan nama kota.
   - Klik tombol "Prediksi".
   - Hasil prediksi, termasuk status, magnitudo gempa, potensi tsunami, dan cuaca akan ditampilkan.
3. **Simpan Riwayat (Perlu Akun):**
   - Daftar atau Login ke akun Anda.
   - Setelah mendapatkan hasil prediksi, klik "Simpan ke Riwayat".
   - Akses semua riwayat prediksi Anda melalui menu "Riwayat" untuk memantau pola risiko.

## Tautan Deployment & Repositori
- **Aplikasi Frontend:** [https://mitigasikita-application.vercel.app/](https://mitigasikita-application.vercel.app/)
- **API Backend:** [https://mitigasi-kita-app-backend-production.up.railway.app/](https://mitigasi-kita-app-backend-production.up.railway.app/)
- **API Model ML:** [https://earthquake-tsunami-model-api-production.up.railway.app/](https://earthquake-tsunami-model-api-production.up.railway.app/)
- **Repositori GitHub:**
  - Frontend (React.js): [https://github.com/lizia20/mitigasi-kita](https://github.com/lizia20/mitigasi-kita)
  - Backend (Node.js): [https://github.com/zainalsaputra/mitigasi-kita-app-backend](https://github.com/zainalsaputra/mitigasi-kita-app-backend)
  - Machine Learning (Notebook): [https://github.com/CCoupse/mitigasi-kita-machine-learning](https://github.com/CCoupse/mitigasi-kita-machine-learning)
  - Model API: [https://github.com/zainalsaputra/earthquake-tsunami-model-api](https://github.com/zainalsaputra/earthquake-tsunami-model-api)

## Tim Pengembang (CC25-CF278)
### Machine Learning (ML)
- Dearmawan - Universitas Mikroskil
- Julianti - Universitas Mikroskil
- Zainal Saputra - Institut Teknologi Sains dan Kesehatan RS dr Soepraoen

### Frontend & Backend (FEBE)
- Puput Purwaningsih - Universitas Nurdin Hamzah
- Aprilia Nurhaliza - Universitas Pendidikan Indonesia
- Andres Junika Putra - Universitas Mercu Buana Yogyakarta

## Ucapan Terima Kasih
Kami mengucapkan terima kasih yang tulus kepada para mentor kami, Ibu Indriati dan Bapak Andika Renda Pribadi, serta kepada Dicoding dan DBS Foundation atas semua dukungan, bimbingan, dan kesempatan yang diberikan selama pengembangan proyek ini.
