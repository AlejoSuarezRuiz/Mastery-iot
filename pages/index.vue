<template>
  <main>
    <section>
      <div class="content-header">
        <h2>My DAQ</h2>
        <span>
          <strong>Automatizar</strong> tu negocio de forma escalable ya no es un mito
        </span>
      </div>
      <div class="image">
        <img src="~assets/img/home.svg" alt="Home">
      </div>
      <p>
        Con el sistema de adquisición de datos MyDAQ puedes hacer crecer tu negocio, teniendo automatizaciones parciales o totales dependiendo de tus necesidades, y lo mejor, tener la información de tu negocio en tiempo real a solo un click.
      </p>
    </section>
    <section>
      <div class="col-information">
        <div class="col-item">
          <div class="item-title">
            <div class="icon"></div>
            <h4>Entrada analógicas</h4>
          </div>
          <div class="item-text">
            Mediante las entradas analógicas puedes conectar una gran variedad de sensores que hacen parte de tu proceso industrial 
          </div>
        </div>
        <div class="col-item">
          <div class="item-title">
            <div class="icon"></div>
            <h4>Salidas analógicas</h4></div>
          <div class="item-text">
            Gracias a las salidas analógicas se pueden realizar lazos de control e influir directamente en los actuadores 
          </div>
        </div>
        <div class="col-item">
          <div class="item-title">
            <div class="icon"></div>
            <h4>Conectividad</h4></div>
          <div class="item-text">
            Gracias a su diseño con conectividad inalámbrica (WiFi), puedes subir tus datos directamente a la nube y procesarlos
          </div>
        </div>
      </div>
      <div class="button-action">
        <nuxt-link to="/demo">demo</nuxt-link>
      </div>
    </section>
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

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
