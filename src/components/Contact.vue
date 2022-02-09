<template>
    <div class="contact">
        <div class="contact__header">
            <p class="contact__header--sub">Comenzemos un proyecto!</p>
            <h5 class="contact__header--title">Contactame</h5>
        </div>
        <div class="contact__body">
            <div class="contact__body__item">
                <p class="contact__body__item--title">Titulo</p>
                <p class="contact__body__item--text">500 South Main Street Bishop, CA 93514</p>
            </div>
            <div class="contact__body__item">
                <p class="contact__body__item--title">Titulo</p>
                <p class="contact__body__item--text">500 South Main Street Bishop, CA 93514</p>
            </div>
            <div class="contact__body__item">
                <p class="contact__body__item--title">Titulo</p>
                <p class="contact__body__item--text">500 South Main Street Bishop, CA 93514</p>
            </div>
            <div class="contact__body__item">
                <p class="contact__body__item--title">Titulo</p>
                <p class="contact__body__item--text">500 South Main Street Bishop, CA 93514</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Contact',
}
</script>

<style>
.contact{
    margin: 0 50px;
    background-color: #f9f9f9;
    padding: 50px;
}
.contact__header--sub{
    font-size: 1.8rem;
    font-weight: 300;
}
.contact__header--title{
    font-size: 6rem;
    font-weight: 700;
}
.contact__body{
    display: flex;
    margin: 100px 0 20px;
}
.contact__body__item{
    width: 25%;
    padding-right: 30px;
}
.contact__body__item--title{
    margin-bottom: 20px;
    font-weight: 700;
}
.contact__body__item--text{
    font-size: 1.8rem;
    font-weight: 300;
}
</style>