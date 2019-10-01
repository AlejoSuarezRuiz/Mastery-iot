<template>
  <div style="display: flex">
    <div class="navbar">
      <div class="logo">
        <img src="~assets/img/logo.png" alt="Logo" width="50" height="50">
      </div>
      <nuxt-link to="/" exact-active-class="active">
        <div class="tabItem">
          Inicio
        </div>
      </nuxt-link>
      <nuxt-link to="/demo">
        <div class="tabItem">
          demo
        </div>  
      </nuxt-link>
      <nuxt-link to="/data">
        <div class="tabItem" >
          Data
        </div>
      </nuxt-link>
    </div>
    <div style="width:95vw">
      <nuxt /> 
    </div>
  </div>
</template>

<style>
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.logo {
  background-color: #504A76;
  height:10vh; 
  color:white;
  display: flex;
  justify-content: center;
  align-items: center;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}

.tabItem {
  height:10vh;
  display:flex;
  align-items: center;
  justify-content: center;
  font-family: 'Rasa';
  font-style: normal;
  font-weight: bold;
  font-size: 24px;
  line-height: 29px;
  color: #B2B2B2;
}

.active .tabItem {
  color: #5870C6;
}

.navbar {
  box-shadow: 0px 6px 6px rgba(0, 0, 0, 0.5);
  background-color: #e4e9ed;
  width: 5vw;
  height: 100vh;
  display: flex;
  flex-direction: column;
}
</style>

<script>
export default {
  data() {
    return{
      'selected': 'inicio'
    }
  },
  methods: {
    isActiveTab(tabName) {
      console.log(this.selected);
      console.log(tabName);
      if(this.selected == tabName){
        return true;
      } else {
        return false;
      }
    },
    changeTab(tabName) {
      this.selected = tabName;
    }
  }
}
</script>