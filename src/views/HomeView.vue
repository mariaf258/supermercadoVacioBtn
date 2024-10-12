<script setup lang="ts">
import TheWelcome from '../components/TheWelcome.vue'
</script>

<template>
  <div id="app">
    <div class="page-wrapper">
      <div class="">
        <header>
          <img src="../../public/img/Supermercado-title-color.png" alt="" />
          <h1>Tu compra es <b>100% segura</b></h1>
          <img src="../../public/img/security.png" alt="" />
        </header>

        <main class="main">
          <div class="button-container">
            <button class="expand-button">
              <img src="../../public/img/shopping-cart-white.png" alt="" />
              <span class="tooltip">Sigue comprando</span>
            </button>
          </div>

          <div class="title">
            <h2>Tus compras</h2>
          </div>
        </main>

        <!-- <hr class="separator-h" /> -->

        <footer>
          <div class="footer-container align-items-center">
            <img
              src="../../public/img/Logo_Supermercado.png"
              alt="logo-supermercado-xyz"
              class="logo-supermercado"
            />
            <p>Todo lo que necesitas en un solo lugar</p>
            <hr class="separator-v" />
            <div class="footer-right">
              <img src="../../public/img/map-color.png" alt="maps" class="maps" />
              <p class="maps">
                Av 13 #3-24 ***** - Cúcuta.<br />
                Norte de Santander, Colombia.
              </p>
              <img src="../../public/img/call-color.png" alt="call" class="call" />
              <p class="call">
                Celular: ##########<br />
                Telefono: ##########
              </p>
            </div>
          </div>
        </footer>
      </div>
    </div>
  </div>
</template>

<style>
header {
  width: 100%;
  height: 50px;
  background-color: #f96616;
  display: flex;
  justify-content: space-between;
  place-items: center;
  padding: 20px;
}

header img {
  /* width: 100%; */
  height: 30px;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #f96616;
}

header h1 {
  /* width: 100%; */
  height: 30px;
  color: white;
  font-size: 18px;
  margin-left: -80px;
}

header h1 b {
  /* width: 100%; */
  height: 30px;
  color: white;
  font-size: 17px;
  font-weight: bold;
}

.main {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
  text-align: center;
  margin-top: -10px;
  margin-bottom: -150px;
}

.button-container {
  position: relative;
  display: inline-block;
  width: 30px;
  height: 30px;
  /* background-color: #f96616; */
  /* border: 1px solid #f96616; */
  border-radius: 5px;
  cursor: pointer;
}

.expand-button {
  /* position: relative;
  background-color: #f96616;
  border: none;
  cursor: pointer; */
  top: -200px;
  left: 630px;
  background-color: transparent;
  border: none;
  cursor: pointer;
  padding: 10px;
  position: absolute;
  display: flex;
  align-items: center;
}

/* .expand-button:hover {
  width: 120px;
  height: 30px;
} */

.tooltip {
  visibility: hidden;
  background-color: #f96616;
  color: #fff;
  text-align: center;
  border-radius: 5px;
  padding: 5px 35px 5px 5px;
  position: absolute;
  bottom: 140%;
  left: -80%;
  transform: translateX(-50%);
  z-index: 1;
  opacity: 0;
  transition: opacity 0.3s;
  white-space: nowrap;
  height: 30px;
}

.expand-button:hover .tooltip {
  visibility: visible;
  opacity: 1;
}

button img {
  width: 30px;
  height: 30px;
  justify-content: end;
  background-color: #f96616;
  border: 1px solid #f96616;
  border-radius: 5px;
  position: relative;
  z-index: 2;
  top: -60px;
}

.Ellipse {
  max-width: 1000px;
  width: 150px;
  height: 150px;
  margin-bottom: 1rem;
  margin-top: -100px;
}

.shopping-cart {
  max-width: 1000px;
  width: 100px;
  height: 100px;
  margin-top: -140px;
  margin-bottom: 50px;
}

.title h2 {
  font-size: 1.5rem;
  text-align: center;
  position: relative;
  color: black;
  top: -280px;
  left: 10px;
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
}

/* .button {
  text-align: left;
  float: left;
  margin-top: 10px;
  display: flex;
  justify-content: center;
} */

.button a {
  color: white;
  background-color: #f96616;
  border: 1px solid #f96616;
  margin-top: 20px;
  /* margin-right: 20px; */
  cursor: pointer;
  border-radius: 3px;
  height: 35px;
  width: 180px;
  text-align: center;
  text-decoration: none;
  font-size: 17px;
  padding: 6px;
}

.button a:hover {
  background-color: white;
  color: #f96616;
  border: 1px solid #f96616;
}

/* .separator-h {
  width: 100%;
  border: 1px solid #f96616;
} */

footer {
  width: 100%;
  height: 100%;
  justify-content: space-around;
  align-items: center;
  padding: 20px;
  border-radius: 0px 0px 10px 10px;
  border: 1px solid #f96616;
}

.footer-container {
  display: flex;
  justify-content: space-around;
  align-items: center;
  padding-bottom: 10px;
  margin-left: -70px;
}

.footer-right {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.footer-right div {
  display: flex;
  align-items: center;
}

.footer-right p {
  display: flex;
  justify-content: space-around;
  align-items: center;
  /* padding: 20px; */
  justify-content: space-around;
}

.footer-right img {
  display: flex;
  justify-content: space-around;
  align-items: center;
  /* padding: 20px; */
  justify-content: space-around;
  margin-left: -130px;
}

.separator-v {
  border-left: 1px solid #f96616;
  height: 170px;
  display: inline-block;
  margin-right: 20px;
}

footer p {
  /* width: 100%; */
  height: 100%;
  left: 20px;
  color: #f96616;
  font-family: Georgia, 'Times New Roman', Times, serif;
  display: flex;
  margin-left: -90px;
  font-size: 17px;
}

footer img {
  width: 230px;
  height: 150px;
  /* background-color: #f96616; */
  margin-left: 20px;
  margin-top: 20px;
}

footer .maps {
  width: 35px;
  height: 35px;
}

p.maps {
  width: 300px;
  margin-right: -50px;
  margin-top: -50px;
  text-align: center;
}

footer .call {
  width: 30px;
  height: 30px;
}

p.call {
  width: 300px;
  margin-right: -250px;
  margin-top: -48px;
  text-align: center;
}
</style>
