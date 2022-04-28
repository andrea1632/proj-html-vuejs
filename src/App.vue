<template>
  <div>
    <HeaderComp/>
    <MainComp/>
  </div>
</template>

<script>
import 'bootstrap'
import MainComp from './components/MainComp.vue'
import HeaderComp from './components/HeaderComp.vue'
export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp,
  }
}
</script>

<style lang="scss">
@import "bootstrap/dist/css/bootstrap.min.css";
  *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
  }
  .w80auto{
    width: 80%;
    margin: auto;
  }
</style>
