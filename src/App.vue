<template>
  <div>
    <HeaderComp :links="headerLinks" id="home" />
    <MainComp/>
    <footer>
      <FooterComp/>
    </footer>
  </div>
</template>

<script>
import FooterComp from './FooterComp.vue'
import 'bootstrap'
import MainComp from './components/MainComp.vue'
import HeaderComp from './components/HeaderComp.vue'
export default {
  name: 'App',
  data(){
    return{
      'headerLinks': [
/*        'home',
        'about',
        'projects',
        'process',
        'testimonials'*/
        {
          'title': 'home',
          'link': 'home'
        },
        {
          'title': 'about',
          'link': 'about'
        },
        {
          'title': 'projects',
          'link': 'projects'
        },
        {
          'title': 'process',
          'link': 'process'
        },
        {
          'title': 'testimonials',
          'link': 'testimonials'
        }
      ]
    }
  },
  components: {
    HeaderComp,
    MainComp,
    FooterComp,
  }
}
</script>

<style lang="scss">
@import "bootstrap/dist/css/bootstrap.min.css";
  .w80auto{
    width: 80%;
    margin: auto;
  }
      .btnLight{
      padding: 10px 20px;
      background-color: transparent;
      text-transform: uppercase;
      border: 1px solid #058283;
      color: white;
      font-weight: 700;
      border-radius: 5px;
      cursor: pointer;
      margin-left: 20px;
      }
      .btnGreen{
      padding: 10px 20px;
      text-transform: uppercase;
      background-color: #058283;
      color: white;
      font-weight: 700;
      border-style: none;
      border-radius: 5px;
      cursor: pointer;
      }
      .overlay{
      background-color: rgba(8, 9, 17, 0.466);
      }
    .greenText{
      color: #058283;
    }
    .greenBg{
    background-color: #DAECED;
  }      
</style>
