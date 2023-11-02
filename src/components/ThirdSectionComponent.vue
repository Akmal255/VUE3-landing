<template>
    <div class="rd-section">
        <div class="fst-template">
            <h1>Готовы присоединиться и развиваться вместе с нами?
            </h1>
            <p class="p">Заполните форму, и мы свяжемся с вами!</p>
            <form class="form">
                <label for="">
                    <p>Имя</p>
                <input type="text">
                </label>
                <label for="">
                    <p>Фамилия</p>
                <input type="text">
                </label>
                <label for="">
                    <p>Номер телефона</p>
                <input type="text" placeholder="+998" value="+9989">
                </label>
                <label for="">
                    <p>Город</p>
                <select name="" id="">
                    <option value=""></option>
                    <option value=""></option>
                </select>
                </label>
                <label for="">
                    <p>Направление</p>
                    <select name="" id="">
                    <option value=""></option>
                    <option value=""></option>
                </select>
                </label>
                <label for="">
                    <p>Район</p>
                    <select name="" id="">
                    <option value=""></option>
                    <option value=""></option>
                </select>
                </label>
                <button class=""></button>
            </form>
            <div style="display: flex; justify-content: center;">
            <button class="btn-registration">Отправить</button>
        </div>
        </div>
        <div class="scnd-template">
            <img src="../assets/images/image10.png" alt="10">
        </div>
    </div>
</template>

<script>
export default {
    name: "ThirdSectionComponent"
}
</script>

<style  scoped>
label{
    width: 350px;
}
input{
    width: 100%;
    padding: 0;
}
.rd-section {
    text-align: left;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 20px;
}
.fst-template{
    margin: auto;
    max-width: 624px;
    margin-top: 32px;
    margin-bottom: 24px;
}
.scnd-template{
    width: 100%;
    max-width: 472px;
}
.scnd-template img{
    width: 100%;
}
.p{
   margin-top: 32px;
   margin-bottom: 24px;
    
}
.form{
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 28px;
}
input , select {
    border: 1px solid #D1D5DB;
    border-radius: 8px;
    height: 40px;
    width: 100%;
        
    margin-top: 8px;
}
.btn-registration{
        border-radius: 16px;
        background: #FF6600;
        max-width:  345px;
        width: 100%;
        height: 48px;
        color: white;
        margin-top: 28px;
        
    }

@media only screen and (max-width: 430px) {
    .form{
        display: block;
    }
    .scnd-template{
        display: none;
    }
}
</style>