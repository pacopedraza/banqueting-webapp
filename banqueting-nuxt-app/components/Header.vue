<template>
  <header>
    <div class="header">
      <img src="../assets/images/banqueting_logo.jpg" alt="logo" />
    </div>
    <nav>
      <ul>
        <li><nuxt-link to=""></nuxt-link></li>
        <li><nuxt-link to="/">Inicio</nuxt-link></li>
        <li><nuxt-link to="/recipes">Galería</nuxt-link></li>
      </ul>
    </nav>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css"> 
    <a href="https://www.facebook.com/banquetingcelaya/" class="fa fa-facebook"></a>
    <a href="https://www.instagram.com/banqueting/?hl=es" class="fa fa-instagram"></a>
    <a href="tel:5214611783479" class="fa fa-whatsapp" style="font-size:70px;color:green"></a>
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

.fa {
  padding: 20px;
  font-size: 30px;
  width: 70px;
  text-align: center;
  text-decoration: none;
  margin: 5px 2px;
  border-radius: 50%;
}

.fa:hover {
    opacity: 0.7;
}

.fa-facebook {
  background: #3B5998;
  color: white;
  position: absolute;
  right: 0;
}

.fa-instagram {
  background: #C13584;
  color: white;
  position: absolute;
  right: 90px;
}

.fa-whatsapp {
  position: absolute;
  right: 200px;
}
</style>
