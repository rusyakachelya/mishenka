<template>
    <div class="login-page">
        <form class="login-form">
            <img class="login-img" :src="getLoginImg" alt="">
           <div class="form-inputs">
               <div class="input-box first">
                    <img :src="getUsernameImg" alt="">
                    <input type="text" placeholder="USERNAME">
                </div>
               <div class="input-box">
                    <img :src="getPasswordImg" alt="">
                    <input type="text" placeholder="PASSWORD">
                </div>
            </div> 
            <div class="login-links">
                <div class="reg-link">
                    <p>Dont have an accaunt?</p>
                    <a href="">Register</a>
                </div>
                 <input class="login-submit" type="submit" value="Login"> 
            </div>
        </form>
    </div>
</template>

<script>
import LoginImg from '@/assets/images/login-img.svg'
import UsernameImg from '@/assets/images/username.svg'
import PasswordImg from '@/assets/images/password.svg'


export default {
  name: 'login-page',
  components: {
    
  },
  data() {
    return {
        LoginImg,
        UsernameImg,
        PasswordImg
    }
  },
  computed: {
    getLoginImg() {
        return this.LoginImg
    },
    getUsernameImg() {
        return this.UsernameImg
    },
    getPasswordImg() {
        return this.PasswordImg
    },
  }

}
</script>


<style >
.input-box{
    padding: 12px 20px;
    border: 1px solid black;
    display: flex;
    align-items: center;
    margin-left: 20px;
    background: white;
}
.input-box img{
    margin-left: 20px;
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
    margin-bottom: 35px;
}
 .login-page{
    height: 100vh;
    background-color: #8EC5FC;
    background-image: linear-gradient(62deg, #8EC5FC 0%, #E0C3FC 100%);
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
    margin-bottom: 70px;
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
