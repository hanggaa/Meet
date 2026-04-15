# Syarat dan Ketentuan Fasilitas Kredit Fintech1000s

**Versi:** 2.0.0
**Tanggal Pembaruan Terakhir:** 10 April 2026

Selamat datang di layanan Fintech1000s. Dengan menyetujui dokumen ini, Anda ("Merchant") sepakat untuk mengaktifkan fasilitas kredit yang dikelola oleh Selling Agent ("SA") melalui platform PT. Mitra Seribu Saudara ("PT. MSS"). Harap membaca ketentuan berikut dengan saksama sebelum melanjutkan.

---

### 1. Definisi Fasilitas
* **Fintech1000s**: Fitur restrukturisasi tagihan di dalam ekosistem Mitra1000s yang memungkinkan Merchant mengubah invoice reguler (prefix `INV-`) menjadi invoice pembiayaan dengan perpanjangan tempo (prefix `FIN-`).
* **Limit Kredit**: Saldo plafon maksimal yang diberikan oleh Selling Agent kepada Merchant untuk digunakan sebagai jaminan perpanjangan tempo.
* **Masa Perpanjangan**: Jangka waktu tambahan yang diberikan untuk pelunasan, yakni maksimal 56 hari (8 minggu) sejak pengajuan perpanjangan tempo disetujui.

### 2. Pemberian Limit dan Pengajuan
* Pemberian, perubahan, serta pembatalan limit kredit merupakan wewenang penuh Selling Agent yang menangani wilayah Merchant terkait.
* Selling Agent hanya dapat memberikan limit kredit selama sisa plafon SA yang tersedia di sistem masih mencukupi.
* Pengajuan perpanjangan tempo hanya dapat dilakukan jika nilai total invoice tidak melebihi sisa limit kredit aktif Merchant.
* Jika nilai invoice melebihi limit, Merchant wajib menutup selisih tersebut terlebih dahulu melalui mekanisme cicilan pokok sebelum perpanjangan dapat diproses oleh sistem.

### 3. Suku Bunga dan Biaya
* Fasilitas ini mengenakan bunga layanan sebesar 0.25% per minggu.
* Bunga dihitung secara mingguan berdasarkan Sisa Pokok Pinjaman (*Remaining Principal*) pada minggu berjalan.
* Bunga akan diakumulasikan secara kumulatif dan wajib dibayarkan secara penuh pada saat Merchant melakukan pelunasan akhir invoice.
* Bunga tetap akan berjalan dan tercatat secara otomatis oleh sistem meskipun tagihan telah melewati batas waktu 56 hari atau berstatus NPL (*Non-Performing Loan*).

### 4. Mekanisme Pembayaran (Cart Billing)
* Merchant wajib melakukan pembayaran melalui sistem **Cart Billing**, yang memungkinkan pemilihan satu atau lebih invoice `FIN-` dalam satu sesi transaksi.
* Setiap pembayaran menggunakan satu kode billing agregat dengan format `BILL-{merchant_id}-{timestamp}` melalui metode Virtual Account (VA) yang tersedia.
* Alokasi dana pembayaran akan diprioritaskan untuk mengurangi Pokok Pinjaman terlebih dahulu agar limit kredit Merchant segera pulih secara real-time.
* Invoice dengan prefix `FIN-` bersifat final dan tidak dapat dilakukan perpanjangan tempo kembali untuk periode berikutnya.

### 5. Konsekuensi Keterlambatan (Wanprestasi)
* Batas maksimal pelunasan seluruh kewajiban adalah H+56 sejak tanggal persetujuan perpanjangan tempo.
* Apabila pada hari ke-57 (H+57) invoice belum lunas, sistem secara otomatis melakukan blokir transaksi pada akun Mitra1000s Merchant sehingga tidak dapat melakukan pemesanan barang baru.
* Status tagihan akan berubah menjadi **Credit Default / NPL** dan akan diekskalasi kepada Selling Agent terkait untuk proses penagihan lapangan.
* Blokir transaksi akan dibuka kembali secara otomatis oleh sistem segera setelah seluruh kewajiban pokok dan bunga pada invoice terkait dinyatakan lunas (`PAID`).

### 6. Persetujuan Digital dan Pembaruan Versi
* Merchant wajib membaca seluruh dokumen ini dengan melakukan navigasi (*scrolling*) hingga bagian akhir sebelum tombol persetujuan aktif.
* Sistem akan merekam *timestamp*, versi dokumen, dan ID Merchant sebagai bukti persetujuan yang sah secara hukum.
* Apabila terdapat pembaruan versi Syarat dan Ketentuan oleh Admin, Merchant wajib memberikan persetujuan ulang sebelum dapat mengajukan perpanjangan tempo berikutnya.

---
**Pernyataan Persetujuan:**
Dengan mengklik tombol "Setuju dan Ajukan", saya menyatakan telah membaca, memahami, dan menyetujui seluruh isi Syarat dan Ketentuan Fasilitas Kredit Fintech1000s ini.