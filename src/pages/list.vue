<template>
<div class="all">
        <div class="list">
        <ul class="box">
            <li v-for="(name,index) in messageList" :class="[listyle]">
                <p :class="[leftstyle]">{{name.left}}</p>
                <span :class="[rightstyle]">{{name.right}}</span>
                <div :class="[name.sign]"></div>
            </li>
        </ul>
    </div>
    <div class="last">
        <div class="last1">
                <p :class="[leftstyle]">{{name}}</p>
                <span :class="[rightstyle]">{{right}}</span>
                <div :class="[sign]"></div>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name:"list",
    data(){
        return {
            messageList:[
                {
                    left:"手机号",
                    right:"未填写",
                    sign:"sign1",
                },{
                    left:"性别",
                    right:"未填写",
                    sign: "sign1"
                },{
                    left:"生日",
                    right:"设置后不可修改",
                    sign:"sign1",
                }
            ],
            leftstyle:"leftstyle1",
            rightstyle:"rightstyle1",
            listyle:"listyle1",
            sign:"sign1",
            name:"地址",
            right:"修改/未添加"
        }
    }
}
</script>

<style scoped lang='less'>
.all {
    width: 750 / 100rem;
    height: 430 / 100rem;
}
.list {
    width: 750 / 100rem;
    height: 300 / 100rem;
    background: #FFFFFF;
    box-shadow: inset 0 -1/100rem 0 0 #E5E5E5;
    margin-top: 20 / 100rem;
    position: relative;
}
.box {
    width: 690 / 100rem;
    position: absolute;
    left: 50%;
    margin-left: -(690 / 100rem)/2;
    height:300 / 100rem;
}
.listyle1 {
    width: 690 / 100rem;
    height: 100 / 100rem;
    box-shadow: inset 0 -1px 0 0 #E5E5E5;
    display: flex;
    align-items: center
}
.leftstyle1{
    display: block;
    font-family: PingFangSC-Light;
    font-size: 32/100rem;
    color: #333333;
    line-height: 44/100rem;
    width: 182/100rem;
    height: 36/100rem;
}
.rightstyle1{
    font-family: PingFangSC-Light;
    font-size: 26/100rem;
    color: #999999;
    text-align: right;
    line-height: 36 / 100rem;
    display: block;
    width: 182/100rem;
    height: 36/100rem;
    position: absolute;
    right: 20 /100rem;
}
.sign1 {
    width: 20/100rem;
    height: 20/100rem;
    transform: rotate(45deg);
    border-right: 1/100rem solid #999999;
    border-top:  1/100rem solid #999999;
    position: absolute;
    right: 0;
}
// .listyle2 {
//     border-top: 30/100rem solid red
// }
.last {
    width: 750 / 100rem;
    height: 100 / 100rem;
    display: flex;
    align-items: center;
    margin-top: 30 / 100rem;
    background: #FFFFFF
}
.last1 {
    width: 690 / 100rem;
    height: 100 / 100rem;
    box-shadow: inset 0 -1px 0 0 #E5E5E5;
    display: flex;
    align-items: center;
    position: absolute;
    left: 50%;
    box-shadow: inset 0 -1px 0 0 #E5E5E5;
    margin-left: -(690/100rem)/2
}
</style>
