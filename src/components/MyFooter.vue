<template>
  <footer>
    <div class="upper-footer">
       <div>
          <img src="../assets/img/avada-music-logo.png" alt="">
        </div>
        <div>
          <ul>
            <li></li>
          </ul>
        </div>
    </div>
    
    <div class="down-footer">
       <div>

        </div>
        <div>
          <ul>
            <li></li>
          </ul>
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

.upper-footer {
  background-color: $brand-primary-bg-light-color;
}
.down-footer {
  background-color: $brand-primary-bg-color;
}
</style>