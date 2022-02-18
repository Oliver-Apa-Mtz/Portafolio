<template>
    <footer class="footer">
        <div class="footer__division">
            <p>©2022 Oliver Aparicio Martinez - All Rights Reserved.</p>
        </div>
        <div class="footer__division">
            <div class="footer__social">
                <a href="https://www.facebook.com/oliver.zowi" target="blank">
                    <img src="../../assets/icon-fb.svg" alt="">
                </a>
                <a href="https://www.instagram.com/oliver_apma/" target="blank">
                    <img src="../../assets/icon-ig.svg" alt="">
                </a>
                <a href="https://twitter.com/OliverMtz21" target="blank">
                    <img src="../../assets/icon-tw.svg" alt="">
                </a>
                <a href="https://github.com/Oliver-Apa-Mtz" target="blank">
                    <img src="../../assets/icon-gh.svg" alt="">
                </a>
                <a href="https://www.linkedin.com/in/oliver-aparicio-martinez" target="blank">
                    <img src="../../assets/icon-li.svg" alt="">
                </a>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'Footer'
}
</script>

<style>
.footer{
    height: 100px;
    border-top: 1px solid lightgray;
    margin: 0 50px 50px;
    background-color: #f9f9f9;
    padding: 50px;
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.footer__social a{
    margin-left: 10px;
}
.footer__social a img{
    width: 30px;
}
.footer__division p{
    font-size: 1.6rem;
    font-weight: 300;
}
@media(max-width: 1023px){
    .footer{
        padding: 20px;
        margin-bottom: 20px;
    }
    .footer__division p{
        font-size: 1.4rem;
    }
    .footer__social a{
        margin-left: 5px;
    }
}
@media(max-width: 639px){
    .footer{
        display: inline-block;
        text-align: center;
        height: auto;
    }
    .footer__division p{
        font-size: 1.2rem;
        margin-bottom: 20px;
    }
}
</style>