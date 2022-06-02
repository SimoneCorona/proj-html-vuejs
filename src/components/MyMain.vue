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
            <img src="../assets/img/blog_music_techo-600x300.jpg" alt="">
            <div class="card-text">
              <h1>Technology and music</h1>
              <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Mollitia, quis voluptates?</p>
            </div>
          </div>
          
          <section>
            <div class="card">
              <img src="../assets/img/blog-post3-200x300.jpg" alt="">
              <div class="card-text">
                <h1>While my guitar gently weeps</h1>
                <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Mollitia, quis voluptates?</p>
              </div>
            </div>
            <div class="card">
              <img src="../assets/img/blog-post4-200x300.jpg" alt="">
              <div class="card-text">
                <h1>It just sound better</h1>
                <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Mollitia, quis voluptates?</p>
              </div>
            </div>
          </section>
          
          
          <div class="card">
            <img src="../assets/img/blog_flavor_rock-600x300.jpg" alt="">
            <div class="card-text">
              <h1>The flavor of rock</h1>
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
        <img src="../assets/img/band_interview_play_icon.png" alt="">
      </div>
    </div>

    <div class="bg dark-container">
        <h1>Live Dates</h1>
        <div class="divider"></div>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus excepturi numquam unde cumque repudiandae recusandae inventore molestias quam perspiciatis, nihil, omnis et laborum, voluptate natus? Fugit voluptates accusamus modi nisi.</p>
        <ul>
          <MyLiveDates v-for="(element, index) in liveDates" :key="index" :live="element"/>
        </ul>
    </div>

    <div class="red-container">
      <a href="">VIEW ALL LATEST DATES</a>
    </div>

    
  </main>
</template>

<script>
import MyLiveDates from './MyLiveDates.vue'

export default {
    name: "MyMain",
    data() {
        return {
            liveDates: [
                {
                    date: "17/08/2020",
                    name: "GEM FESTIVAL 2020",
                    state: "ANAKALIA, GEORGIA",
                    showCard: true,
                },
                {
                    date: "24/9/2020",
                    name: "GROOVFEST",
                    state: "DOMINIC REPUBLIC",
                    showCard: true,
                },
                {
                    date: "31/10/2020",
                    name: "OASIS FESTIVAL 2020 MARRAKECH",
                    state: "MARRAKECH, MOROCCO",
                    showCard: true,
                },
                {
                    date: "07/11/2020",
                    name: "MOGA FESTIVAL -",
                    state: "ESSAOURIA, MOROCCO",
                    showCard: true,
                },
                {
                    date: "10/12/2020",
                    name: "ENVISION FESTIVAL -",
                    state: "UVITA, COSTA RICA",
                    showCard: true,
                },
            ],
        }
    },
    components: { MyLiveDates },
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
    }
    .banner {
      .container {
        display: flex;
        background-color: $brand-primary-bg-color;
        padding: 0 15% 20%;
        
        
        .col-left {
          height: 1300px;
          width: 100%;
          margin: 10px;
        }
        .col-right {
          height: 1300px;
          width: 70%;
          margin: 10px;
        }
        .card {
          margin-bottom: 1rem;
        }
        .card:hover {
          transition: .5s;
          filter: grayscale(100%) brightness(40%) sepia(100%) hue-rotate(-50deg) saturate(600%) contrast(0.7);
          
          h1 {
            position: absolute;
            top: 40%;
            left: 25%;
            color: white;
          }
          .card-text{
            background:none;
          }
          p {
              display: none;
          }
        }

          img {
            width: 100%;
            }
            .card-text {
              background-color: $brand-primary-bg-light-color;
              padding: 20px;
              font-size: 0.7rem;
              h1 {
                color: $brand-primary-btn-color;
                font-size: 1.2rem;
              }
              p {
                  color: #7D7B8D;
                  line-height: 1.5rem;
              }
          }
        }
        section {
          display: flex;
          flex-direction: column;
          flex-wrap: wrap;
          height: 500px;
          margin-bottom: 1rem;
          
          .card {
            width: 295px;
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
          margin-bottom: 2rem;
        }
        img {
          width: 70px;
        };
      }
    }

</style>