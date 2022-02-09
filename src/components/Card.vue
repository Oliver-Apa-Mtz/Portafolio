<template>
    <div class="card">
        <div class="card__visible">
            <div class="card__image" :class="{'card__image--small' : type == 'project'}">
                <img v-if="data.image" :src="require(`../assets/${data.image}`)" alt="">
            </div>
        </div>
        <div class="card__hidden">
            <p class="card__hidden__title">{{data.title}}</p>
            <p class="card__hidden__year">{{data.year}}</p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Card',
    props: ['data', 'type']
}
</script>

<style>
.card{
    width: 100%;
    height: 400px;
    position: relative;
    cursor: pointer;
    overflow: hidden;
    background-color: #EEEEEE;
}
.card__visible{
    width: 100%;
    height: 100%;
    
}
.card__hidden{
    position: absolute;
    width: 100%;
    height: 60px;
    left: 0;
    bottom: -80px;
    background: rgba(0,0,0,.8);
    padding: 5px 20px 0px;
    transition: all .3s;
}
.card__hidden__title, .card__hidden__year{
    color: white;
    text-align: center;
    font-weight: 300;
}
.card__hidden__year{
    font-size: 1rem;
    margin-bottom: 0px;
}
.card:hover > .card__hidden{
    bottom: 0;
}
.card__image{
    width: 100%;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
}
.card__image:hover > img{
    transform: scale(1);
}
.card__image img{
    width: 70%;
    transition: all .2s linear;
    transform: scale(.7);
}
.card__image--small img{
    width: 50%;
}
</style>