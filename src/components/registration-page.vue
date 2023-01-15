<template>
    <div class="registration-page">
        <form class="login-form">
            <img class="login-img" :src="getImage('UnRegistr')" alt="">
           <div class="form-inputs">
               <div class="input-box first">
                    <img :src="getImage('EmailImg')" alt="">
                    <input type="text" placeholder="EMAIL">
                </div>
               <div class="input-box first">
                    <img :src="getImage('UsernameImg')" alt="">
                    <input type="text" placeholder="USERNAME">
                </div>
               <div class="input-box">
                    <img :src="getImage('PasswordImg')" alt="">
                    <input type="text" placeholder="PASSWORD">
                </div>
            </div> 
            <div class="login-links">
                 <input class="login-submit" type="submit" value="Register"> 
            </div>
        </form>
    </div>
</template>

<script>
import UnRegistr from '@/assets/images/unregistr.svg'
import UsernameImg from '@/assets/images/username.svg'
import PasswordImg from '@/assets/images/password.svg'
import EmailImg from '@/assets/images/email-img.svg'


export default {
  name: 'registration-page',
  components: {
    
  },
  data() {
    return {
        images: {
            UnRegistr,
            UsernameImg,
            PasswordImg,
            EmailImg
        }
       
    }
  },
  methods: {
    getImage(key) {
        return this.images[key]
    }
  },
  computed: {
   
  }

}
</script>


<style scoped>
.input-box{
    /* padding: 12px 20px; */
    width: 400px;
    border: 1px solid black;
    display: flex;
    align-items: center;
    background: white;
    margin-left: 0px !important;
}

.input-box input{
   padding: 0px 50px;
   width: 100%;
    border: none;
}
.input-box input:focus{
    outline: none;
}
.first{
    margin-bottom: 20px;
}
 .registration-page{
    height: 100vh;
    background-image: linear-gradient( 135deg, #97ABFF 10%, #123597 100%);
    display: flex;
    justify-content: center;
    align-items: center;
 }
 .login-form{
    width: 600px;
    border-radius: 10px;
    background: #ffff;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    position: relative;
 }
 .login-img{
    width: 216px;
    height: 203px;
    position: absolute;
    top: -100px;
 }
 .form-inputs{
    max-width: 520px;
    margin: 0 auto;
    margin-bottom: 30px;
    padding-top: 150px;
 }
 .form-input{
    width: 510px !important;
    height: 50px;
 }
 .login-form input::placeholder{
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 400;
    font-size: 17px;
    line-height: 26px;
    letter-spacing: 0.1em;
    color: #000000;
 }

 .login-links{
    display: flex;
    align-items: center;
    padding-bottom: 60px;
 }
 .login-submit{
    width: 213px;
    height: 65px;
    background: #2F8CAD;
    border-radius: 12px;
    color: white;
    display: block;
    margin-left: 150px;
    cursor: pointer;
    border: none;
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 400;
    font-size: 27px;
    line-height: 48px;
    letter-spacing: 0.1em;
 }
 .reg-link a{
    text-decoration: underline;
    color: blue;
    align-self: flex-end;
 }
 .reg-link{
    display: flex;
    flex-direction: column;
 }
</style>
