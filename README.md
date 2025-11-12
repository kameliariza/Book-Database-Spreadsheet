# Book-Database-Spreadsheet
A Google Apps Script solution for custom data entry into Google Sheets with category separation (Fiction/Non-Fiction) and duplicate validation.

[Bahasa Indonesia]
1. Buka Google Spreadsheet dan buat dokumen baru.
2. Buat kolom sesuai yang diinginkan.
3. Di menu atas, klik Ekstensi (Extensions).
4. Pilih Apps Script. Ini akan membuka jendela baru yang merupakan editor skrip.
5. Secara default, disana akan membuka satu file bernama Code.gs (atau Proyek Tanpa Judul). Kamu perlu membuat satu file lagi untuk antarmuka pengguna (form input).
Untuk Code.gs: Pastikan kalau kamu ada di file ini, lalu copas seluruh kode dari file kode_gs.txt.
6. Buat File HTML:
    - Di sebelah kiri, klik ikon + atau New file (File baru). Pilih HTML.
    - Beri nama file: FormBuku. Pastikan nama dan penulisannya sama.
    - Salin dan tempel seluruh kode dari bagian Form FormBuku_HTML.txt ke dalamnya.
    - Klik Save (icon disket)
7. Balik lagi ke tab Google Sheets, lalu refresh halaman.
8. Setelah reload, akan muncul menu baru di atas: “Koleksi Buku”. Kamu pastikan dulu judul buku tersebut mau di masukkan list di sheet mana.
9. Klik: Koleksi Buku → Input Buku Baru
    - Akan muncul popup form:
    - Izinkan autorisasi dulu, nanti centang semua. setelah selesai klik lagi Koleksi Buku → Input Buku Baru.
    - Isi judul dan penulis
10. Klik Simpan

Notes :
Jika judul sudah pernah kamu input:
Script akan mengecek kolom Judul (case-insensitive/gak peduli kapital atau bukan) 
Kalau ketemu, akan muncul pesan:
 “Buku dengan judul "..." sudah ada di database.”
 jadi tidak menambah baris baru.
 
[English]
1. Open Google Sheets and create a new document.
2. Create the columns as desired.
3. In the top menu, click Extensions.
4. Select Apps Script. This will open a new window that is the script editor.
5. By default, a file named Code.gs (or Untitled Project) will open. You need to create another file for the user interface (input form).
For Code.gs: Make sure you're in this file, then copy and paste all the code from the code_gs.txt file.
6. Create an HTML File:
    - On the left, click the + icon or New file. Select HTML.
    - Name the file: FormBuku. Make sure the name and spelling are the same.
    - Copy and paste all the code from the Form section of FormBuku_HTML.txt into it.
    - Click Save (the diskette icon).
7. Return to the Google Sheets tab and refresh the page.
8. After reloading, a new menu will appear at the top: "Book Collection." First, determine which sheet you want to include the book title in.
9. Click: Book Collection → Input New Book
    - A popup form will appear:
    - Allow authorization first, then check all boxes. Once finished, click Book Collection → Input New Book again.
    - Enter the title and author.
10. Click Save
