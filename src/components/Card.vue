<template>
    <div class="card">
        <div class="card__visible">
            <div class="card__image"></div>
        </div>
        <div class="card__hidden">
            <p class="card__hidden__title">{{title}}</p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Card',
    props: ['title', 'info']
}
</script>

<style>
.card{
    width: 100%;
    height: 400px;
    position: relative;
    cursor: pointer;
    overflow: hidden;
}
.card__visible{
    width: 100%;
    height: 400px;
    background-color: #EEEEEE;
}
.card__hidden{
    position: absolute;
    width: 100%;
    height: 80px;
    left: 0;
    bottom: -80px;
    background: rgba(0,0,0,.8);
    padding: 10px 20px;
    transition: all .3s;
}
.card__hidden__title{
    color: white;
    text-align: center;
    font-weight: 300;
}
.card:hover > .card__hidden{
    bottom: 0;
}
</style>