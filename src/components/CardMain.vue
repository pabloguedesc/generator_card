<template>
  <div id="HomePage">
    <Navbar/>
    <main>
      <div class="main-container">
        <div>
          <h1 class="title">Seja Bem vindo!</h1>
            <h1 id="titleMain" class="title">ao <span class="textMain">Generator Card</span></h1>
          <p class="subtitle">O melhor gerador de cartões virtuais do Brasil</p>
          <p class="subtitle">- Alta performance</p>
          <p class="subtitle">- Novas formas de conseguir dinheiro</p>
          <div class="camp-btn">
            <input id="btn-start" class="btn" type="submit" value="Vamos começar!     ->">
            <input id="btn-more" class="btn" type="submit" value="Saiba mais">
          </div>
        </div>
      </div>
      <section class="credit-card">
        <div class="responsive-card">
          <div class="card">
            <div class="face front absolute">
              <img src="../assets/chip.svg" alt="Chip" id="chip" class="absolute">
              <img src="../assets/signal.svg" alt="Signal" id="signal" class="absolute">
              <img src="../assets/logo.svg" alt="Logo" id="logo" class="absolute">
              <p id="owner" class="absolute">PABLO R G COSTA</p>
            </div> 
            <div class="face back absolute">
              <div id="graybar" class="absolute"></div>
              <div id="card-info" class="absolute">
                <p id="card-number">1234 5678 9999 0000</p>
                <div class="flex">
                  <p class="flex informations">
                    <span class="label">MEMBER SINCE</span>
                    <span>01/01</span>
                  </p>
                  <p class="flex informations">
                    <span class="label">VALID THRU</span>
                    <span>12/29</span>
                  </p>
                  <p class="flex informations">
                    <span class="label">SECURITY CODE</span>
                    <span>271</span>
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div>
          <div class="circle left"></div>
          <div class="circle right"></div>
        </div>

      </section>

    </main>
  </div>
</template>

<script>

import Navbar from "../components/navbar.vue"

export default {
  data(){
    return{
    }
  },
  components:{
    Navbar
  }
}
</script>

<style scoped>  

#HomePage {
  background-color: var(--dark-gray);
  width: 100%;
  height: 100vh;
  display: flex;
}

main {
  display: flex;
  margin: 0 auto;
  width: 90%;
  justify-content: space-around;
}

.main-container {
  display: flex;
  align-items: center;
}

.main-container div{
  width: 100%;
  height: 50%;
}

.title{
  color: var(--white);
  font-size: 2.5rem;
  font-weight: 600;
}

#titleMain {
  margin-top: -20px;
}

.textMain{
  color: var(--yellow);
  font-size: 2.8rem;
  font-weight: 700;
  margin-top: -15px;
}

.subtitle{
  color: var(--white);
  font-size: 16px;
}

.camp-btn {
  margin-top: 2rem;
}

#btn-start {
  margin-right: 1.5rem;
  background: linear-gradient(-120grad, rgba(177, 165, 204, 0.623), rgba(158, 144, 190, 0.623), rgba(168, 150, 211, 0.623),rgba(130, 111, 173, 0.623), rgba(34, 27, 51, 0.623), rgba(0, 0, 0, 0.945));
  color: var(--white);
  border: 1px solid var(--white);
  box-shadow: rgba(255, 255, 255, 0.178) 0px 1px 2px 0px, rgba(255, 255, 255, 0.185) 0px 1px 3px 1px;
  width: 162px;
  transition: 0.5s;
}
#btn-start:hover{
  width: 202px;
}

#btn-more {
  margin-right: 1.5rem;
  background-color: rgba(0, 0, 0, 0);
  color: #ffffff9c;
  border: 1px solid rgb(130, 111, 173, 0.623);
  box-shadow: rgba(255, 255, 255, 0.178) 0px 1px 2px 0px, rgba(255, 255, 255, 0.185) 0px 1px 3px 1px;
  transition: 0.5s;
}

