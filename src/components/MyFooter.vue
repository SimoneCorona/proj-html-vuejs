<template>
  <footer>
    <div class="upper-footer">
       <div>
          <img src="../assets/img/avada-music-logo.png" alt="">
        </div>
        <div>

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
          <i class="fab fa-facebook-f"></i>
          <i class="fab fa-twitter"></i>
          <i class="fab fa-instagram"></i>
          <i class="fab fa-youtube"></i>
        </div>
    </div>
  </footer>
</template>

<script>
export default {
    name: 'MyFooter'
}
</script>

<style scoped lang="scss">
@import "../style/variable.scss";
@import '~@fortawesome/fontawesome-free/css/all.min.css';

.upper-footer {
  background-color: $brand-primary-bg-light-color;
  padding: 30px;
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
  }
}
</style>