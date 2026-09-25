<template>
  <nav class="navbar">
    <div class="logo">
      SMK Yadika Soreang - Onlineshop
    </div>

    <div class="nav-menu">
      <RouterLink to="/">Landing</RouterLink>
      <RouterLink to="/product">Product</RouterLink>
      <RouterLink to="/about">About</RouterLink>
      <RouterLink to="/FAQ">FAQ</RouterLink>
      <RouterLink to="/Contact">Contact</RouterLink>
    </div>
  </nav>
</template>

<style scoped>
.navbar {
  width: 100%;
  box-sizing: border-box;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 30px;
  padding: 18px 50px;
  background: white;
}

/* Nama toko */
.logo {
  flex-shrink: 0;
  color: #1f3b5b;
  font-size: 20px;
  font-weight: 500;
  white-space: nowrap;
}

/* Menu */
.nav-menu {
  display: flex;
  align-items: center;
  justify-content: flex-end;
  gap: 28px;
  flex-wrap: wrap;
}

.nav-menu a {
  color: #222;
  text-decoration: none;
  font-size: 17px;
  white-space: nowrap;
}

.nav-menu a:hover {
  color: #2196d3;
}


/* =========================
   TAMPILAN HP
========================= */

@media (max-width: 768px) {
  .navbar {
    flex-direction: column;
    align-items: stretch;
    justify-content: center;
    gap: 12px;
    padding: 15px 20px;
  }

  .logo {
    width: 100%;
    text-align: center;
    white-space: normal;
    font-size: 18px;
    line-height: 1.3;
  }

  .nav-menu {
    width: 100%;
    justify-content: center;
    gap: 10px 18px;
  }

  .nav-menu a {
    font-size: 15px;
  }
}
</style>