#btn-more:hover {
  color: var(--white);
  border: 1px solid var(--white);
  box-shadow: rgba(255, 255, 255, 0.664) 0px 1px 2px 0px, rgba(255, 255, 255, 0.911) 0px 1px 3px 1px;
}

.btn {
  font-size: 16px;
  font-weight: 500;
  padding: 12px;
  border-radius: 5px;
  border: none;
  cursor: pointer;
}


/* .circle.left {
  background-color: var(--purple);
  width: 200px;
  height: 200px;
  border-radius: 50%;
  margin: 12rem -9rem 0 0;
  box-shadow: rgba(192, 49, 49, 0.452) 0px 30px 90px;
  filter: blur(2px);
} */

/* .circle.right {
  background-color: rgb(177, 199, 97);
  width: 250px;
  height: 250px;
  border-radius: 50%;
  box-shadow: rgba(192, 49, 49, 0.452) 0px 30px 90px;
  filter: blur(2px);
  position: relative;
  margin: -14rem -35rem;
  z-index: 1;
} */

.flex {display: flex;}
.absolute {position: absolute;}

.credit-card {
  display: flex;
  align-items: center;
  width: 50%;
  justify-content: center;
}

.responsive-card {
  width: 80%;
  height: 50%;
}

.card {
  position: relative;
  width: 100%;
  height: 100%;
  transform-style: preserve-3d;
  perspective: 700px;
  z-index: 100;
}

.card .face {
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border: 1px solid rgba(255, 255, 255, 0.200);
  border-radius: 10px;
  background: linear-gradient(135deg, rgba(255, 255, 255, 0.100) 0%, transparent 100%);
  backdrop-filter: blur(10px);
  box-shadow: 2px 2px 0px 0px rgba(255, 255, 255, 0.150);
  transform-style: preserve-3d;
  transition: 1s ease-in-out;
  backface-visibility: hidden;
  transform: rotateY(0);
}

#chip {
  width: 60px;
  height: 60px;
  top: 100px;
  left: 50px;
}

#signal{
  width: 25px;
  height: 25px;
  top: 115px;
  left: 115px;
  transform: rotate(90deg);
}

#logo{
  width: 75px;
  height: 75px;
  bottom: 30px;
  left:40px;
}

#owner{
  bottom: 55px;
  left: 140px;
  font-size: 1.35rem;
  letter-spacing: 1px;
  color: white;;
}

.card .face.back {
  transform: rotateY(180deg);
}

#graybar {
  width: 100%;
  height: 50px;
  top: 15px;
  background: var(--gray);
}

#card-info {
  width: 100%;
  bottom: 15px;
  padding: 0 20px;
  color: var(--white);
}

.card-info .informations:not(:first-child) {
  margin-left: 10px;
}

.card-info .informations {
  align-items: center;
}

#card-info .flex .informations .label {
  display: block;
  font-size: 0.4rem;
  margin-left: 4px;
  width: 30px;
}

.card .face.front::before,
.card .face.front::after,
.card .face.back::before,
.card .face.back::after{
  content: "";
  position: absolute;
  width: 45px;
  height: 45px;
  border-radius: 50%;
  opacity: 0.75;
}

.card .face.front::before,
.card .face.front::after{
  top: 10px;
  mix-blend-mode: overlay;
}

.card .face.back::before,
.card .face.back::after{
  bottom: 10px;
  mix-blend-mode: hue;
}

.card .face.face.front::before,
.card .face.face.back::before {
  right: 20px; 
}

.card .face.face.front::after, 
.card .face.face.back::after {
  right: 45px; 
}

.card .face.front::before {
  background: var(--yellow);
}

.card .face.front::after{
  background: var(--red);
}

.card .face.back::before {
  background: var(--light-blue);
}

.card .face.back::after{
  background: var(--dark-blue);
}

.card:hover .face.front {
  transform: rotateY(180deg);
}

.card:hover .face.back {
  transform: rotateY(360deg);
}


</style>