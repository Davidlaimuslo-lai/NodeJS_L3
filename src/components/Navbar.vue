<template>
  <nav class="navbar">
    <div class="logo">
      SMK Yadika soreang - Onlineshop
    </div>

  <div class="nav-menu">
     <RouterLink to="/"> Landing</RouterLink>
        <RouterLink to="/product"> Product</RouterLink>
        <RouterLink to="/About"> About</RouterLink>
        <RouterLink to="/FAQ"> FAQ</RouterLink>
        <RouterLink to="/Contact"> Contact</RouterLink>
  </div>
</nav>
</template>
<style scoped>
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px 32px;
  border-bottom: 1px solid #999;
  width: 100%;
  box-sizing: border-box;
}

.logo {
  color: #1f3b5b;
}

.nav-menu {
  display: flex;
  gap: 20px;
}
</style>