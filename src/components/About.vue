<template>
    <div class="about" id="about">
        <div class="about__item">
            <div class="about__item--image"></div>
        </div>
        <div class="about__item">
            <div class="about__item--info">
                <h3 class="about__item--title">Sobre mí</h3>
                <p class="about__item--text">Apasionado en el desarrollo web, con más de 4 años de experiencia aprendiendo nuevas tecnologias y nuevas herramientas, me motiva cada conocimiento obtenido, me fascina todo el proceso que conlleva un proyecto web, desde que comienza con un diseño hasta verlo reflejado en un computador o un celular. Interesado en aprender mas cosas tales como diseño en interfaces ( UI ) y en la generación de buena experiencia al usuario ( UX ), con la finalidad de ser un desarrollador FullStack.</p>
                <a href="#experiences" class="about__item--btn">Experiencia</a>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'About',
}
</script>

<style>
.about{
    width: 100%;
    padding: 50px;
    display: flex;
}
.about__item{
    width: 50%;
    height: 600px;
    display: flex;
    align-items: center;
    justify-content: center;
}
.about__item--image{
    width: 100%;
    height: 600px;
    background-image: url('../assets/person.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center center;
    filter: grayscale(1);
}
.about__item--info{
    width: 100%;
    max-width: 500px;
    padding: 0 20px;
}
.about__item--text{
    font-size: 2rem;
    line-height: 3rem;
    margin: 30px 0;
}
.about__item--btn{
    width: max-content;
    font-size: 2.2rem;
    font-weight: 700;
    cursor: pointer;
    position: relative;
    padding: 4px 15px;
}
.about__item--btn::before{
    position: absolute;
    left: 0;
    top: 0;
    content: "";
    height: 100%;
    width: 45%;
    background: lightgray;
    z-index: -1;
    transition: all .5s ease-in-out;
}
.about__item--btn:hover::before{
    width: 100%;
}

@media(max-width: 1023px){
    .about{
        flex-wrap: wrap;
    }
    .about__item{
        width: 100%;
        height: auto;
    }
    .about__item--image{
        width: 60%;
        height: 400px;
        margin-bottom: 40px;
    }
}
@media(max-width: 639px){
    .about__item--image{
        width: 60%;
        height: 300px;
        margin-bottom: 40px;
    }
}
</style>