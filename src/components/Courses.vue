<template>
    <div class="projects">
        <div class="projects__title">
            <h3>Certificaciones</h3>
            <p>Certificaciones obtenidas mediante distintas plataformas en lo largo de mi trayectoria</p>
        </div>
        <div class="projects__random">
            <div class="projects__random__division">
                <div class="projects__cards__item" v-for="(item, i) in courses" :key="'courses'+i">
                    <Card :data="item"></Card>
                </div>
            </div>
            <div class="projects__random__division">
                <div class="projects__cards__item" v-for="(item, i) in desing" :key="'desing'+i">
                    <Card :data="item"></Card>
                </div>
            </div>
            <div class="projects__random__division">
                <div class="projects__cards__item" v-for="(item, i) in more" :key="'othres'+i">
                    <Card :data="item"></Card>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import Card from './Card.vue'
export default {
    name: 'Courses',
    components: { Card },
    data: function () {
        return {
            courses: [
                {
                    title: 'Diplomado Front End Web Developer',
                    year: '2021',
                    image: 'uvm.png'
                },
                {
                    title: 'Curso de Introducción al Desarrollo Web',
                    year: '2016',
                    image: 'google.png'
                }
            ],
            desing: [
                {
                    title: 'Curso de ECMAScript 6+',
                    year: '2022',
                    image: 'js.png'
                },
                {
                    title: 'Curso de Figma para Frontends',
                    year: '2021',
                    image: 'figma.webp'
                }
            ],
            more: [
                {
                    title: 'Curso de Inglés para Principiantes',
                    year: '2022',
                    image: 'ingles.png'
                }
            ]
        }
    }
}
</script>

<style>
.projects__random{
    width: 100%;
    padding: 10px 0;
    display: flex;
}
.projects__random__division{
    width: 33%;
    padding: 0 5px;
}
.projects__random__division .projects__cards__item{
    width: 100%;
    margin-bottom: 10px;
}
.projects__random__division .projects__cards__item .card{
    height: auto;
    padding: 20px 0;
}
</style>