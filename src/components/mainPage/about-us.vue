<template>
  <div class="about-us">
        <div class="container">
            <div class="about__text">
              <h2 class="about__title">About Us</h2>
              <div class="about__subtitle">
                <span>Who we are?</span><br>
                <span>What are we doing?</span><br>
                <span>Why you should start with UI/UX design </span>
              </div>
          </div>
        </div>
          <div class="about__portfolio">
              <div class="about__box">
                <img class="about__image" :src="getPortfolioImg" alt="">
                <h4>Age: 25</h4>
                <h4>Location: USA</h4>
              </div>
              <div class="about__descript">
                <div class="about__descr-text">Mat Simon,is a professional UI/UX designer from USA who will help you to learn everithing about UI/UX design
                </div>
                  <div class="about__us-answers">
                      <div class="about__us-quest">
                        <p>Who we are?</p>
                        <p>-We are a company from the USA that helps young, future designers</p>
                      </div>
                      <div class="about__us-quest center">
                        <p>What are we doing?</p>
                        <p>As we have already said, we help people learn UI / UX design</p>
                      </div>
                      <div class="about__us-quest">
                        <p>Why u should start with UI/UX</p>
                        <p>UI / UX design is very simple. All you need is a little imagination and creativity and you will master it quickly</p>
                      </div>
                  </div>
              </div>
          </div>
  </div>
</template>

<script>
import PortfolioImg from '@/assets/images/portfolio.png'

export default {
  name: 'about-us',
  components: {
    
  },
  data() {
    return {
        PortfolioImg,
    }
  },
  computed: {
     getPortfolioImg() {
        return this.PortfolioImg
    }
  }

}
</script>


<style >
 .about-us{
    margin-left: 115px;
    padding-top: 50px;
 }

</style>
