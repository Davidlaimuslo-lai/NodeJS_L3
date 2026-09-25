<script setup>
function kirimPesan(event) {
  event.preventDefault()

  alert("Pesan berhasil dikirim!")

  // Reset / refresh halaman
  window.location.reload()
}
</script>

<template>
    <div class="Judul">
      <h1>Kontak Kami</h1>
      </div>
  <div class="contact-container">

    <!-- BAGIAN KIRI -->
    <div class="info-kontak">
      <h1>Info kontak</h1>

      <h2>Alamat</h2>
      <p>jalan sini deket situ</p>

      <h2>Telepon</h2>
      <p>(+62)89555532444</p>

      <h2>Email</h2>
      <p>smkyadikasoreang@gmail.com</p>
    </div>

    <!-- BAGIAN KANAN -->
    <div class="form-kontak">
      <h1>Kirim Pesan</h1>

      <form @submit="kirimPesan">

        <label>Nama</label>
        <input
          type="text"
          placeholder="Masukkan Nama"
          required
        >

        <label>Email</label>
        <input
          type="email"
          placeholder="Masukan Email"
          required
          pattern="[a-zA-Z0-9._%+-]+@gmail\.com"
          title="Email harus menggunakan @gmail.com"
        >

        <label>Pesan</label>
        <textarea
          placeholder="Masukkan Pesan"
          required
        ></textarea>

         <div class ="btn-grad"><button type="submit">Kirim</button></div>

      </form>
    </div>

  </div>
</template>

<style scoped>
.Judul {
  text-align: center;
  padding: 40px 20px;
  background: linear-gradient(90deg, #315a91, #36b5e8);
  color: white;
  border-radius: 10px;
  width: 90%;
  max-width: 1100px;
  margin: 20px auto;
}

/* CONTAINER */
.contact-container {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  gap: 50px;
  width: 90%;
  max-width: 1100px;
  margin: 0 auto;
  padding: 30px 0;
  box-sizing: border-box;
}

/* KIRI */
.info-kontak {
  width: 45%;
}

/* KANAN */
.form-kontak {
  width: 45%;
}

/* FORM */
.form-kontak form {
  display: flex;
  flex-direction: column;
  width: 100%;
  max-width: 400px;
}

.form-kontak input,
.form-kontak textarea {
  width: 100%;
  padding: 10px;
  margin-bottom: 10px;
  box-sizing: border-box;
  border: 1px solid #aaa;
  border-radius: 5px;
}

.form-kontak textarea {
  height: 100px;
  resize: vertical;
}

/* TOMBOL */
.btn-grad {
  width: 100%;
  max-width: 300px;
  height: 50px;
  margin: 20px auto;

  display: flex;
  justify-content: center;
  align-items: center;

  background: linear-gradient(to right, #31546b, #20a9df);
  border-radius: 15px;

  box-shadow: 0 0 20px rgba(255, 255, 255, 0.7);
}

.form-kontak button {
  width: auto;
  padding: 8px 25px;
  border: none;
  background: transparent;
  color: white;
  font-size: 18px;
  cursor: pointer;
}


/* =========================
   TAMPILAN HP
   ========================= */

@media (max-width: 768px) {

  .Judul {
    width: 90%;
    padding: 30px 15px;
    margin: 15px auto;
  }

  .Judul h1 {
    font-size: 28px;
  }

  .contact-container {
    width: 90%;
    padding: 20px 0;
    flex-direction: column;
    gap: 30px;
  }

  .info-kontak,
  .form-kontak {
    width: 100%;
  }

  .form-kontak form {
    width: 100%;
    max-width: none;
  }

  .form-kontak input,
  .form-kontak textarea {
    width: 100%;
  }

  .btn-grad {
    width: 100%;
    max-width: 300px;
  }
}
</style>