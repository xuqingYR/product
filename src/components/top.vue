<template>
<div class="all">
        <div class='top'>
        <div class="top-first">
            <div class="top-first-left">
                <div class="circular1"></div>
                <div class="circular2"></div>
                <div class="circular2"></div>
                <div class="circular2"></div>
                <div class="circular2"></div>
                <div class="Brianna">
                    <p>{{msg}}</p>
                </div>
                <div class="signal">
                <div class="curveOne med"></div>
                <div class="curveTwo med"></div>
                <div class="curveThree"></div>
                </div>
            </div>
            <div class="top-first-middle">
                <p>{{ time }}</p>
            </div>
            <div class="top-first-right">
                <p>{{ electric }}</p>
                <img src="../assets/electric.png">
            </div>
        </div>
        <div class="top-second">
            <div class="icon">
                <div class="row"></div>
                <div class="clou"></div>
            </div>
            <p class="personal">{{ message }}</p>
            <div class="icon1">
                <div class="icon2"></div>
                <div class="icon3"></div>
                <div class="icon2"></div>
            </div>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name:"list",
    data(){
        return{
            msg: "Brianna",
            time: "9:50AM",
            electric: "100%",
            message: "个人信息",
            close: "X"
        }
    }
}
</script>

<style scoped lang="less">
.all {
    width: 750 / 100rem;
}
.top {
    height:128 / 100rem;
}
.top-first-left {
    float: left;
    height: 33 / 100rem;
}
.top-first {
    height: 33 / 100rem;
    width: 750 / 100rem;
}
.circular1 {
    width: 11 / 100rem;
    height: 11 /100rem;
    border-radius: 50%;
    background: #333333;
    margin: 15 / 100rem 0 0 13 / 100rem;
    float: left;
}
.circular2 {
    width: 11 / 100rem;
    height: 11 / 100rem;
    border-radius: 50%;
    background: #333333;
    margin: 15 / 100rem 0 0 4 / 100rem;
    float: left;
}
.Brianna{
    font-size: 24 / 100rem;
    line-height: 33 / 100rem;
    height: 33 / 100rem;
    width: 85 / 100rem;
    float: left;
    margin: 3 / 100rem 0 0 6 / 100rem;
    font-family: PingFangSC-Regular;
    color: #333333;
    letter-spacing: 0;
    text-align: left;
}
.signal{
  //background-color:green;
  width:13 / 100rem;
  height:13 / 100rem;
  //margin-top:50px;
  position:relative;
  top: 7 / 100rem;
  left: 20 / 100rem;
  overflow:hidden;
  //transform-origin:50% 50%;
  -webkit-transform:rotate(45deg) scale(2);
          transform:rotate(45deg) scale(2);
}

.curveOne{
  border-radius:50%;
  border:1.3 / 100rem solid #333333;;
  position:absolute;
  right:0%;
  bottom:0;
  -webkit-transform:translate(50%,50%);
          transform:translate(50%,50%);
  width:150%;
  height:150%;
}

.curveTwo{
  border-radius:50%;
  border:1.3 / 100rem solid #333333;;
  position:absolute;
  right:0%;
  bottom: 0.1/100rem;
  width:100%;
  -webkit-transform:translate(50%,50%);
          transform:translate(50%,50%);
  height:100%;
}

.curveThree{
  border-radius:50%;
  border:1.3 / 100rem solid #333333;;
  position:absolute;
  bottom:0;
  background-color:#333333;
  height:50%;
  right:0%;
  width:50%;
  -webkit-transform:translate(50%,50%);
          transform:translate(50%,50%)
}
.top-first-middle{
    width: 93 / 100rem;
    height: 28 / 100rem;
    position: absolute;
    left: 50%;
    margin-left: -(93 / 100rem)/2;
    margin-top: 7 / 100rem;
}
.top-first-middle p{
    font-family: SFNSText;
font-size: 24 / 100rem;
color: #333333;
letter-spacing: 0;
text-align: center;
}
.top-first-right {
    float: right;
    height: 28px;
    position: absolute;
    right: 0;
    display: flex;
    justify-content:space-between;
}
.top-first-right p {
    display: block;
    font-size: 24 / 100rem;
    font-family: SFNSText;
    color: #333333;
    letter-spacing: 0;
    text-align: center;
    display: block;
    width: 66 /100rem;
    height: 28 / 100rem;
    margin-top: 7 / 100rem;
}
.top-first-right img{
    width: 41 / 100rem;
    margin-left: 8 / 100rem;
    height: 19 / 100rem;
    margin-top:13/100rem;
}
.top-second {
    height: 95 / 100rem;
    width: 750 / 100rem;
    position: relative;
}
.icon {
    width: 31.1 / 100rem;
    height: 31.1 / 100rem;
    margin-left: 30/100rem;
    position: absolute;
    top:10/100rem;
}
.row {
	height: 43/100rem;
    width: 5/100rem;
    position: relative;
    left: 60%;
    top: 70%;
    background: #333333;
    transform: rotate(45deg);
			}
.clou{
	height: 5/100rem;
	position : absolute;/*绝对定位*/
    width: 43/100rem;
    background: #333333;
    transform: rotate(45deg);

}
.personal {
    width:144/100rem;
    height: 50 / 100rem;
    position: absolute;
    left: 50%;
    top: 23/100rem;
    margin-left: -(144/100rem)/2;
    text-align: center;
    font-family: PingFangSC-Semibold;
    font-size: 36/100rem;
    color: #333333;

}
.icon1{
    display: flex;
    position: absolute;
    top: 41/100rem;
    right: 38 / 100rem;
}
.icon2{
    width: 8/100rem;
    height: 8/100rem;
    border-radius: 100%;
    background: #333333;
    margin-left:6/100rem;
}
.icon3{
    width: 12/100rem;
    height: 12/100rem;
    border-radius: 100%;
    background: #333333;
    margin-left:6/100rem;
    margin-top: -7%
}
</style>
