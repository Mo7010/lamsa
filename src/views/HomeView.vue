<script>
import { RouterLink, RouterView } from 'vue-router'
import NavBar from '@/components/NavBar.vue'
import Footer from '@/components/Footer.vue'

export default{
  components:{
    NavBar,
    Footer
  },
  data() {
    return {
      images:[
        'https://media.discordapp.net/attachments/1229488327124586607/1235938364222607370/C41E2F59-5A48-4513-A837-B5F50878F5F4.jpg?ex=663630cc&is=6634df4c&hm=f7146878a685ae34ea5984c30cd4d926592d1a1c2bf3f22e269c3466cc0d8711&',
        'https://media.discordapp.net/attachments/1229488327124586607/1235938398649454592/5EB65398-2069-4400-B7D8-254A5F28F6F8.jpg?ex=663630d4&is=6634df54&hm=1ca312519ed72ff4ba45b4c751bac96986f9ecdc59cbbfeec56992f057b6c618&',
        'https://media.discordapp.net/attachments/1229488327124586607/1235938409617297441/3C009975-9DCB-4A27-B4DB-6DE6A20726C9.jpg?ex=663630d7&is=6634df57&hm=59eb4b59e13a043133504b73934b75d37f6dd086ac065f9da90bea225b2dfc19&'
      ]
    };
  },
}
</script>

<template>
  <main>
    <div class="home">
      <NavBar />
      <div class="text">
        <h1>لمسة لخدمات التصميم</h1>
        <h2>نقدم لك لمسة من الابداع بافضل جودة في الديسكورد نقدم لك تصاميم لكل المجالات باسعار متوفرة لدي الجميع بكل طرق الدفع</h2>
        <div class="btns">
          <a class="btn" href="https://discord.gg/l-m1">العروض</a>
          <RouterLink class="btn" to="/order">اطلب الان</RouterLink>
        </div>
      </div>
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path fill="#ffffff" fill-opacity="1" d="M0,128L48,149.3C96,171,192,213,288,224C384,235,480,213,576,186.7C672,160,768,128,864,133.3C960,139,1056,181,1152,186.7C1248,192,1344,160,1392,144L1440,128L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"></path></svg>
    </div>
    <div class="prices" id="prices">
      <h1>الأسعار <font-awesome-icon :icon="['fas', 'tag']" /></h1>
      <div class="cont">
        <div class="card">
          <h2>حزمة الاثارة</h2>
          <div class="info">
            <a>لوقو ثابت او متحرك</a>
            <a>بنر ثابت او متحرك</a>
            <a>خط ثابت</a>
            <a>انفو 8</a>
            <a>صور بوتات 4</a>
          </div>
          <div class="price">
            <h3>5 مليون كرديت</h3>
            <h3>28 ريال سعودي</h3>
          </div>
        </div>
        <div class="card">
          <h2>حزمة الابداع</h2>
          <div class="info">
            <a>لوقو ثابت او متحرك</a>
            <a>بنر ثابت او متحرك</a>
            <a>خط ثابت او متحرك</a>
            <a>بنر انفايت</a>
            <a>انفو 10</a>
            <a>صور بوتات 5</a>
            <a>ترحيب</a>
          </div>
          <div class="price">
            <h3>7 مليون كرديت</h3>
            <h3>40 ريال سعودي</h3>
          </div>
        </div>
        <div class="card">
          <h2>حزمة المستوي</h2>
          <div class="info">
            <a>لوقو ثابت</a>
            <a>بنر ثابت</a>
            <a>خط ثابت</a>
            <a>انفو 5</a>
            <a>صور بوتات 2</a>
          </div>
          <div class="price">
            <h3>3.5 مليون كرديت</h3>
            <h3>13 ريال سعودي</h3>
          </div>
        </div>
      </div>
    </div>
    <div class="feedbacks">
      <h1>الأراء <font-awesome-icon :icon="['fas', 'comment']" /></h1>
      <div class="cont">
        <div data-aos="fade-right" data-aos-duration="1500" class="cont1">
                    <div class="top">
                        <div class="left">
                            <img src="https://media.discordapp.net/attachments/1229488327124586607/1229516737150713916/70614f56c734f3af4c3e42b6abbd92ef.png?ex=662ff7b1&is=661d82b1&hm=9479522394defc3f826b0d52ce244f685707d775da1508a08e01af641e04500c&=&format=webp&quality=lossless" alt="lamsa feedbacks">
                        <p>kg.r</p>
                        </div>
                        <div class="right">
                            <p>✨✨✨✨✨</p>
                        </div>
                    </div>
                    <h3>يبوي اقسم بالله فنان و تصاميم جامده و ابو عسره القوه تصاميم توب توب</h3>
                    </div>
                    <div data-aos="fade-right" data-aos-duration="1500" class="cont1">
                    <div class="top">
                        <div class="left">
                            <img src="https://media.discordapp.net/attachments/1229488327124586607/1229516683673342049/cd21e2fd5f5200a4ef4d707fd98593b8.png?ex=662ff7a4&is=661d82a4&hm=b63548a9dbe14c34b4bfb73666f52d388a4350dc265f418baae1d942ee89e718&=&format=webp&quality=lossless" alt="lamsa feedbacks">
                        <p>naseer1319</p>
                        </div>
                        <div class="right">
                            <p>✨✨✨✨✨</p>
                        </div>
                    </div>
                    <h3>فنااااااان ماشاء الله تصاميمه مرة قوية والجودة عالية مرة انصحكم فيه بدون تفكير</h3>
                    </div>
                    <div data-aos="fade-right" data-aos-duration="1500" class="cont1">
                    <div class="top">
                        <div class="left">
                            <img src="https://media.discordapp.net/attachments/1229488327124586607/1229516787545014282/314050b87db9530181acaa68ee0d7cff.png?ex=662ff7bd&is=661d82bd&hm=6fe915fc8e9603f62ed2689fd4e7ab2201628d635898bdb09f4db9440e962592&=&format=webp&quality=lossless" alt="lamsa feedbacks">
                        <p>3we6</p>
                        </div>
                        <div class="right">
                            <p>✨✨✨✨✨</p>
                        </div>
                    </div>
                    <h3>ما عندي شي اقولوا غير انهم ملوك التصاميم</h3>
                    </div>
      </div>
    </div>
    <div class="works" id="works">
      <h1>الأعمال <font-awesome-icon :icon="['fas', 'briefcase']" /></h1>
      <div v-for="(image, index) in images" :key="index" class="cont">
          <img :src="image" alt="Slide">
        </div>
    </div>
    <Footer />
  </main>
