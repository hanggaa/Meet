# Syarat dan Ketentuan Fasilitas Kredit Fintech1000s

**Versi:** 2.0.0
**Tanggal Pembaruan Terakhir:** 10 April 2026

Selamat datang di layanan Fintech1000s. Dengan menyetujui dokumen ini, Anda ("Merchant") sepakat untuk mengaktifkan fasilitas kredit yang dikelola oleh Selling Agent ("SA") melalui platform PT. Mitra Seribu Saudara ("PT. MSS"). Harap membaca ketentuan berikut dengan saksama sebelum melanjutkan.

---

### 1. Definisi Fasilitas
* **Fintech1000s**: Fitur restrukturisasi tagihan di dalam ekosistem Mitra1000s yang memungkinkan Merchant mengubah invoice reguler (prefix `INV-`) menjadi invoice pembiayaan dengan perpanjangan tempo (prefix `FIN-`).
* **Limit Kredit**: Batas fasilitas kredit yang diberikan oleh Selling Agent kepada Merchant untuk digunakan dalam pengajuan perpanjangan tempo.
* **Masa Perpanjangan**: Jangka waktu tambahan yang diberikan untuk pelunasan, yakni maksimal 56 hari (8 minggu) yang dihitung mulai dari tanggal jatuh tempo terakhir invoice reguler (`INV-`) yang direstrukturisasi menjadi invoice `FIN-`, bukan dari tanggal persetujuan pengajuan perpanjangan tempo.

### 2. Pemberian Limit dan Pengajuan
* Pemberian, perubahan, serta pembatalan limit kredit merupakan wewenang penuh Selling Agent yang menangani wilayah Merchant terkait.
* Pengajuan perpanjangan tempo hanya dapat dilakukan jika nilai total invoice tidak melebihi sisa limit kredit aktif Merchant.
* Jika nilai invoice melebihi limit, Merchant wajib menutup selisih tersebut terlebih dahulu melalui mekanisme cicilan pokok sebelum perpanjangan dapat diproses oleh sistem.
* Invoice dengan prefix `FIN-` bersifat final untuk restrukturisasi terkait dan tidak dapat diajukan perpanjangan tempo kembali.

### 3. Bunga dan/atau Biaya Layanan
* Penggunaan fasilitas kredit Fintech1000s dapat dikenakan bunga dan/atau biaya layanan sesuai kebijakan yang berlaku.
* Besaran, dasar perhitungan, dan waktu pembebanan bunga dan/atau biaya layanan akan diinformasikan kepada Merchant melalui sistem pada saat pengajuan, persetujuan, dan/atau selama masa tagihan berjalan.
* Bunga dan/atau biaya layanan yang telah timbul menjadi bagian dari kewajiban pembayaran Merchant sampai kewajiban dinyatakan lunas oleh sistem.
* Bunga dan/atau biaya layanan tetap dapat berjalan sesuai ketentuan produk yang berlaku meskipun tagihan telah melewati batas waktu 56 hari atau berstatus NPL (*Non-Performing Loan*).

### 4. Mekanisme Pembayaran (Cart Billing)
* Merchant wajib melakukan pembayaran melalui sistem **Cart Billing**, yang memungkinkan pemilihan satu atau lebih invoice `FIN-` dalam satu sesi transaksi.
* Setiap pembayaran menggunakan satu kode billing agregat dengan format `BILL-{merchant_id}-{timestamp}` melalui metode Virtual Account (VA) yang tersedia.
* Dalam satu sesi Cart Billing, Merchant dapat memilih aksi yang berbeda untuk setiap invoice `FIN-`, termasuk:
  * **Cicil Pokok**, yaitu Merchant mengisi nominal cicilan pokok sesuai kebutuhan Merchant; dan/atau
  * **Lunasi Tagihan**, yaitu Merchant melunasi seluruh kewajiban pada invoice terkait sesuai nominal yang ditampilkan sistem.
* Setelah Merchant memilih invoice, menentukan aksi pembayaran, membuat billing, memilih metode pembayaran, dan menyelesaikan pembayaran melalui Virtual Account (VA), sistem akan melakukan validasi dan verifikasi pembayaran.
* Setelah pembayaran tervalidasi, sistem akan mengeksekusi hasil pembayaran sesuai aksi yang dipilih Merchant pada masing-masing invoice, termasuk:
  * mengurangi sisa pokok pada invoice yang dipilih dengan aksi **Cicil Pokok**; dan/atau
  * mengubah status invoice menjadi **PAID** pada invoice yang dipilih dengan aksi **Lunasi Tagihan**.
* Merchant memahami bahwa rincian kewajiban pembayaran yang ditampilkan sistem dapat terdiri dari pokok, bunga, dan/atau komponen biaya lainnya sesuai ketentuan yang berlaku pada masing-masing invoice.

### 5. Konsekuensi Keterlambatan (Wanprestasi)
* Batas maksimal pelunasan seluruh kewajiban adalah H+56 sejak tanggal persetujuan perpanjangan tempo.
* Apabila pada hari ke-57 (H+57) invoice belum lunas, sistem secara otomatis melakukan blokir transaksi pada akun Mitra1000s Merchant sehingga tidak dapat melakukan pemesanan barang baru.
* Status tagihan akan berubah menjadi **Credit Default / NPL** dan akan diekskalasi kepada Selling Agent terkait untuk proses penagihan lapangan.
* Blokir transaksi akan dibuka kembali secara otomatis oleh sistem segera setelah seluruh kewajiban pokok dan bunga pada invoice terkait dinyatakan lunas (`PAID`).

### 6. Persetujuan Digital dan Pembaruan Versi
* Merchant wajib membaca seluruh dokumen ini dengan melakukan navigasi (*scrolling*) hingga bagian akhir sebelum tombol persetujuan aktif.
* Sistem akan merekam *timestamp*, versi dokumen, dan ID Merchant sebagai bukti persetujuan yang sah secara hukum.
* Apabila terdapat pembaruan versi Syarat dan Ketentuan oleh Admin, Merchant wajib memberikan persetujuan ulang sebelum dapat mengajukan perpanjangan tempo berikutnya.
* Merchant memahami bahwa informasi bunga, biaya, limit kredit, dan kewajiban pembayaran yang berlaku untuk transaksi tertentu dapat ditampilkan melalui sistem sebagai bagian dari rincian transaksi yang disetujui Merchant.

---
**Pernyataan Persetujuan:**
Dengan mengklik tombol "Setuju dan Ajukan", saya menyatakan telah membaca, memahami, dan menyetujui seluruh isi Syarat dan Ketentuan Fasilitas Kredit Fintech1000s ini.
