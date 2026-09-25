<template>
    <main>
        <div class="Card1">
            <h1>Belanja perlengkapan sekolah, gampang & terpercaya</h1>
            <p>Mulai dari kaos,topi,sampai tas sekolah - semua ada di satu  tempat</p>
        <div class ="btn-grad"><RouterLink to="/product">Lebih lengkap</RouterLink></div>
    </div>
   
    <video controls width="480" muted loop> 
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
  padding: 70px 30px;
  background: linear-gradient(90deg, #315a91, #36b5e8);
  color: white;
  border-radius: 10px;

  width: 90%;
  max-width: 1100px;
  margin: 20px auto;
} 
.Card1 h1 {
  font-size: 36px;
  margin-bottom: 15px;
}
video { 
        margin-top: 16px; 
        border-radius: 10px; 
        display: block; 
        margin-left: auto;
        margin-right: auto;
} 
.Card{
        text-align: center;
        padding: 16px;  
        border-radius: 10px;
        border: 1px;
        width: 175px;  
        margin-top: 20px;
        margin-left: 10px;
        background: linear-gradient(90deg, #315a91, #36b5e8);
        color:white;
        box-shadow: 20%;
        justify-content: space-between;
}
.Container{
        display: flex;
        justify-content: center;
        align-items: center;
        box-shadow: 20%;
        align-items: center;    
        margin-top: 20px;
}
.btn-grad {
        background-image: linear-gradient(to right, #314755 0%, #26a0da 51%, #314755 100%);
}

.btn-grad {
        width: 300px;
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

</style>