</template>


<style scoped>
.cont img{
  border-radius:8px;
  width:40%;
}

.card{
  display:flex;
  flex-direction:column;
  justify-content:center;
  align-items:center;
  padding:20px 100px;
  background-color:whitesmoke;
  border-radius:10px;
  gap:30px;
}

  .home svg{
    margin-top:auto;
  }
.card h2{
  font-size:30px;
  color:#582592;
}

.card .info{
  width:100%;
  font-size:20px;
  display:flex;
  flex-direction:column;
  justify-content:center;
  align-items:end;
}

.cont{
  margin-top:100px;
  width:100%;
  display:flex;
  flex-direction:row;
  gap:80px;
  justify-content:center;
  flex-wrap:wrap;
}

.card .price{
  width:100%;
  direction:rtl;
  display:flex;
  flex-direction:column;
  justify-content:center;
  align-items:start;
  gap:10px;
}

.prices h1,.feedbacks h1,.works h1{
  color:#582592;
  font-size:50px;
}

main{
  width:100%;
  height:100%;
  overflow:hidden;
}

.prices{
  margin-top:100px;
  width:100%;
  display:flex;
  flex-direction:column;
  align-items:center;
}

.feedbacks{
  margin-top:100px;
  width:100%;
  display:flex;
  flex-direction:column;
  align-items:center;
}

.works{
  margin-top:100px;
  width:100%;
  display:flex;
  flex-direction:column;
  align-items:center;
}

.home{
  width:100%;
  height:100vh;
  background-image:url('https://media.discordapp.net/attachments/1229488327124586607/1235934098569039892/E940DFEB-2EE6-476E-8DCC-474AB0BE36F9.jpg?ex=66362cd3&is=6634db53&hm=abf914d0d1230f02f88c516072d0c28d2193c86ccee2ea77c3f9c0d273554777&=&format=webp');
  background-size:cover;
}

.text{
  text-align:center;
  margin-top:150px;
  width:100%;
  display:flex;
  flex-direction:column;
  justify-content:center;
  align-items:center;
  gap:8px;
}

.text h1{
  color:white;
  font-size:55px;
  text-shadow:1px 1px 3px rgba(0, 0, 0, 0.425);
}

.text h2{
  color:rgb(255, 255, 255);
  font-weight:lighter;
  width:40%;
  text-shadow:2px 2px 5px rgba(0, 0, 0, 0.377)
}

.btns{
  margin-top:10px;
  display:flex;
  justify-content:center;
  align-items:center;
  gap:20px;
}

.btn{
  text-decoration:none;
  color:#582592;
  padding:8px 30px;
  border-radius:25px;
  background-color:white;
  cursor:pointer;
  box-shadow:2px 2px 5px rgba(0, 0, 0, 0.377)
}

.cont1{
    border-radius:8px;
    background-color:whitesmoke;
    width:400px;
    padding:5px 10px;
    height:250px;
    display:flex;
    flex-direction:column;
    border-top:4px solid #3C6CFF;
    border-bottom:4px solid #3C6CFF;
}

.top{
    margin-top:15px;
    display:flex;
    justify-content:space-around;
    align-items:center;
}

.left{
    display:flex;
    justify-content:space-around;
    align-items:center;
}

.top img{
    width:40px;
    margin-right:10px;
}

.cont1 h3{
    text-align:end;
    margin-top:60px;
    padding:5px 5px;
}

@media screen and (max-width: 768px) {
  .home svg{
    display:none;
  }

  .home{
    min-height:100vh;
  }

  .home .text h2{
    width:90%;
  }

  .prices{
    margin-top:200px;
  }

  .works img{
    width:80%;
  }
  .cont1{
    width:90%;
  }

  .prices .card{
    width:90%;
  }
  
  .cont1 p{
    font-size:20px;
  }

  .prices .card{
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
    text-align:center;
  }
  
  .prices .card h2,.prices .card .info,.prices .card .price{
    width:300px;
  }
  .home{
    min-height:120vh;
  }
}
</style>
