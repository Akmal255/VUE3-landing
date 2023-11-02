<template>
    <div class="fst-section">   
        <div class="fst-template">
            <div class="img-fst-section">
                <img src="../assets/images/image 02.png" class="imgg"  alt="img5">
            </div>
        </div>
        <div class="scnd-template">
            <div class="scnd-template-title">
                <div class="galochka"><img src="../assets/images/right8 1.png" alt="rigth"></div>
                <h1>EDU COOZIN</h1>
            </div>
            <p>Онлайн-академия Coozin предоставляет обучение и помощь в развитии бизнеса. </p>
            <div class="scnd-template-title">
                <div class="galochka"><img src="../assets/images/right8 1.png" alt="rigth"></div>

                <h1>Курсы и мастер-классы</h1>
            </div>
            <p>На платформе доступны онлайн-курсы и мастер-классы по различным темам, связанным с бизнесом, такими как
                управление продажами, маркетинг, финансы и другие.</p>
            <div class="scnd-template-title">
                <div class="galochka"><img src="../assets/images/right8 1.png" alt="rigth"></div>

                <h1>Опытные специалисты</h1>
            </div>
            <p>Курсы ведут опытные специалисты, которые делятся своими знаниями и опытом.</p>
            <div class="scnd-template-title">
                <div class="galochka"><img src="../assets/images/right8 1.png" alt="rigth"></div>

                <h1>Обучись и начни свое дело</h1>
            </div>
            <p>Пользователи которые успешно прошли курсы имеют возможность
                присоединиться к торговой площадке Coozin.</p>
        </div>
    </div>
</template>

<script>
export default {
    name: "FirstSectionComponent"
}
</script>

<style  scoped>
.fst-section {
    margin-top: 24px;
    text-align: left;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 10px;
}

.scnd-template {
    margin-top: 24px;
    max-width: 570px;
}

.scnd-template p {
    margin: 12px 0 24px 0;
}

.img-fst-section {
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 16px;
}
.img-fst-section img{
    width: 100%;
}

.scnd-template-title {
    display: flex;
    align-items: center;
}

.galochka {
    width: 32px;
    height: 32px;
    margin-right: 12px;
}
@media only screen and (max-width: 430px) {
    .fst-section{
        flex-direction: column;
    }
    .imgg{
        height: 283px;
    }
}
</style>