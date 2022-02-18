<template>
    <div class="contact" id="contact">
        <div class="contact__header">
            <p class="contact__header--sub">¡Comenzemos un proyecto!</p>
            <h5 class="contact__header--title">Contactame</h5>
        </div>
        <div class="contact__body">
            <div class="contact__body__item">
                <p class="contact__body__item--title">Dirección</p>
                <p class="contact__body__item--text">Benito Juarez sn, Col. Lombardo <br>Salina cruz, Oaxaca, México</p>
            </div>
            <div class="contact__body__item">
                <p class="contact__body__item--title">Email</p>
                <p class="contact__body__item--text">olivermtz35@gmail.com</p>
            </div>
            <div class="contact__body__item">
                <p class="contact__body__item--title">Teléfono / WhastApp</p>
                <p class="contact__body__item--text">(+52) 33 2480 6546</p>
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

@media(max-width: 1200px){
    .contact{
        padding: 20px 40px;
    }
    .contact__body{
        margin-top: 50px;
    }
    .contact__body__item{
        width: 33%;
    }
}
@media(max-width: 1023px){
    .contact{
        padding: 20px;
    }
    .contact__body{
        margin-top: 50px;
        flex-wrap: wrap;
        margin-bottom: 0px;
    }
    .contact__body__item{
        width: 50%;
        padding-right: 20px;
        margin-bottom: 40px;
    }
    .contact__body__item--title{
        margin-bottom: 10px;
    }
}
@media(max-width: 639px){
    .contact{
        text-align: center;
    }
    .contact__body__item{
        width: 100%;
        padding-right: 0px;
    }
    .contact__header--sub{
        font-size: 1.6rem;
        margin-bottom: 20px;
    }
    .contact__header--title{
        font-size: 4rem;
    }
}
</style>