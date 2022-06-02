<template>
   <li>
        <i class="fas fa-plus"></i>
        <i class="fas fa-minus"></i>
        {{ live.date }} {{ live.name }} {{ live.state }}
        
        <div class="live-info">
            <img src="../assets/img/google-maps-satellite.jpg" alt="">
            <div>
                <h1>Untold Stories</h1>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Beatae possimus delectus dolore sunt, tempore quia fugiat magnam ducimus.</p>
                <button>BOOK NOW</button>
            </div>
        </div>
    </li>
</template>

<script>
export default {
    name: 'MyLiveDates',
   
    props: {
       live: Object,
    },
}

</script>

<style scoped lang="scss">
@import "../style/variable.scss";
@import "../style/common.scss";>

li {
    padding: 5px;
    margin: 10px 0;
}
i {
    color: white;
    font-size: 0.5rem;
    padding: 0.8rem;
}
.live-info {
    display: flex;
    flex-wrap: wrap;
    img{
        width: 200px;
        height: 150px;
        margin: 1rem;
    }
    div{
        width: 60%;
        margin: 1rem 1rem 0;
    }
    h1 { 
        font-size: 1rem;
        color: white;
        margin-bottom: 1rem;
    }
    p {
        color: #7D7B8D;
        line-height: 1.5rem;
    }
    button {
        padding: 0.5rem 1.2rem;
        margin-top: 30px;
        color: white;
        box-shadow: 0px;
        background-color: $brand-primary-btn-color;
        border-color: $brand-primary-btn-color;
        }
}
</style>