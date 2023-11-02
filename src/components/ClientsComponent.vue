<template>
    <div class="client-template">
        <h1>Наши довольные вендоры</h1>
        <swiper ref="{swiperRef}" :slides-per-view="count" :space-between="16" :loop="true" :modules="modules"
            :class="MySwiper">
            <swiper-slide>
                <div>
                    <div class="feedback-info">
                        <div class="t_frame">
                            <img src="../assets/images/tutuq.png" alt="img">
                        </div>
                        <p>When our designs need an expert opinion or approval, I know I can rely on your agency Thank you
                            for
                            all your help-I will be recommending you to everyone</p>
                    </div>
                    <div class="profile">
                        <div class="img">
                            <img src="../assets/images/User Image 01.png" alt="user">
                        </div>
                        <h1>Name</h1>
                        <p>Designation</p>
                    </div>
                </div>
            </swiper-slide>
            <swiper-slide>
                <div>
                    <div class="feedback-info">
                        <div class="t_frame">
                            <img src="../assets/images/tutuq.png" alt="img">
                        </div>
                        <p>When our designs need an expert opinion or approval, I know I can rely on your agency Thank you
                            for
                            all your help-I will be recommending you to everyone</p>
                    </div>
                    <div class="profile">
                        <div class="img">
                            <img src="../assets/images/User Image 01.png" alt="user">
                        </div>
                        <h1>Name</h1>
                        <p>Designation</p>
                    </div>
                </div>
            </swiper-slide>
            <swiper-slide>
                <div>
                    <div class="feedback-info">
                        <div class="t_frame">
                            <img src="../assets/images/tutuq.png" alt="img">
                        </div>
                        <p>When our designs need an expert opinion or approval, I know I can rely on your agency Thank you
                            for
                            all your help-I will be recommending you to everyone</p>
                    </div>
                    <div class="profile">
                        <div class="img">
                            <img src="../assets/images/User Image 01.png" alt="user">
                        </div>
                        <h1>Name</h1>
                        <p>Designation</p>
                    </div>
                </div>
            </swiper-slide>
            <swiper-slide>
                <div>
                    <div class="feedback-info">
                        <div class="t_frame">
                            <img src="../assets/images/tutuq.png" alt="img">
                        </div>
                        <p>When our designs need an expert opinion or approval, I know I can rely on your agency Thank you
                            for
                            all your help-I will be recommending you to everyone</p>
                    </div>
                    <div class="profile">
                        <div class="img">
                            <img src="../assets/images/User Image 01.png" alt="user">
                        </div>
                        <h1>Name</h1>
                        <p>Designation</p>
                    </div>
                </div>
            </swiper-slide>
        </swiper>

    </div>
</template>

<script>
import { Swiper, SwiperSlide } from 'swiper/vue';
import 'swiper/css'
import 'swiper/css/navigation';
import '../style.css'
import { Navigation } from 'swiper/modules'

export default {
    name: "ClientsComponent",
    components: {
        Swiper,
        SwiperSlide,
    },
     data() {
        return {
            screenWidth: window.innerWidth,
            count: 1
        };
    },
    mounted() {
        window.addEventListener("resize", this.onResize);
    },
    beforeUnmount() {
        window.removeEventListener("resize", this.onResize);
    },
    methods: {
        onResize() {
            this.screenWidth = window.innerWidth;
            if (this.screenWidth > 430) {
                this.count = 3
            }
            else {
                this.count = 1
            }
        }
    },
    setup() {
        return {
            modules: [Navigation]
        };
    },
}
</script>

<style scoped>
.client-template {
    margin-top: 64px;
}

.scnd-template {
    margin-top: 32px;

}

.feedback-box {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    height: 400px;
}

.img {
    width: 48px;
    height: 48px;
    border-radius: 50%;
    margin: auto;
}

.t_frame {
    width: 25px;
    height: 20px;
    margin: auto;
    margin-bottom: 10px;

}

.profile {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 24px;
}

.feedback-info {
    margin-top: 48px;
    padding: 48px;
    border-radius: 16px;
    width: 185px;
    background: var(--gray-100, #F3F4F6);
}
@media only screen and (max-width: 430px) {
    .feedback-info{
    padding: 20px;
    margin-top: 20px;
    }
    .client-template{
        margin-top: 20px;
    }
}
</style>