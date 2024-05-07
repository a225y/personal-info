<template>
    <div class="section flex">
        <div class="info w-1/2">
            <div class="info-main">
                <div class="name">
                <div> 
                    <h1>蘇 瀚儒</h1>
                    <h4>ソ カンジュウ</h4>
                </div>
            </div> 
             <!-- 1 -->
             <div class="about">
                <div class="about-box">
                    <h1 class="mb-5">転職きっかけ</h1>
                    <p>・前職は清水建設の現場調達として勤務しております。
                    台湾に第3棟、陽子線を利用してがん細胞を狙い撃ち
                    というがん治療センターの病院を建てました。</p>
                    <p>・IT、Web開発に興味を持っている私は、現場事務所解散した後。
                    去年の10月に再春館入社します</p>
                </div>    
            </div>
            <!-- 2 -->
            <div class="about ">
                <div class="about-box">
                    <h1 class="mb-5">趣味・好きな事</h1>
                    <p>・パンと料理を作る。</p>
                    <p>・コーディングとWebサイトを作る</p>
                    <p>・旅行</p>
                    <p>・フイルム写真を撮る</p>
                    <p>・株を投資すること</p>
                </div>    
            </div>
            </div>
            
        </div>

        <div class="img w-1/2">
           <img src="../assets/vue.svg" alt="" srcset="">	
           <div class="img-swiper">
                <Swiper/>
                <Hoby/>
           </div>
		</div>
       
    </div>
</template>

<script >
import Swiper from '../components/Swiper.vue'
import Hoby from '../components/Hoby.vue';
export default {
    components:{ Swiper,Hoby }
}

</script>


<style scoped>
.section {
    width: 100%;
    height: 100vh;
    background-color: #000;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
}
.section p{
    font-weight: 200;
    padding: 3px;
}
.info{
    /* background-image: url(../assets/bg.png); */
    background-color: #FFF;
   
}
.info-main{
    width: 100%;
    height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
}
.name{
    display: flex;
    justify-content: center;
    margin-top: 50px;
}
.name h1{
    font-size: 4.5rem;
}
.name h4{
    font-size: 2rem;
}
.about{
    margin: 50px 0;
    width: 400px;
}
.about h1{
    font-size: 1.3rem;
    position: relative;
    display: inline-block;
}
.about h1::after{
    content: '';
    width: 200px;
    border-bottom: 1px solid #000;
    position: absolute;
    top: 50%;
    left: 180px;
}

</style>
