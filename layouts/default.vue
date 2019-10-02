<template>
  <div style="display: flex">
    <div class="navbar">
      <div class="logo">
        <nuxt-link to="/">
          <img src="~assets/img/icons/artificial-intelligence.svg" alt="Logo" width="50" height="50">
        </nuxt-link>
      </div>
      <nav class="navigation">
        <nuxt-link to="/" exact-active-class="active">
          <div class="tabItem">
          <i class="icon icon-home"></i>
            Home
          </div>
        </nuxt-link>
        <nuxt-link to="/demo" exact-active-class="active">
          <div class="tabItem">
          <i class="icon icon-pointer"></i>
          demo
          </div>  
        </nuxt-link>
        <nuxt-link to="/data" exact-active-class="active">
          <div class="tabItem" >
          <i class="icon icon-data"></i>
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