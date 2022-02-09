<template>
    <div class="projects">
        <div class="projects__title">
            <h3>Experiencia</h3>
            <p>Empresas para las cuales eh trabajado</p>
        </div>
        <div class="projects__cards">
            <div class="projects__cards__item" v-for="(item, i) in experience" :key="'card'+i">
                <Card :data="item" :type="'project'"></Card>
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
                    image: 'intagono.png'
                },
                {
                    title: 'Orderly',
                    year: '2019 - 2021',
                    image: 'orderly.png'
                },
                {
                    title: 'Dacodes',
                    year: '2021 - Actualmente',
                    image: 'dacodes.webp'
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
    width: 30%;
}
</style>