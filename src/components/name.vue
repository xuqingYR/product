<template>
    <div class="name">
        <img src="../assets/cat.jpg" alt="">
        <div class="personal">
            <h2>{{ name }}</h2>
            <p>{{ address }}</p>
        </div>
    </div>
</template>

<script>
export default {
    name:"name",
    data(){
        return{
            name:"无敌的空格",
            address: "上海"
        }
    }
}
</script>

<style scoped lang='less'>
.name {
    height: 180/100rem;
    width: 750/100rem;
    background: #ffffff;
    display: flex;
}
.name img {
    width:120 / 100rem;
    height: 120 / 100rem;
    border-radius: 60 / 100rem;
    border: 2/100rem solid #FFFFFF;
    margin: 30/100rem 0 0  30/100rem;
}
.personal h2 {
    display: block;
    width: 181 / 100rem;
    height: 50 / 100rem;
    font-size: 36 / 100rem;
    font-family: PingFangSC-Regular;
    color: #333333;
    letter-spacing: 0;
    padding: 36/100rem 0 0 30/100rem;
}
.personal p {
    font-family: PingFangSC-Regular;
    font-size: 24 / 100rem;
    color: #9B9B9B;
    line-height: 32 / 100rem;
    width: 48 / 100rem;
    height: 32 / 100rem;
    padding: 24/100rem 0 0 30/100rem;
}
</style>
