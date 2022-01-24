<template>
    <header class="header">
        <div class="header__logo">
            <img src="../../assets/logo.png" alt="">
        </div>
        <div class="header__nav">

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
    width: 100%;
    height: 100px;
    padding: 0 40px;
}
.header__logo{
    height: 100%;
    display: flex;
    align-items: center;
}
.header__logo img{
    height: 80px;
}
</style>