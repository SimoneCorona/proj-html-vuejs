<template>
   <li>
        <a href="">
            <i class="fas fa-plus"></i>
            {{ live.date }} {{ live.name }} {{ live.state }}
        </a>
    </li>
</template>

<script>
export default {
    name: 'MyLiveDates',

    props: {
       live: Object,
    }
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
</style>