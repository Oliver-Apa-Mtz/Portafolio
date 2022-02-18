<template>
    <div class="projects" id="experiences">
        <div class="projects__title">
            <h3>Experiencia</h3>
            <p>Empresas para las cuales eh trabajado</p>
        </div>
        <div class="projects__cards">
            <div class="projects__cards__item" v-for="(item, i) in experience" :key="'card'+i">
                <a :href="item.url" target="_blank">
                    <Card :data="item" :type="'project'"></Card>
                </a>
            </div>
        </div>
    </div>
</template>

<script>
import Card from './Card.vue'

export default {
    name: 'Projects',
    components: { Card },
    data: function () {
        return {
            experience: [
                {
                    title: 'Intagono',
                    year: '2017 - 2019',
                    image: 'intagono.png',
                    url: 'https://intagono.com/'
                },
                {
                    title: 'Orderly',
                    year: '2019 - 2021',
                    image: 'orderly.png',
                    url: 'https://somosorderly.com/'
                },
                {
                    title: 'Dacodes',
                    year: '2021 - Actualmente',
                    image: 'dacodes.webp',
                    url: 'https://dacodes.com/'
                }
            ]
        }
    }
}
</script>

<style>
.projects{
    width: 100%;
    padding: 50px;
}
.projects__title{
    width: 100%;
    text-align: center;
    margin-bottom: 50px;
}
h3{
    font-size: 5rem;
    font-weight: 700;
    margin-bottom: 10px;
}
.projects__title p{
    font-size: 2rem;
    font-weight: 300;
}
.projects__cards{
    display: flex;
    justify-content: space-between;
}
.projects__cards__item{
    width: 33%;
    position: relative;
    transition: all .3s;
}
@media(max-width: 1023px){
    .projects__cards{
        flex-wrap: wrap;
    }
    .projects__cards__item{
        width: 49%;
        margin-bottom: 20px;
    }
}
@media(max-width: 639px){
    .projects__cards__item{
        width: 100%;
        margin-bottom: 40px;
    }
}
</style>