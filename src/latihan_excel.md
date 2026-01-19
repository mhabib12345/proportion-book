# 📊 Latihan Rumus Excel Interaktif

Gunakan tabel di bawah ini untuk menjawab soal-soal latihan. Masukkan rumus Excel yang tepat (gunakan huruf kapital) lalu klik tombol **Cek Jawaban**.

### Tabel Data Referensi:
| | A (Nama Produk) | B (Harga Satuan) | C (Jumlah Terjual) |
|:---:|:---:|:---:|:---:|
| **1** | Kopi | 15000 | 10 |
| **2** | Teh | 10000 | 5 |
| **3** | Roti | 5000 | 20 |

---

### Soal 1: Penjumlahan Dasar
Hitung total seluruh produk yang terjual (Kolom C)!
*Input jawaban (Contoh: =SUM(C1:C3)):*

<input type="text" id="soal1" placeholder="Masukkan rumus...">
<button onclick="cekSoal1()">Cek Jawaban</button>
<p id="hasil1"></p>

---

### Soal 2: Perkalian & Total Harga
Hitung total pendapatan untuk **Kopi** saja (Harga Satuan $\times$ Jumlah Terjual)!
*Input jawaban:*

<input type="text" id="soal2" placeholder="Masukkan rumus...">
<button onclick="cekSoal2()">Cek Jawaban</button>
<p id="hasil2"></p>

---

### Soal 3: Fungsi Logika (IF)
Jika jumlah terjual (C3) lebih dari 15, maka tampilkan "Laris", jika tidak tampilkan "Biasa".
*Input jawaban:*

<input type="text" id="soal3" placeholder="Masukkan rumus...">
<button onclick="cekSoal3()">Cek Jawaban</button>
<p id="hasil3"></p>

---

<script>
function cekSoal1() {
    var jawaban = document.getElementById("soal1").value.replace(/\s+/g, '');
    var feedback = document.getElementById("hasil1");
    if (jawaban === "=SUM(C1:C3)") {
        feedback.innerHTML = "✅ Benar! Kamu menggunakan fungsi SUM dengan tepat.";
        feedback.style.color = "green";
    } else {
        feedback.innerHTML = "❌ Salah. Coba gunakan =SUM(C1:C3)";
        feedback.style.color = "red";
    }
}

function cekSoal2() {
    var jawaban = document.getElementById("soal2").value.replace(/\s+/g, '');
    var feedback = document.getElementById("hasil2");
    if (jawaban === "=B1*C1") {
        feedback.innerHTML = "✅ Benar! Perkalian sel menggunakan tanda bintang (*).";
        feedback.style.color = "green";
    } else {
        feedback.innerHTML = "❌ Salah. Coba masukkan =B1*C1";
        feedback.style.color = "red";
    }
}

function cekSoal3() {
    var jawaban = document.getElementById("soal3").value.replace(/\s+/g, '');
    var feedback = document.getElementById("hasil3");
    // Mengecek jawaban dengan kutipan ganda atau tunggal
    if (jawaban === '=IF(C3>15,"Laris","Biasa")' || jawaban === "=IF(C3>15,'Laris','Biasa')") {
        feedback.innerHTML = "✅ Luar Biasa! Fungsi IF kamu sudah benar.";
        feedback.style.color = "green";
    } else {
        feedback.innerHTML = "❌ Salah. Formatnya: =IF(C3>15,\"Laris\",\"Biasa\")";
        feedback.style.color = "red";
    }
}
</script>

<style>
input {
    padding: 8px;
    width: 250px;
    border-radius: 4px;
    border: 1px solid #ccc;
    margin-bottom: 10px;
}
button {
    padding: 8px 15px;
    background-color: #4CAF50;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
}
button:hover {
    background-color: #45a049;
}
#hasil1, #hasil2, #hasil3 {
    font-weight: bold;
    margin-top: 5px;
}
</style>