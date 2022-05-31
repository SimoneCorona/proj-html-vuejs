<template>
    <header>
        <div class="container-logo">
            <div>
                <img src="../assets/img/avada-music-logo.png" alt="">
            </div>
            <div>

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
    </header>
</template>

<script>
export default {
    name: 'MyHeader'
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
            padding: 30px;
        }
        .header-content {
            text-align: center;

            h1 h2 {
                color: white;
            }
            h1 {
                margin-top: 6rem;
                font-size: 4rem;
            }
            h2 {
                margin-top: 1rem;
                font-size: medium;
            }
            .buttons {
                margin: 3rem 0;

                button {
                    padding: 0.5rem 1.2rem;
                    margin: 0 10px;
                    color: white;
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
    }
</style>