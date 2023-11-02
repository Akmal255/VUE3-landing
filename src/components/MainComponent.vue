<template>
    <div class="main">
        <div class="img-template">
            <div class="fst-template">
                <div class="fst-image img"><img src="../assets/images/Image 04.png" alt="img1"></div>
                <div class="scnd-image img"><img src="../assets/images/Image 03.png" alt="img1"></div>
            </div>
            <div class="scnd-template">
                <div class="rd-image img"><img src="../assets/images/image 02.png" alt="img1"></div>
                <div class="frth-image img"><img src="../assets/images/Image 01.png" alt="img1"></div>
            </div>
        </div>
        <div class="main-content">
            <div>
            <h1>Раскрой свой потенциал вместе с Coozin!</h1>
            <p>Универсальная платформа Coozin предоставляют множество возможностей для самозанятых женщин. На платформе
                можно продавать товары и услуги, а также учиться новым навыкам и развивать свой бизнес</p>
            <button class="btn-registration">Присоединиться</button>
        </div>
            <div class="results">
                <p>Достижения</p>
                <div class="results-info">
                    <div class="block">
                        <h1>1K</h1>
                        <p>женщин прошли обучение</p>
                    </div>
                    <div class="block">
                        <h1>130K</h1>
                        <p>присоединились
                            в платформу</p>
                    </div>
                    <div class="block">
                        <h1>1K</h1>
                        <p>пользователей платформы</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "MainComponent"
}
</script>

<style  scoped>
.main {
    display: flex;
    justify-content: space-between;
    flex-direction: row-reverse;
    margin-top: 60px;
    gap: 10px;
}

.img-template {
    max-width: 624px;
    width: 100%;

}

.main-content {
    margin-top: 20px;
    text-align: left;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
}

.main-content p {
    margin: 12px 0 24px 0;
}
.results-info{
    display: flex;
    gap: 16px;
}
.results-info p{

font-size: 16px;
line-height: 16px;
letter-spacing: 0px;
text-align: left;
}
.results-info h1{
font-size: 36px;
font-weight: bolder;
line-height: 40px;
letter-spacing: 0px;
text-align: left;
}

.block{
    width: 164px;
}
.btn-registration {
    border-radius: 16px;
    background: #FF6600;
    max-width: 165px;
    padding: 16px;
    height: 48px;
    color: white;
}

.fst-template {
    display: grid;
    grid-template-columns: 2fr 1fr;
    gap: 12px;
    width: 100%;
}

.scnd-template {
    display: grid;
    grid-template-columns: 1fr 2fr;
    gap: 12px;
    margin-top: 12px;
}

.fst-image img {
    width: 100%;
    height: 316px;
}

.scnd-image img {
    width: 100%;
    height: 316px;
}

.rd-image img {
    width: 100%;
    height: 328px;
}

.frth-image img {
    width: 100%;
    height: 328px;
}

.img {
    border-radius: 16px;
}

@media only screen and (max-width: 430px) {

    .main {
        flex-direction: column;
        margin-top: 20px;
    }

    .btn-registration {
        border-radius: 16px;
        background: #FF6600;
        width: 100%;
        height: 48px;
        max-width: 100%;
        color: white;
    }

    .fst-image img {
        height: 178px;
    }

    .scnd-image img {
        height: 178px;
    }

    .rd-image img {
        height: 185px;
    }

    .frth-image img {
        height: 185px;
    }
}
</style>