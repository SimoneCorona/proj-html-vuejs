<template>
  <div>
    <MyHeader :menù="element"/>
    <MyMain />
    <MyFooter :menù="element" />
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
            menùOptions: [
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
