<template>
  <footer>
    <div class="upper-footer">
       <div class="avada-container">
          <img src="../assets/img/avada-music-logo.png" alt="">
        </div>
        <div class="menu">
          <p v-for="(element, index) in menu" :key="index"><a href="">{{ element }}</a></p>
        </div>
    </div>
    
    <div class="down-footer">
       <div>
          <p>&copy; Copyright 2012 -2020 |</p>
          <p>AVADA THEME BY THEMEFUSION |</p>
          <p>ALL RIGHTS RESERVED |</p>
          <p>POWERED BY WORDPRESS</p>
        </div>
        <div>
          <a href="https://it-it.facebook.com/"><i class="fab fa-facebook-f"></i></a>
          <a href="https://twitter.com/"><i class="fab fa-twitter"></i></a>
          <a href="https://www.instagram.com/"><i class="fab fa-instagram"></i></a>
          <a href="https://www.youtube.com/"><i class="fab fa-youtube"></i></a>
        </div>
    </div>
  </footer>
</template>

<script>
export default {
    name: 'MyFooter',

    props: {
       menu: Array,
    },
}
</script>

<style scoped lang="scss">
@import "../style/variable.scss";
@import '~@fortawesome/fontawesome-free/css/all.min.css';

.upper-footer {
  background-color: $brand-primary-bg-light-color;
  padding: 30px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  color: #7D7B8D;
      
    .menu{
      display: flex;
      p {
        margin: 0 10px;
      }
      p:hover{
        color: white;
      }
    }
}
.down-footer {
  background-color: $brand-primary-bg-color;
  height: 80px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  color: #7D7B8D;
  padding: 0 30px;
  font-size: 0.7rem;

  p {
    display: inline-block;
    margin-right: 4px;
    font-weight: bold;
  }
  .fab {
    background-color: $brand-primary-bg-light-color;
    font-size: 1.2rem;
    height: 45px;
    width: 45px;
    padding: 0.8rem;
    margin: 0 10px;
    cursor: pointer;
  }
}
</style>