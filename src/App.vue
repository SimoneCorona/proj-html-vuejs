<template>
  <div>
    <MyHeader :menu="menuOptions"/>
    <MyMain />
    <MyFooter :menu="menuOptions" />
  </div>
</template>

<script>
import MyHeader from "./components/MyHeader.vue"
import MyMain from "./components/MyMain.vue"
import MyFooter from "./components/MyFooter.vue"


export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,
    MyFooter,
  },

  data() {
        return {
            menuOptions: [
              'Home',
              'Meet The Band',
              'Live Dates',
              'Latest News',
              'Albums',
              'Fans'
            ],  
        };
      },
}        
</script>

<style lang="scss">
@import "./style/common.scss";
@import "./style/variable.scss"

</style>
