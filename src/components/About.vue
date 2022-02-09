<template>
    <div class="about">
        <div class="about__item">
            <div class="about__item--image"></div>
        </div>
        <div class="about__item">
            <div class="about__item--info">
                <h3 class="about__item--title">About</h3>
                <p class="about__item--text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Ducimus ex harum est eaque, pariatur praesentium enim ut corrupti quasi ipsum tempora officiis quod, cupiditate dicta eum, recusandae fugit quos? Numquam.</p>
                <div class="about__item--btn">Experiencia</div>
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
    font-size: 2.4rem;
    line-height: 3.4rem;
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
</style>