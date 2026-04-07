# CSV to Google Sheets Workflow (n8n)

## 📋 Deskripsi
Workflow ini membaca file CSV dari lokal, mem-parsing data, lalu mengirimnya ke Google Sheets.

## 🔧 Prasyarat
- n8n (self-hosted)
- Node **Safe Execute Command** (install dari Community Nodes)
- Google Sheets account (untuk OAuth2)
- File CSV dengan format: `kolom1,kolom2,kolom3,kolom4,kolom5`

## 🚀 Cara Install
1. Download file `CSV_to_Google_Sheets.json`
2. Di n8n, klik **Import from File**
3. Setup credential Google Sheets (ikuti petunjuk OAuth)
4. Set **Environment Variable** `CSV_FILE_PATH` di n8n:
   - Buka **Settings** → **Environment Variables**
   - Tambahkan: `CSV_FILE_PATH` = `/path/to/your/barang.csv`
5. Sesuaikan nama sheet di node Google Sheets (default: `sheet 1`)
6. Aktifkan workflow dan Execute

## 📄 Contoh File CSV
2026,04,07,Flashdisk,00001



## 🧠 Catatan
- Node `Safe Execute Command` harus diinstall terlebih dahulu dari **Settings** → **Community Nodes**
- Pastikan file CSV ada di path yang sudah ditentukan

## 👤 Author
Dibuat oleh Fahri Permana - SMK Az Zahra Sepatan
