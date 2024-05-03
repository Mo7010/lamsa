<script>
  import { RouterLink, RouterView } from 'vue-router'
</script>
<template>
  <div class="nav">
    <img src="https://media.discordapp.net/attachments/1229488327124586607/1229489909648199810/772BDE8C-F7B0-422A-8B7D-CD8162611EBF.png?ex=662fdeb5&is=661d69b5&hm=92eaeed4cc570f537d0f7c50082f96fb73f51b2e6ab7fce9f14d646114f6add2&=&format=webp&quality=lossless&width=80&height=80">
    <div class="pages">
      <a href="/">الرئيسية</a>
      <a href="#prices">الأسعار</a>
      <a href="/#works">الأعمال</a>
      <RouterLink class="page" to="/order">اطلب الان</RouterLink>
    </div>
    <a class="btn" href="https://discord.gg/l-m1">سيرفر الديسكورد</a>
  </div>
</template>

<style scoped>
.nav{
  width:100%;
  height:15vh;
  display:flex;
  flex-direction:row-reverse;
  justify-content:center;
  align-items:center;
  gap:20%;
}

.nav .pages{
  display:flex;
  flex-direction:row-reverse;
  justify-content:center;
  align-items:center;
  gap:30px;
}

.nav .pages a,.page{
  text-decoration:none;
  color:#3B0C52;
  cursor:pointer;
}

/*
.nav .pages a{
  text-decoration:none;
  color:#3C6CFF;
  padding:5px 15px;
  border-top-left-radius:25px;
  border-bottom-right-radius:25px;
  background-color:white;
  cursor:pointer;
  transition:1s;
}*/

.nav .pages a:hover{
  border-bottom:1px solid white;
}

.nav .btn{
  text-decoration:none;
  color:#3C6CFF;
  padding:5px 15px;
  border-radius:8px;
  background-color:white;
  cursor:pointer;
}

@media screen and (max-width: 768px) {
  .nav .pages{
    display:none;
  }
}
</style>
