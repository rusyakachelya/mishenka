<template>
    <div class="main-footer">
      <div class="footer-box">
        <div class="footer__card">
            <img class="footer__card-img" :src="getFooterCardImg" alt="">
            <div class="footer__card-title">Mat Simon</div>
            <div class="footer__card-subtitle">Professional UI/UX designer</div>
        </div>
        <div class="footer__content">
            <!-- <img class="footer__content-img" :src="getFooterImg" alt=""> -->
            <p class="footer__content-text">User interface design or user interface engineering is the design of user interfaces for machines and software, such as computers, home appliances, mobile devices, and other electronic devices, with the focus on maximizing usability and the user experience.</p>
        </div>
      </div>
    </div>
</template>

<script>
import FooterCard from '@/assets/images/footer-card.svg'
import FooterContent from '@/assets/images/footer-content.png'

export default {
  name: 'main-footer',
  components: {
    
  },
  data() {
    return {
        FooterCard,
        FooterContent,

    }
  },
  computed: {
     getFooterCardImg() {
        return this.FooterCard
    },
     getFooterImg() {
        return this.FooterContent
    },
  },
}
</script>

<style>
    .main-footer{
        background: rgba(12, 79, 249, 0.39);
        padding: 20px 80px 30px 140px;
        margin-top: 200px;
    }
    .footer-box{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .footer__content{
        display: flex;
    }
    .footer__content-img{
        /* position: absolute; */
    }
    .footer__card{
        width: 300px;
        height: 235px;
        background: #FFFFFF;
        border-radius: 22px;
        position: relative;
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: column;
    }
    .footer__card-img{
        position: absolute;
        top: -40px;
        right: 100px;
    }
    .footer__card-title{
        font-family: 'Poppins';
        font-style: normal;
        font-weight: 700;
        font-size: 23px;
        line-height: 34px;
    }
    .footer__card-subtitle{   
        font-family: 'Poppins';
        font-style: normal;
        font-weight: 400;
        font-size: 21px;
        line-height: 32px;
        letter-spacing: 0.07em;
        max-width: 240px;
    }
    .footer__content-text{
        max-width: 600px;
        font-family: 'Poppins';
        font-style: normal;
        font-weight: 400;
        font-size: 22px;
        line-height: 30px;
        letter-spacing: 0.01em;
        position: relative;
    }
    .footer__content-text::before{
        content: url('/src/assets/images/footer-content.png');
        position: absolute;
        left: -400px;
        bottom: -94px;
    }
</style>
