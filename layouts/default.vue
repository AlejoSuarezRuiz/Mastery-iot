<template>
  <div style="display: flex">
    <div class="navbar">
      <div class="logo">
        <img src="~assets/img/logo.png" alt="Logo" width="50" height="50">
      </div>
      <nav>
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
      </nav>
    </div>
    <div style="width:95vw">
      <nuxt /> 
    </div>
  </div>
</template>

<style>

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