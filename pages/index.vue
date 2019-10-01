<template>
  <main>
    <div class="top" style="height: 52vh">
      <div class="upper-container">
        <div class="content-header">
          <div class="title">My DAQ</div>
          <div class="subtitle">
            <b>Automatizar</b> tu negocio de forma escalable ya no es un mito
          </div>
        </div>
        <div class="image">
          <img src="~assets/img/home.svg" alt="Home" style="width: 50%;">
        </div>
      </div>
      <div class="description">
        Con el sistema de adquisición de datos <b>MyDAQ</b> puedes hacer crecer tu negocio, teniendo automatizaciones parciales o totales dependiendo de tus necesidades, y lo mejor, tener la información de tu negocio en tiempo real a solo un click.
      </div>
    </div>
    <div class="bottom" style="height: 40vh">
      <div class="col-information">
        <div class="col-item">
          <div class="item-title">
            <div class="icon"></div>
            <b>Entrada analógicas</b>
          </div>
          <div class="item-text">
            Mediante las entradas analógicas puedes conectar una gran variedad de sensores que hacen parte de tu proceso industrial 
          </div>
        </div>
        <div class="col-item">
          <div class="item-title">
            <div class="icon"></div>
            <b>Salidas analógicas</b>
          </div>
          <div class="item-text">
            Gracias a las salidas analógicas se pueden realizar lazos de control e influir directamente en los actuadores 
          </div>
        </div>
        <div class="col-item">
          <div class="item-title">
            <div class="icon"></div>
            <b>Conectividad</b>
          </div>
          <div class="item-text">
            Gracias a su diseño con conectividad inalámbrica (WiFi), puedes subir tus datos directamente a la nube y procesarlos
          </div>
        </div>
      </div>
      <div class="button-action">
        <div class="button">
          <nuxt-link to="/demo"><p class="button-text">Demo</p></nuxt-link>
        </div>
      </div>
    </div>
  </main>
</template>



<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.content-header {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 50vw;
}

.image {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 40vw;
}

.upper-container {
  display: flex;
  flex-direction: row;
  margin-top: 8vh;
}

.bottom {
  background-color: #9FA9D0;
  color: white;
  display: flex;
  flex-direction: column;
}

.title {
  font-family: 'Rasa';
  color: #4B5B85;
  font-style: normal;
  font-weight: bold;
  font-size: 72px;
  line-height: 88px;
  margin-bottom: 100px;
}

.subtitle {
  font-family: 'Rasa';
  font-style: normal;
  font-size: 36px;
  line-height: 44px;
  color: #475071;
  padding: 30px 10vw 30px 10vw;
}

.description {
  font-family: 'Rasa';
  font-style: normal;
  font-weight: normal;
  font-size: 28px;
  line-height: 34px;
  color: #475071;
  padding: 0px 20vw 20px 20vw;
  text-align: center;
}

.links {
  padding-top: 15px;
}

.col-information {
  display: flex;
  flex-direction: row;
}

.col-item {
  padding: 3%;
}

.item-title {
  font-family: 'Rasa';
  font-style: normal;
  font-size: 36px;
  line-height: 44px;
}

.item-text {
  font-family: 'Rasa';
  font-style: normal;
  font-weight: normal;
  font-size: 22px;
  line-height: 26px;
  text-align: left;
}

.button-action {
  display: flex;
  justify-content: center;
  padding: 2vh;
  height: 20vh;
}

.button {
  background-color: #4B5B85;
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  border-radius: 20px;
  width: 20vw;
  height: 8vh;
  border: none;
}

.button:hover {
  box-shadow: 0px 6px 6px rgba(255, 255, 255, 0.5);
}

.button-text {
  color: white;
  font-family: Rasa;
  font-style: normal;
  font-weight: bold;
  font-size: 50px;
  line-height: 73px;
}
</style>
