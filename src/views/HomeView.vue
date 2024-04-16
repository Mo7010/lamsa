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
        'https://media.discordapp.net/attachments/1224031249379758110/1229524710073831454/IMG_6797.png?ex=662fff1e&is=661d8a1e&hm=93e6a42c94f09724f272f076035049ec2e1b3e9f3e234d571e74eba6ab6dff2e&',
        'https://media.discordapp.net/attachments/1224031249379758110/1229524710824480818/5D89DFB8-F2B2-49CF-96D9-FB2DEC54081A.jpg?ex=662fff1e&is=661d8a1e&hm=0aaf243a21f03176398285c51c51b8e93a8aba8ea2a91d7c353bc76123d3c416&',
        'https://media.discordapp.net/attachments/1224031249379758110/1229524711428460675/E7B06402-C4E6-4F65-81C4-0961B7DB51D2.jpg?ex=662fff1e&is=661d8a1e&hm=fa47a8dd7fd1ba19f177bdc32d3f9ea710e8c473f7e0e3ebc7703532194c4da4&',
        'https://media.discordapp.net/attachments/1224031249379758110/1229524711428460675/E7B06402-C4E6-4F65-81C4-0961B7DB51D2.jpg?ex=662fff1e&is=661d8a1e&hm=fa47a8dd7fd1ba19f177bdc32d3f9ea710e8c473f7e0e3ebc7703532194c4da4&',
        'https://media.discordapp.net/attachments/1224031249379758110/1229524711705415721/B1F9A97E-B462-49F4-898E-F9AF1089CC21.jpg?ex=662fff1e&is=661d8a1e&hm=aac50ec0bed3ad913c29d0d711ab1c34425b883b18dcb02cc4e597edd0ba5ef8&',
        'https://media.discordapp.net/attachments/1229513281408860282/1229524670001319966/lamstamer1.png?ex=662fff14&is=661d8a14&hm=b5dc7adf70bd8bce0a19f98d3b08a80d360d62b65fd713ca92500217f27091c4&',
        'https://media.discordapp.net/attachments/1229513281408860282/1229524669715972117/lamsatamer3.png?ex=662fff14&is=661d8a14&hm=0519cc86ed667ef92cb61cc4a5f320f1f66fdc781295654e5bf987a2ebc153e1&',
        'https://media.discordapp.net/attachments/1229513281408860282/1229525040387719168/lamsatamer22.png?ex=662fff6d&is=661d8a6d&hm=6e45c75ad52e8542085d28efac317abd97b8a0175328c0390c9791883432e8b9&'
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
                    <h3>يبوي اقسم بالله فنان و تصاميم جامده و ابو عسره القوه تصاميم توب و سرعه في التعامل و الرد الصاروخي ياخي وش اقول وش اخلي توب توب</h3>
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
    margin-top:100px;
  }
.card h2{
  font-size:30px;
  color:#3C6CFF;
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
  color:#3C6CFF;
  font-size:50px;
}

main{
  width:100%;
  height:100%;
}

.prices{
  margin-top:-100px;
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
  background-image:url('https://media.discordapp.net/attachments/1229488327124586607/1229504834584186991/5F5A4ED9-ACBB-4CF6-8D03-071499885703.jpg?ex=662fec9b&is=661d779b&hm=432adadb64e8f9a61a4510a4327074cc22e02aa9a460e274a8cd213da0b7cae8&=&format=webp');
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
  color:#3C6CFF;
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
}
</style>
