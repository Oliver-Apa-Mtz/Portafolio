<template>
    <header class="header">
        <div class="header__logo">
            <a href="#home">
                <img src="../../assets/logo.png" alt="">
            </a>
        </div>
        <div class="header__nav">
            <nav>
                <a href="#about">Sobre mí</a>
                <a href="#experiences">Experiencia</a>
                <a href="#courses">Certificaciones</a>
                <a href="#projects">Proyectos</a>
                <a href="#contact">Contacto</a>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    name: 'Header',
    data:() => ({
        active: 'guide'
    })
}
</script>

<style>
.header{
    position: fixed;
    z-index: 99;
    width: 100%;
    height: 70px;
    padding: 0 40px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: white;
    top: 0;
    left: 0;
    box-shadow: 0px 2px 6px rgba(0,0,0,.1);
}
.header__logo{
    height: 100%;
    display: flex;
    align-items: center;
}
.header__logo a{
    display: flex;
    align-items: center;
}
.header__logo img{
    height: 70px;
}
.header__nav{
    padding-right: 10px;
}
.header__nav a{
    text-decoration: none;
    margin-left: 20px;
    font-size: 1.6rem;
    font-weight: 300;
}
.header__nav a:hover{
    color: black;
}
@media(max-width: 639px){
    .header{
        padding: 0 20px;
    }
    .header__nav{
        padding-right: 0px;
    }
    .header__nav a{
        font-size: 1.2rem;
        margin-left: 8px;
    }
}
</style>