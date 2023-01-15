<template>
    <div class="main-header">
        <div class="main__header">
          <div class="container">
                <nav class="main__nav">
                <div class="main__logo">
                    <img :src="getLogoImg" alt="">
                </div>
                <div class="main__header-right">
                        <ul>
                            <li class="nav__item"><a href="">Home</a></li>
                            <li class="nav__item"><a href=""> About us</a></li>
                            <li class="nav__item"><a href=""> Log in</a></li>
                        </ul>
                    <div class="person__logo">
                        <img :src="getPersonImg" alt="">
                    </div> 
                </div>
                </nav>
            </div>
        </div>
    </div>
</template>

<script>
import MainLogo from '../../assets/images/main-logo.svg'
import PersonImg from '@/assets/images/person.svg'

export default {
  name: 'main-header',
  data() {
    return {
        headerImages: {main: MainLogo, person: PersonImg}
    }
  },
  computed: {
    getLogoImg() {
        return this.headerImages.main
    },
    getPersonImg() {
        return this.headerImages.person
    },
  },

}
</script>

<style>

</style>
