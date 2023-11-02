<template>
    <div class="scnd-section">
        <div class="fst-template">
            <h1>Почему Coozin?</h1>
        </div>
        <div class="scnd-template">
            <div class="scnd-template-info">
                <div class="img"><img src="../assets/images/1.png" alt="1"></div>
                <h3>Универсальная платформа</h3>
                <p>Предназначенная для самозанятых женщин превратить свое хобби в прибыльный бизнес</p>
            </div>
            <div class="scnd-template-info">
                <div class="img"><img src="../assets/images/2.png" alt="2"></div>
                <h3>Обучение и бизнес</h3>
                <p>Женщины экономят время и ресурсы, которые могут быть направлены на развитие своего бизнеса</p>
            </div>
            <div class="scnd-template-info">
                <div class="img"><img src="../assets/images/3.png" alt="3"></div>
                <h3>Дополнительный заработок</h3>
                <p> Домохозяйки могут стать партнерами нашего проекта и получить инструменты для управления своим бизнесом.</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "SecondSectionComponent"
}
</script>

<style  scoped>
.scnd-section {
    margin-top: 24px;
    text-align: center;
    padding: 100px 0;
}

.scnd-template {
    margin-top: 24px;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;

}
.scnd-template-info{
    display: flex;
    flex-direction: column;
    align-items: center;

}
.scnd-template-info p{
    max-width: 350px;
}
.img{
    width: 140px;
    height: 140px;
    margin: auto;
    margin-bottom: 16px;
}
.scnd-template p {
    margin: 12px 0 24px 0;
}

@media only screen and (max-width: 430px) {
    .scnd-template {
        display: flex;
        flex-direction: column;
}
.scnd-section{
    padding: 0;
}
}




</style>