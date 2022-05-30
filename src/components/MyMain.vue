<template>
  <main>
      <div class="bg-light-container">
        <h1>Music Is Life</h1>
        <div class="divider"></div>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus excepturi numquam unde cumque repudiandae recusandae inventore molestias quam perspiciatis, nihil, omnis et laborum, voluptate natus? Fugit voluptates accusamus modi nisi.</p>
    </div>

    <div class="bg-dark-container">
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

    <div class="bg-dark-container">
        <h1>Live Dates</h1>
        <div class="divider"></div>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus excepturi numquam unde cumque repudiandae recusandae inventore molestias quam perspiciatis, nihil, omnis et laborum, voluptate natus? Fugit voluptates accusamus modi nisi.</p>
        <ul v-for="(element, index) in liveDates" :key="index">
          <li>{{ element.date }} {{ element.name }} {{ element.state }}</li>
        </ul>
    </div>

    <div class="red-container">
      <a href="">VIEW ALL LATEST DATES</a>
    </div>

    
  </main>
</template>

<script>
export default {
    name: 'MyMain',
    data() {
      return {
        liveDates: [
          {
            date: '17/08/2020',
            name: 'GEM FESTIVAL 2020',
            state: 'ANAKALIA, GEORGIA'
          },
          {
            date: '24/9/2020',
            name: 'GROOVFEST',
            state: 'DOMINIC REPUBLIC'
          },
          {
            date: '31/10/2020',
            name: 'OASIS FESTIVAL 2020 MARRAKECH',
            state: 'MARRAKECH, MOROCCO'
          },
          {
            date: '07/11/2020',
            name: 'MOGA FESTIVAL -',
            state: 'ESSAOURIA, MOROCCO'
          },
          {
            date: '10/12/2020',
            name: 'ENVISION FESTIVAL -',
            state: 'UVITA, COSTA RICA'
          },
        ]
      }
    }
}

</script>

<style scoped lang="scss">
@import "../style/variable.scss";
    
    .bg-light-container {
        background-color: $brand-primary-bg-light-color;
        padding: 5% 20%;
        text-align: center;
    }
    .bg-dark-container {
        background-color: $brand-primary-bg-color;
        padding: 5% 20%;
        text-align: center;
    }
    .red-container {
      text-align: center;
      background-color: $brand-primary-btn-color;
      height: 80px;
      line-height: 80px;

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