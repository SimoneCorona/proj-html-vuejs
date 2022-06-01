<template>
    <header>
        <div class="container-logo">
            <div>
                <img src="../assets/img/avada-music-logo.png" alt="">
            </div>
            <div>
                <i class="fas fa-bars"></i>
            </div>
            <div>
                <p v-for="(element, index) in menu" :key="index">{{ element }}</p>
            </div>
        </div>
        <div class="header-content">
            <h1>Untold Stories</h1>
            <h2>There is an untold story behind every favorite song.</h2>
            <section class="buttons">
                <button class="red-btn">LATEST ALBUM</button>
                <button class="transparent-btn">LIVE DATES</button>
            </section>
        </div>
        <div class="red-line"></div>
    </header>
</template>

<script>
export default {
    name: 'MyHeader',
    props: {
       menu: Array
    },
}
</script>

<style scoped lang="scss">
@import "../style/variable.scss";

    header{
        background-image: url(../assets/img/home_slider.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;
        color: white;
        height: 100vh;

        .container-logo {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 30px;
            
            i {
                font-size: 1.5rem;
            }
        }
        .header-content {
            text-align: center;

            h1 h2 {
                color: white;
            }
            h1 {
                margin-top: 6rem;
                font-size: 7rem;
            }
            h2 {
                margin-top: 1rem;
                font-size: medium;
                font-weight: lighter;
            }
            .buttons {
                margin: 3rem 0;

                button {
                    padding: 0.5rem 1.2rem;
                    margin: 0 10px;
                    color: white;
                    box-shadow: 0px;
                }
                .red-btn {
                    background-color: $brand-primary-btn-color;
                    border-color: $brand-primary-btn-color;
                }
                .transparent-btn {
                    background-color: transparent;
                    border-color: white;
                }
            }
        }
        .red-line {
                position: absolute;
                border-top: 10px solid $brand-primary-btn-color;
                width: 200px;
                bottom: -10px;
                left: 42%;
        }
    }
</style>