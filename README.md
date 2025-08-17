# 🛒 Olshop Web - Keranjang & Checkout WhatsApp

Proyek ini adalah contoh **web toko online sederhana** menggunakan **HTML + TailwindCSS + JavaScript**.  
Fitur utama adalah **keranjang belanja** dan **checkout langsung via WhatsApp**.

---

## ✨ Fitur
- Tampilan modern menggunakan [TailwindCSS](https://tailwindcss.com/).
- Daftar produk dalam grid responsif.
- Tombol **Add to Cart** untuk memasukkan produk ke keranjang.
- Ringkasan keranjang berisi daftar item + total harga.
- Tombol **Checkout via WhatsApp** yang otomatis membuka chat ke nomor admin.
- Harga dalam format **Rupiah (Rp)**.

---

## 🚀 Cara Menjalankan
1. Clone / download repository ini.
2. Buka file `index.html` di browser (cukup double click).
3. Pastikan ada koneksi internet agar **Tailwind CDN** termuat.  
   > Jika ingin offline, unduh file `tailwind.css` lalu ganti CDN dengan file lokal.

---

## ⚙️ Cara Edit Produk
Produk berada di dalam section grid di file `index.html`:

```html
<div class="bg-white rounded-xl shadow-lg overflow-hidden p-4 text-center">
  <img src="https://placehold.co/400x300/2563EB/ffffff?text=Gambar" class="w-full h-48 object-cover mb-4" alt="Nama Produk">
  <h3 class="text-xl font-semibold mb-2">Nama Produk</h3>
  <p class="text-gray-600 mb-4">Rp29.999</p>
  <button class="add-to-cart w-full py-2 bg-blue-600 text-white rounded-lg hover:bg-blue-700 transition-colors"
          data-product="Nama Produk" data-price="29999">
    Add to Cart
  </button>
</div>
```

### Untuk menambahkan produk baru:
1. **Copy paste div di atas**.
2. Ganti:
   - `src` gambar → link gambar produk.
   - `alt` → nama produk.
   - `h3` → nama produk.
   - Harga (`Rp...`) → harga rupiah.
   - `data-product` → nama produk.
   - `data-price` → angka harga tanpa titik.

---

## 📲 Cara Ganti Nomor WhatsApp
Buka bagian script di bawah file `index.html`:

```js
const whatsappNumber = "6281234567890"; // Ganti dengan nomor WhatsApp kamu
```

Ganti dengan nomor kamu (format internasional tanpa `+`).

---

## 🖼️ Preview
![Preview Website](https://placehold.co/400x300/2563EB/ffffff?text=apa+lu?)
