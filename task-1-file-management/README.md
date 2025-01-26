# Task 1: File Management

## Tujuan

Tugas ini bertujuan untuk memanipulasi file dan direktori menggunakan perintah dasar Linux.

## Langkah-langkah

### Task 1.1: Create a directory structure as follows:

![Struktur](task-1-file-management/screenshoot/image.png)

Perintah yang digunakan:

```bash
mkdir -p project/reports/2024 project/reports/2025 project/scripts project/data
```

### Task 1.2: Create three empty files in the reports/2024 directory: `q1.txt, q2.txt, and q3.txt.`

Buat tiga file kosong dengan nama `q1.txt`, `q2.txt`, dan `q3.txt` di dalam direktori `reports/2024/`.

```bash
touch reports/2024/q1.txt
touch reports/2024/q2.txt
touch reports/2024/q3.txt
```

### Task 1.3: Move `q1.txt` to the 2025 directory.

Pindahkan file `q1.txt` ke dalam direktori `reports/2025/`.

```bash
mv reports/2024/q1.txt reports/2025/
```

### Task 1.4: Copy `q2.txt` to the scripts directory and rename it as `analysis.txt.`

Salin file `q2.txt` ke direktori `scripts/` dan beri nama baru `analysis.txt`.

```bash
cp reports/2024/q2.txt script/analysis.txt
```

### Task 1.5: List all files in the `reports/2025` directory using ls and log the output to `file_list.log.`

Gunakan perintah untuk menampilkan semua file yang ada di dalam direktori `reports/2025/` dan simpan hasilnya ke dalam file `file_list.log`.

```bash
ls reports/2025 > file_list.log
```

### Task 1.6: Display the contents of `q3.txt` using cat and append "Task Completed" to the file.

```bash
echo "Task Completed" >> reports/2024/q3.txt
cat reports/2024/q3.txt
```

Tampilkan isi dari file `q3.txt` dan tambahkan tulisan "Task Completed" pada akhir file tersebut.

### Task 1.7: Use tree to display the directory structure of the project directory and save the output to `structure.log.`

Tampilkan struktur direktori dari direktori `project/` dan simpan hasilnya ke dalam file `structure.log`.

```bash
tree ~/Documents/project > structure.log
```

### Task 1.8: Remove the `scripts/analysis.txt` file and confirm its deletion by listing the contents of the scripts directory.

Hapus file `scripts/analysis.txt` dan pastikan bahwa file tersebut sudah terhapus dengan melihat isi dari direktori `scripts/`.

```bash
rm scripts/analysis.txt
ls scripts
```

### Task 1.9: Copy the entire project directory to a new directory named `project-old.`

Salin seluruh direktori `project/` ke dalam direktori baru bernama `project-old/`.

```bash
cp -r ~/Documents/project ~/Documents/project-old
```

### Task 1.10: Delete the original project directory.

Hapus direktori `project/` yang asli.

```bash
rm -ri ~/Documents/project
```

### Task 1.11: Create a large file (5GB) in the data directory using dd or truncate. Name it `large_file.dat`.

Buat file besar berukuran 5GB di dalam direktori `data/` dengan menggunakan perintah `dd` atau `truncate` dan beri nama file tersebut `large_file.dat`.

```bash
truncate -s 5G ~/Documents/large_file.dat
```

## Hasil

Setelah menyelesaikan semua langkah di atas, pastikan untuk mengecek dan memverifikasi hasilnya sesuai instruksi yang diberikan.

## Tantangan

Deskripsikan tantangan atau masalah yang dihadapi selama pengerjaan tugas ini.

## Kesimpulan

Jelaskan pelajaran yang didapat dari pengerjaan tugas ini dan langkah-langkah berikutnya yang akan dilakukan.
