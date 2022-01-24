<template>
    <div class="banner">
        <div class="banner__contain">
            <div class="banner__contain__text">
                <p>Bienvenido</p>
                <h1>Oliver Aparicio Martinez</h1>
                <h2>Desarrollador FrontEnd</h2>
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
}
.banner__contain{
    width: 100%;
    height: 600px;
    /*background-image: url('../assets/banner.jpg');*/
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center center;
    padding: 0 50px;
    background-color: #EEEEEE;
}
.banner__contain__text{
    width: 100%;
    text-align: right;
    padding: 40px;
}
h1{
    font-size: 6rem;
    font-weight: 700;
    letter-spacing: 2px;
}
h2{
    font-size: 2.6rem;
    font-weight: 400;
    letter-spacing: 2px;
}
p{
    font-size: 2rem;
}
</style>