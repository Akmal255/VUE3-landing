<template>
    <div class="footerSmart">
        <div class="wrapper">
            <div @click="Show" class="title">
                <p>О нас </p>
                <p v-if="!isActive">+</p>
                <p v-if="isActive">-</p>
            </div>
            <div class="hint" :class="{ show: isActive }">
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quam, accusantium!
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quam, accusantium!
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quam, accusantium!
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quam, accusantium!
            </div>
            <div @click="Show1" class="title">
                <p>Edu Coozin </p>
                <p v-if="!isActive1">+</p>
                <p v-if="isActive1">-</p>
            </div>
            <div class="hint" :class="{ show: isActive1 }">
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quam, accusantium!
            </div>
            <div @click="Show2" class="title">
                <p>Почему Coozin? </p>
                <p v-if="!isActive2">+</p>
                <p v-if="isActive2">-</p>
            </div>
            <div class="hint" :class="{ show: isActive2 }">
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quam, accusantium!
            </div>
            <div @click="Show3" class="title">
                <p> При поддержке</p>
                <p v-if="!isActive3">+</p>
                <p v-if="isActive3">-</p>
            </div>
            <div class="hint" :class="{ show: isActive3 }">
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quam, accusantium!
            </div>
        </div>
        <div class="links">
            <div class="social_apps">
                <div class="apps"><img src="../assets/images/instaSmart.png" alt="1"></div>
                <div class="apps"><img src="../assets/images/faceSmart.png" alt="2"></div>
                <div class="apps"><img src="../assets/images/youSmart.png" alt="3"></div>
            </div>
            <img src="../assets/images/coozin.png" alt="1">
        </div>
        <div class="copy">
        <p>&copy; 2021 Coozin · All Rights Reserved</p>
    </div>
    </div>
    <div class="footerWeb">
        <img src="../assets/images/coozin.png" class="footerCoolinz" alt="1">
        <div class="nav-links">
                <ul>
                    <li><a href="#">О нас</a></li>
                    <li><a href="#">Edu Coozin</a></li>
                    <li><a href="#">Почему Coozin?</a></li>
                    <li><a href="#">Мероприятия</a></li>
                </ul>
            </div>
            <div class="sponsor">
                <p>При поддержке </p>
                <img src="../assets/images/sponsor1.png" alt="">
                <img src="../assets/images/sponsor2.png" alt="">
            </div>
            <div class="subscribe">
                <p>ПОДПИСЫВАЙТЕСЬ НА НАС</p>
                <div class="line"></div>
                <div class="social_apps">
                <div class="apps"><img src="../assets/images/instaSmart.png" alt="1"></div>
                <div class="apps"><img src="../assets/images/faceSmart.png" alt="2"></div>
                <div class="apps"><img src="../assets/images/youSmart.png" alt="3"></div>
            </div>
            </div>
        <p>&copy; 2021 Coozin · All Rights Reserved</p>

    </div>
</template>

<script>
export default {
    name: "FooterComponent",
    data() {
        return {
            isActive: false,
            isActive1: false,
            isActive2: false,
            isActive3: false,
        }
    }
    ,
    methods: {
        Show() {
            this.isActive = !this.isActive
        },
        Show1() {
            this.isActive1 = !this.isActive1
        },
        Show2() {
            this.isActive2 = !this.isActive2
        },
        Show3() {
            this.isActive3 = !this.isActive3
        },
    },

}
</script>

<style  scoped>

.title {
    color: grey;
    text-align: left;
    border-bottom: 1px solid grey;
    padding: 12px 0;
    display: flex;
    justify-content: space-between;
}
.copy{
    margin-top: 28px;
font-size: 12px;
font-weight: 400;
line-height: 16px;
letter-spacing: 0em;

}
.footerCoolinz{
    width: 97px;
    height: 97px;
}
.subscribe{
    display: flex;
    gap: 20px;
    align-items: center;

}
.footerWeb{
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 40px;
    padding: 80px;
}
.sponsor{
    display: flex;
    justify-content: space-between;
    gap: 20px;
}
.nav-links{
    max-width: 475px;
    width: 100%;
}
.line{
    width: 64px;
    height: 5px;
    background-color: gray;
}
.nav-links ul{
display: flex;
justify-content: space-between;
}
.links{
    display: flex;
    justify-content: space-between;
    margin-top: 24px;
}
.social_apps{
    display: flex;
    gap: 10px;
    align-self: flex-end;
}
.apps, .apps img{
display: flex;
    width: 40px;
    height: 40px;
    align-items: center;
}
.footerSmart{
    display: none;
}
.hint {
    position: relative;
    opacity: 0;
    text-align: left;
    padding: 12px;
    visibility: hidden;
    height: 0;
    transition: all ease 0.5s;
    top: -300px;
}

.show {
    opacity: 1;
    visibility: visible;
    height: 100%;
    top: 0px;
}
@media only screen and (max-width: 430px) {
    .footerWeb{
        display: none;
    }
    .footerSmart{
        display: block;
    }
    .apps, .apps img{
        width: 24px;
        height: 24px;
    }
}
</style>