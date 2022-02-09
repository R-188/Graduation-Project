<template>
    <div class="container mx-auto">
        <a class="section1" v-for="item in shopPic" :key="item" href="">
            <img :src="item.img" alt />
            <div class="item price">           
                <span>￥200.00</span>
            </div>
            <div class="item itemName">
                <span><a href="">2022最新款包邮(限购5卷)78抽超大卷洁面巾F191145</a></span>
            </div>
        </a>

    </div>
</template>



<script>
import logo from "../../assets/logo.png"
import vp from "../../assets/1484728977lV1.png"
import emo from "../../assets/emo.jpg"
export default {
    name: 'Shop',
    data() {
        return{
            shopPic:[
                {id:0, img: logo},
                {id:1, img: vp},
                {id:2, img: emo}
            ]
        };
    }
}
</script>


<style scoped>
.container {
    display: flex;
    flex-wrap: wrap;
    margin-top: 25px;

}
.section1 {
    width: 350px;
    height: 495px;
    display: flex;
    margin: 35px;
    flex-direction: column;
    border-radius: 1rem;
}
.section1:hover {
    background:#fff;
    box-shadow:0 19px 39px 0 rgba(0,0,0,.2);
}

img {   
    width: 350px;
    height: 350px;
    border-radius: 12px;
    overflow: hidden;
}
.item {
    box-sizing: border-box;
    display: flex;
    align-content: flex-start;
    position: relative;
}
.price {
    display: flex;
    width: 350px;
    justify-content: flex-end;
    margin-block: 20px;
    font-size: 1.5rem;
    line-height: 2rem;
    font-weight: 900;
}
.itemName {
    display: flex;
    width: 350px;
    flex-wrap: wrap;
}
.itemName:hover {
    color: rgb(236, 94, 12);
    text-decoration-style: solid;
    text-shadow: 3px 3px 6px rgb(0 0 0 / 26%), 0 0 5px rgb(15 3 86 / 22%);
}
</style>