<template>
    <div class="projects">
        <div class="projects__title">
            <h3>Proyectos Freelances</h3>
            <p>Proyectos trabajados en conjunto de forma independiente</p>
        </div>
        <div class="projects__cards projects__cards--custom">
            <div class="projects__cards__item" v-for="(item, i) in freelances" :key="'freelances'+i">
                <Card :data="item"></Card>
            </div>
        </div>
    </div>
</template>

<script>
import Card from './Card.vue'
export default {
    name: 'Freelances',
    components: { Card },
    data: function () {
        return {
            freelances: [
                {
                    title: 'Página Web - Referee Pro',
                    year: '2018 - 2019',
                },
                {
                    title: 'Sistema Web - Asefis Consultores',
                    year: '2019 - 2020',
                }
            ]
        }
    }
}
</script>

<style>
.projects__cards--custom{
    justify-content: flex-start !important;
}
.projects__cards--custom .projects__cards__item{
    margin-right: 20px;
}
</style>