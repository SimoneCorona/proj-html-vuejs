<template>
  <main>
      <div class="music_is_life_section">
        <h1>Music Is Life</h1>
        <div class="divider"></div>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus excepturi numquam unde cumque repudiandae recusandae inventore molestias quam perspiciatis, nihil, omnis et laborum, voluptate natus? Fugit voluptates accusamus modi nisi.</p>
    </div>

    <div class="latest_band_new_section">
        <h1>Latest Band News</h1>
        <div class="divider"></div>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus excepturi numquam unde cumque repudiandae recusandae inventore molestias quam perspiciatis, nihil, omnis et laborum, voluptate natus? Fugit voluptates accusamus modi nisi.</p>
    </div>
    
    <div class="banner">
      <div class="container">

      </div>
    </div>

    <div class="red-container">
      <a href="">VIEW ALL LATEST NEWS</a>
    </div>
    
    <div class="jumbotron">
      <div>
        <h1>"I just listened to it and said to myself, "Man, I really love this album." Still, today, it just sounds so fresh. It sounds full of ideas. These guys knew what they were doing. They' re good. And they're inventive. I haven't heard anything this year that's ad inventite. I don't really expect to."</h1>
        <i></i>
      </div>
    </div>

    <div class="latest_band_new_section">
        <h1>Live Dates</h1>
        <div class="divider"></div>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus excepturi numquam unde cumque repudiandae recusandae inventore molestias quam perspiciatis, nihil, omnis et laborum, voluptate natus? Fugit voluptates accusamus modi nisi.</p>
        

    </div>

    <div class="red-container">
      <a href="">VIEW ALL LATEST DATES</a>
    </div>

  </main>
</template>

<script>
export default {
    name: 'MyMain'
}
</script>

<style scoped lang="scss">
@import "../style/variable.scss";
    
    .music_is_life_section {
        background-color: $brand-primary-bg-light-color;
        padding: 5% 20%;
        text-align: center;
    }
    .latest_band_new_section {
        background-color: $brand-primary-bg-color;
        padding: 5% 20%;
        text-align: center;
    }
    .red-container {
      text-align: center;
      background-color: $brand-primary-btn-color;
      height: 100px;
      line-height: 100px;

      a {
        text-decoration: none;
        color: white;
      }
    }
    .jumbotron {
      background-image: url(../assets/img/home-testimonial-parallax.jpg);
      height: 700px;              
      background-size: cover;
      background-position: center;
      background-repeat: no-repeat;
      display: flex;
      justify-content: center;
      align-items: center;
      
      div {
        color: white;
        margin: 0 30%;
        text-align: center;
        font-style: italic;

        h1 {
          font-size: 1rem;
        }
      }
    }

</style>