<template>
  <main>
      <div class="bg light-container">
        <h1>Music Is Life</h1>
        <div class="divider"></div>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus excepturi numquam unde cumque repudiandae recusandae inventore molestias quam perspiciatis, nihil, omnis et laborum, voluptate natus? Fugit voluptates accusamus modi nisi.</p>
    </div>

    <div class="bg dark-container">
        <h1>Latest Band News</h1>
        <div class="divider"></div>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus excepturi numquam unde cumque repudiandae recusandae inventore molestias quam perspiciatis, nihil, omnis et laborum, voluptate natus? Fugit voluptates accusamus modi nisi.</p>
    </div>
    
    <div class="banner">
      <div class="container">
        <div class="col-left">
          <div class="card">
            <img src="../assets/img/blog-post1-400x600.jpg" alt="">
            <div class="card-text">
              <h1>Taking it back to the old school</h1>
              <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Mollitia, quis voluptates?</p>
            </div>
          </div>
        </div>
        <div class="col-right">
          <div class="card">
            <img src="../assets/img/blog-post1-400x600.jpg" alt="">
            <div class="card-text">
              <h1>Taking it back to the old school</h1>
              <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Mollitia, quis voluptates?</p>
            </div>
          </div>
          <div class="card">
            <img src="../assets/img/blog-post2-400x600.jpg" alt="">
            <div class="card-text">
              <h1>Sharing the stage with a legend</h1>
              <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Mollitia, quis voluptates?</p>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="red-container">
      <a href="">VIEW ALL LATEST NEWS</a>
    </div>
    
    <div class="jumbotron">
      <div>
        <h1>"I just listened to it and said to myself, "Man, I really love this album." Still, today, it just sounds so fresh. It sounds full of ideas. These guys knew what they were doing. They' re good. And they're inventive. I haven' t heard anything this year that's ad inventite. I don' t really expect to."</h1>
        <i class="fas fa-play"></i>
      </div>
    </div>

    <div class="bg dark-container">
        <h1>Live Dates</h1>
        <div class="divider"></div>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus excepturi numquam unde cumque repudiandae recusandae inventore molestias quam perspiciatis, nihil, omnis et laborum, voluptate natus? Fugit voluptates accusamus modi nisi.</p>
        <ul v-for="(element, index) in liveDates" :key="index">
          <li>
            <a href="">
              <i class="fas fa-plus"></i>
              {{ element.date }} {{ element.name }} {{ element.state }}
            </a>
          </li>
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
@import "../style/common.scss";
    

    .bg {
        padding: 5% 20%;
        text-align: center;

        h1 {
          color: white;
        }
        p {
          color: #7D7B8D;
          line-height: 1.5rem;
        }
    }
    .light-container {
        background-color: $brand-primary-bg-light-color;
    }
    .dark-container {
        background-color: $brand-primary-bg-color;

        ul li{
          color: $brand-primary-btn-color;
          background-color: $brand-primary-bg-light-color;
          padding: 5px;
          margin: 10px 0;
          font-size: 0.8rem;
          text-align: start;
        }
        i {
          color: white;
          font-size: 0.5rem;
          padding: 0.8rem;
        }
    }
    .banner {
      .container {
        display: flex;
        min-height: 500px;
        background-color: $brand-primary-bg-color;
        padding: 0 15% 5%;
        
        .col-left {
          height: 100%;
          width: 100%;
        }
        .col-right {
          height: 100%;
          width: 70%;
          margin-left: 10px;
        }
        .card {
          img {
            width: 100%;
            }
            .card-text {
              background-color: $brand-primary-bg-light-color;
              padding: 20px;
              font-size: 0.7rem;
              h1 {
                color: $brand-primary-btn-color;
              }
              p {
                  color: #7D7B8D;
                  line-height: 1.5rem;
              }
          }
        }
      }
    }
    .red-container {
      text-align: center;
      background-color: $brand-primary-btn-color;
      height: 80px;
      line-height: 80px;
      font-size: 0.8rem;
      color: white;
      cursor: pointer;
      transition: .5s;
    }
    .red-container:hover {
        background-color: white;
        color: black;
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
          line-height: 1.5rem;
        }
        i {
          background-color: #ea4a56;
          color: white;
          padding: 1.2rem;
          border-radius: 50%;
          margin: 2rem 0;
        }
      }
    }

</style>