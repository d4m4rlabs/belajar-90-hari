# Belajar Fullstack 90 Hari — Kyokai (d4m4rlabs)

> Perjalanan belajar fullstack developer dari nol dalam 90 hari.
> Dimulai 16 Mei 2026.

---

## Progress

| Hari | Materi | Status |
|------|--------|--------|
| Hari 1 | HTML, CSS, JavaScript Pertama | ✅ Selesai |
| Hari 2-3 | Variabel, Tipe Data, If/Else | ✅ Selesai |
| Hari 4 | Loop/Perulangan | 🔄 Berikutnya |

---

## Hari 1 — JavaScript Pertama

**Tanggal:** 16 Mei 2026

**Yang Dipelajari:**
- `function` — blok kode yang bisa dipanggil berkali-kali
- `getElementById` — mencari elemen HTML berdasarkan id
- `.innerText` — membaca atau mengubah teks elemen
- `.style.color` — mengubah warna teks lewat JavaScript
- CSS: `background-color`, `border-radius`, `padding`, `transition`, `display: flex`, `gap`, `cursor: pointer`, `:hover`

**Project:**
- Halaman perkenalan diri dengan 4 tombol interaktif
- Dark theme (#0f0f0f)
- Tombol: Perkenalan, Tujuan 90 Hari, Tanggal, Reset

**Bug yang Ditemukan:**
- `<script>` harus di dalam `<body>` sebelum `</body>`
- `margin-bottom: inline-block` salah — harusnya `display: inline-block`

**File:** `hari1.html`

---

## Hari 2-3 — Variabel, Tipe Data, If/Else

**Tanggal:** 18 Mei 2026

**Yang Dipelajari:**

Variabel:
```javascript
let nama = "Kyokai";   // bisa diubah
const umur = 17;       // tidak bisa diubah
// hindari var         // cara lama
```

Tipe Data:
```javascript
let teks   = "Kyokai"; // String
let angka  = 90;       // Number
let benar  = true;     // Boolean
let kosong = null;     // Null
let belum;             // Undefined
```

Ambil Input dari User:
```javascript
let nama  = document.getElementById("nama").value;
let angka = Number(document.getElementById("angka").value);
```

If / Else:
```javascript
if (nilai >= 80) {
  pesan = "Bagus!";
} else if (nilai >= 60) {
  pesan = "Cukup!";
} else {
  pesan = "Belajar lagi!";
}
```

Cek Input Kosong:
```javascript
if (nama == "") {
  // kosong
} else {
  // ada isinya
}
```

**Project:**
- Progress checker 90 hari
- Input angka dari user
- 6 kondisi if/else if dengan warna berbeda

**Bug yang Ditemukan:**
- `fungction` → `function`
- `getElementByid` → `getElementById` (I besar)
- `getElementByld` → `getElementById` (Id bukan ld)
- Tanda kutip tidak ditutup → `"#a855f7"`
- Hardcode nilai → harusnya pakai `.value`
- `else if` duplikat → kondisi terakhir tidak pernah jalan
- `getElementById(hasil)` → harus `getElementById("hasil")`

**File:** `hari2-3.html`

---

## Problem Solving — Pola Cek Bug

```
Error tidak jalan?
→ Cek id di HTML ada tidak?
→ Cek typo getElementById?
→ Cek tanda kutip buka tutup?
→ Cek tanda titik sebelum innerText?
→ Cek posisi script di dalam body?
```

**Skor Problem Solving: 7/10**

---

## Konsep Wajib Diingat

```
.value          → selalu String, pakai Number() untuk angka
id="nama"       → harus sama persis di HTML dan JS
tanda kutip     → harus selalu buka dan tutup
else if duplikat→ kondisi ketiga tidak akan pernah jalan
script position → harus sebelum </body>
```

---

## Git Commands yang Dipakai

```bash
git init
git add .
git commit -m "pesan"
git branch -M main
git remote add origin https://github.com/d4m4rlabs/NAMA-REPO.git
git push -u origin main

# Setiap hari cukup:
git add .
git commit -m "Hari X - materi"
git push
```

---

## Roadmap Selanjutnya

- [ ] Hari 4 — Loop (for, while)
- [ ] Hari 5 — Array dan Object
- [ ] Hari 6-10 — DOM Manipulation lanjutan
- [ ] Hari 11-25 — JavaScript ES6+
- [ ] Hari 26-50 — React + Tailwind CSS
- [ ] Hari 51-75 — Node.js + Express + Database
- [ ] Hari 76-90 — Fullstack Project + Deploy

---

## Tools yang Dipakai

- VS Code
- Git + GitHub
- Browser (Live Server)
- Claude AI — sebagai coach/tutor

---

*"Tidak ada yang instan. Seperti Ippo — latihan setiap hari sampai jadi."*
— Kyokai, 16 Mei 2026