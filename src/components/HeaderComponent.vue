<template>
    <div class="header">
        <div class="nvabar">
            <div class="burger-menu"><img src="../assets/images/Menu alt 2.png" alt="burger"></div>
            <img src="../assets/images/logo.png" alt="logo">
            <div class="nav-links">
                <ul>
                    <li><a href="#">О нас</a></li>
                    <li><a href="#">Edu Coozin</a></li>
                    <li><a href="#">Почему Coozin?</a></li>
                    <li><a href="#">Мероприятия</a></li>
                </ul>
            </div>
            <div class="basket">
                <div class="language">UZ</div>
                <button class="btn-registration">Присоединиться</button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "HeaderComponent",
}
</script>

<style scoped>
.nvabar {
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.basket{
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 5px;
}
.nav-links{
    max-width: 475px;
    width: 100%;
}
.nav-links ul{
display: flex;
justify-content: space-between;
}
.btn-registration {
    border-radius: 16px;
    background: #FF6600;
    max-width: 165px;
    height: 48px;
    color: white;
    padding: 16px;
}

.burger-menu {
    display: none;
}
.language {
        width: 48px;
        height: 48px;
        background: #F3F4F6;
        display: flex;
        justify-content: center;
        align-items: center;
        border-radius: 16px;
    }
@media only screen and (max-width: 430px) {
    .burger-menu {
        width: 24px;
        display: block;
        height: 24px;
    }
    .btn-registration, .nav-links{
        display: none;
    }
  
}</style>