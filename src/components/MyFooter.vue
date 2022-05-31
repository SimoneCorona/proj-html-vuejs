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
          <p>Copyright 2012 -2020 |</p>
          <p>AVADA THEME BY THEMEFUSION |</p>
          <p>ALL RIGHTS RESERVED |</p>
          <p>POWERED BY WORDPRESS</p>
        </div>
        <div>
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
  line-height: 80px;

  p {
    display: inline-block;
    color: #7D7B8D;
    margin-right: 4px;
  }
}
</style>