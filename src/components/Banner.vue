<template>
    <div class="banner" id="home">
        <div class="banner__contain">
            <div class="banner__contain__text">
                <p>Bienvenido</p>
                <h1>Oliver Aparicio Martinez</h1>
                <h2>Front End Software Engineer</h2>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Banner'
}
</script>

<style>
.banner{
    padding: 0 50px;
    margin-bottom: 50px;
    margin-top: 100px;
}
.banner__contain{
    width: 100%;
    height: 600px;
    background-image: url('../assets/banner.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center center;
    padding: 0 50px;
}
.banner__contain__text{
    width: 100%;
    padding-top: 40px;
}
h1{
    font-size: 6rem;
    font-weight: 700;
    letter-spacing: 2px;
    text-shadow: 0px 4px 8px rgba(0,0,0,.3);
}
h2{
    font-size: 2.6rem;
    font-weight: 400;
    letter-spacing: 2px;
}
p{
    font-size: 2rem;
}

@media(max-width: 1200px){
    .banner__contain{
        height: 400px;
    }
}
@media(max-width: 1023px){
    .banner__contain{
        height: 320px;
    }
    .banner h1{
        font-size: 4rem;
    }
}
@media(max-width: 639px){
    .banner{
        margin-bottom: 20px;
    }
    .banner__contain{
        height: 250px;
        padding: 0 20px;
    }
    .banner__contain__text{
        padding: 0px;
        text-align: right;
        padding-top: 40px;
    }
    .banner h1{
        font-size: 2em;
    }
    .banner h2, .banner p{
        font-size: 1.8rem;
    }
}
</style>