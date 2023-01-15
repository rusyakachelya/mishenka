<template>
  <div class="main-page">
      <main-header/>
      <main-body/>
      <about-us/>
      <main-footer></main-footer>
      <login-page></login-page>
      <registration-page/>
  </div>
</template>

<script>
import MainHeader from './main-header.vue'
import MainBody from './main-body.vue'
import AboutUs from './about-us.vue'
import MainFooter from './main-footer.vue'
import LoginPage from '../login-page.vue'
import RegistrationPage from '../registration-page.vue'

export default {
  name: 'main-page',
  components: {
    MainHeader,MainBody,AboutUs,MainFooter,LoginPage,RegistrationPage
  },
  data() {
    return {

    }
  },

}
</script>


<style >
  .main-page{
    padding-top: 40px;
  }
  .main__nav{
    display: flex;
    justify-content: space-between;
    text-align: center;
    align-items: center;
  }
  .main__nav ul{
    display: flex;
    margin-right: 150px;
  }
  .main__header-right{
    display: flex;
    align-items: center;
  }
  ul{
    padding-left: 0;
  }
  .nav__item{
    margin-right: 30px;
    font-family: 'Roboto';
    font-style: normal;
    font-weight: 400;
    font-size: 18px;
  }
  .nav__item:last-child{
    margin-right: 0px;
  }
  a{
    text-decoration: none;
    color: inherit;
  }
  .main__body{
    padding-top: 150px;
    max-width: 580px;
  }
  .body__title{
    font-family: 'Roboto';
    font-style: normal;
    font-weight: 500;
    font-size: 62px;
    line-height: 56px;
  }



  .about__text{
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .about__title{
    font-family: 'Roboto';
    font-style: normal;
    font-weight: 500;
    font-size: 52px;
    line-height: 56px;
    margin-right: 30px;
  }
  .about__subtitle{
    color: #BEAEAE;
    letter-spacing: 0.11em;
  }
  .about__portfolio{
    padding-top: 60px;
    display: flex;
  }
  .about__box{
    margin-right: 40px;
  }
  h4{
    margin: 5px 0;
    margin-left: 20px;
  }
  .about__image{
    margin-bottom: 15px;
  }
  .about__descr-text{
    margin-top: 50px;
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 700;
    font-size: 34px;
    line-height: 51px;
    letter-spacing: 0.08em;
    margin-bottom: 100px;
  }
  .about__us-answers{
    display: flex;
    height: 200px;
  }
  p{
    margin: 0;
  }
  .about__us-quest{
    width: 350px;
    height: 150px;
    background: #A0BAFD;
    margin-right: 15px;
  }
  .about__us-quest:last-child{
    margin-right: 0;
    align-self: flex-end;
  }
  .about__us-quest.center{
    align-self: center;
  }
  .about__us-quest p{
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 700;
    font-size: 20px;
    line-height: 28px;
    letter-spacing: 0.08em;
  }
  .about__us-quest:last-child p {
    font-size: 18px;
  }


</style>
