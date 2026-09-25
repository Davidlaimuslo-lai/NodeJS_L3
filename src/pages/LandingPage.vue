<template>
  <main>
    <div class="Card1">
      <h1>Belanja perlengkapan sekolah, gampang & terpercaya</h1>

      <p>
        Mulai dari kaos,topi,sampai tas sekolah - semua ada di satu tempat
      </p>

      <div class="btn-grad">
        <RouterLink to="/product">Lebih lengkap</RouterLink>
      </div>
    </div>

    <video controls muted loop>
      <source src="/video/videopromosi.mp4" type="video/mp4" />
      Browser kamu tidak mendukung pemutaran video.
    </video>

    <div class="Container">
      <div class="Card">
        <p>🛡️</p>
        <h2>Kualitas Terjamin</h2>
        <p>Bahan dipilih oleh ahli sekolah</p>
      </div>

      <div class="Card">
        <p>✅</p>
        <h2>Harga bersahabat</h2>
        <p>Harga murah dikalangan siswa</p>
      </div>

      <div class="Card">
        <p>⚡</p>
        <h2>Penjualan Terlaris</h2>
        <p>Produk paling laris di toko kami</p>
      </div>
    </div>
  </main>
</template>

<style scoped>
.Card1 {
  text-align: center;
  padding: 70px 20px;
  background: linear-gradient(90deg, #315a91, #36b5e8);
  color: white;
  border-radius: 10px;
}

.Card1 h1 {
  margin: 0;
  font-size: 28px;
}

.Card1 p {
  font-size: 20px;
  margin: 10px 0;
}

video {
  width: 480px;
  max-width: 100%;
  margin: 16px auto 0;
  border-radius: 10px;
  display: block;
}

.Container {
  display: flex;
  justify-content: center;
  align-items: stretch;
  gap: 10px;
  margin-top: 20px;
  flex-wrap: wrap;
}

.Card {
  text-align: center;
  padding: 16px;
  border-radius: 10px;
  width: 175px;
  background: linear-gradient(90deg, #315a91, #36b5e8);
  color: white;
}

.btn-grad {
  width: 300px;
  max-width: 80%;
  height: 50px;
  margin: 20px auto;

  display: flex;
  justify-content: center;
  align-items: center;

  background: linear-gradient(to right, #31546b, #20a9df);
  border-radius: 15px;

  box-shadow: 0 0 20px rgba(255, 255, 255, 0.7);
}

.btn-grad a {
  color: white;
  text-decoration: none;
  font-size: 18px;
}

/* HP */
@media (max-width: 768px) {
  .Card1 {
    padding: 50px 15px;
  }

  .Card1 h1 {
    font-size: 20px;
  }

  .Card1 p {
    font-size: 14px;
    line-height: 1.5;
  }

  .btn-grad {
    width: 80%;
    max-width: 300px;
  }

  video {
    width: 100%;
    max-width: 480px;
  }

  .Container {
    flex-direction: column;
    align-items: center;
  }

  .Card {
    width: 80%;
    max-width: 300px;
  }
}
</style>