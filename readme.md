Autop-letters merupakan sistem automasi yang dibuat untuk mempermudah pembuatan application letter atau surat lamaran dengan melakukan generate berdasarkan wordlist yang sudah ada. Tentunya cara ini lebih efisien daripada membuatnya satu per satu :).

Sayangnya untuk saat ini program ini hanya dapat digunakan di **Windows system** karena salah satu library yang digunakan adalah [docx](https://python-docx.readthedocs.io/en/latest/), yang mana memerlukan aplikasi Microsoft Word Document.

# Demo
![Demo](assets\carbon.png)
[Demo video](https://drive.google.com/file/d/1euCrkya5hJ2Wn0yrHPwOBdfZzCoSfnYC/view?t=1) *sorry for bad quality video :(* 

# Installation
1. Pertama, pastikan sudah ada python di komputer kamu. Jika belum ada, download dulu di website resminya [python disini](https://www.python.org/downloads/).
2. Clone repository ini
```
git clone https://github.com/Hakim-0000/autop-letters
```
3. Jika sudah, untuk step 2 ini **OPSIONAL**, jika kamu mau melewati step ini aman-aman saja. Di step 2 ini kamu bisa membuat virtual environment untuk python dengan cara, dan run venv tersebut.
```powershell
# buat venv
python -m venv autop_letter

# running venv di powershell
./autop_letter/Scripts/Activate.ps1
# running venv di cmd
./autop_letter/Scripts/activate.bat
```
3. Selanjutnya install requirements package yang dibutuhkan untuk automasi
```powershell
pip install -r requirements.txt
```
4. Siapkan dokumen yang kamu butuhkan. Ada beberapa dokumen yang bisa kamu edit
    - `SURAT_LAMARAN_KERJA.docx` didalam folder docs itu merupakan contoh surat lamaran kerja. Silahkan diubah, kecuali yang bertanda `<<>>` karena itu yang nanti akan menjadi acuan program untuk edit secara otomatis.
    - `doc_to_merge.pdf` didalam folder pdf-to-be-merge itu merupakan dokumen yang nantinya akan di merge dengan application letter atau lamaran
    - `company_list.txt` dan `job_title_list.txt` merupakan file wordlist nama PT atau perusahaan sekaligus lowongan pekerjaan yang ditawarkan. Silahkan diisi sendiri :)

# Usage
Mulai automasinya untuk membuat banyak surat lamaran dengan cara memasukkan input wordlist dan juga lokasi sekarang kamu berada.
```powershell
python autop-letters.py -c company_wordlist -j job_wordlist -l location
```

Contohnya seperti berikut, lalu tekan enter.
```powershell
python autop-letters.py -c company_list.txt -j job_title_list.txt -l Semarang
```
Done, tinggal kirim-kirim surat lamarannya deh :)

# ⚠️⚠️⚠️**Peringatan**⚠️⚠️⚠️
**Tidak ada jaminan** bisa dapat pekerjaan kalo pakai ini, karena program ini hanya untuk mempermudah saja :)

### Edit source code?
Boleh banget kalo kamu mau ambil source code nya dan mau edit sesuka kamu :) dan nggak perlu mention ke aku juga :D

### Pertanyaan?
Kalo kamu ada pertanyaan, bisa chat ke
- Discord: `urk3e`
- Telegram: `urk3e`

I'll try my best to help you out :)