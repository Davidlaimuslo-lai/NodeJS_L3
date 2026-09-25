<script setup>
import ProductCard from '../components/ProductCard.vue'

const daftarProduk = [
  {
    id: 1,
    nama: 'Kaos Sekolah',
    harga: 75000,
    gambar: '/image/kaos.jpg'
  },
  {
    id: 2,
    nama: 'Topi Sekolah',
    harga: 25000,
    gambar: '/image/topi.jpg'
  },
  {
    id: 3,
    nama: 'Tas Sekolah',
    harga: 120000,
    gambar: '/image/tas.jpg'
  },

]
</script>

<template>
  <div class="product-grid">
    <ProductCard
      v-for="produk in daftarProduk"
      :key="produk.id"
      :nama="produk.nama"
      :harga="produk.harga"
      :gambar="produk.gambar"
    />
  </div>
</template>

<style scoped>
.product-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 30px;
  padding: 30px;
} 
@media (max-width: 900px) {
  .product-grid {
    grid-template-columns: repeat(2, 1fr);
  } 
}

@media (max-width: 600px) { 
  .product-grid {
    grid-template-columns: 1fr; 
    padding: 15px;
  }
} 
</style>