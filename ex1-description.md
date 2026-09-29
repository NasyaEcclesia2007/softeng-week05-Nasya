1. Primary actor: Customer  
2. Stakeholders: Customer (tidak antre lama), Bank (antrean tertib)  
3. Trigger: Customer ingin berkunjung ke cabang  
4. Precondition: Customer punya akun, app terpasang  
5. Main scenario:  
   * Customer menjalankan Log In («include»)  
   * Customer memilih cabang  
   * Customer memilih layanan  
   * Customer memilih slot waktu  
   * App mengirim request booking, sistem mengecek ketersediaan  
   * Sistem menyimpan tiket dan menjalankan Send Reminder («include»)  
   * App menampilkan tiket digital  
6. Extensions:  
   * 5a. Cabang penuh: sistem menyarankan cabang terdekat («extend» Suggest Nearest Branch), kembali ke langkah 2  
   * 5b. Slot terisi: Customer memilih slot lain, kembali ke langkah 4  
7. Postcondition: tiket tersimpan, reminder terjadwal