<template>
  <header>
    <div class="header">
      <img src="../assets/images/banqueting_logo.jpg" alt="logo" />
    </div>
    <nav>
      <ul>
        <li><nuxt-link to=""></nuxt-link></li>
        <li><nuxt-link to="/">Inicio</nuxt-link></li>
        <li><nuxt-link to="/recipes">Fotos</nuxt-link></li>
        <li><nuxt-link to="/gallery">Futura Seccion</nuxt-link></li>
      </ul>
    </nav>
  </header>
</template>

<style scoped>
header {
  width: 100%;
  height: 100px;
  display: flex;
  justify-content: right;
  align-items: center;
  background-color: #494942;
}
.header img {
  float: left;
  width: 100px;
  height: 100px;
  object-fit: cover;
  border-radius: 50%;
}

ul{
  list-style: none;
  padding: 0;
  margin: 0;
  display: flex;
  justify-content: center;
  align-items: center;
}

li {
  margin: 0 10px;
}

a {
  text-decoration: none;
  color: white;
}
</style>
