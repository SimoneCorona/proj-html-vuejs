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


    header{
        background-image: url(../assets/img/home_slider.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;
        width: 100%;
        color: white;
        
        .container-logo {
            padding: 30px;
        }
        .header-content {
            text-align: center;

            .buttons {
                button {
                    padding: 0.5rem 1.2rem;
                }
                .transparent-btn {
                    background-color: transparent;
                }
            }
        }
    }
</style>