<script>
  import { RouterLink, RouterView } from 'vue-router'
</script>
<template>
  <div class="nav">
    <img src="https://media.discordapp.net/attachments/1229488327124586607/1235930332235169885/C98CBA3F-7E7E-49D8-A8F0-0826D4BFB9CF.png?ex=6646a411&is=66455291&hm=a7c75e65aa38e3748f25d78af407d263329005b95c883bf7276729e4324882a7&=&format=webp&quality=lossless&width=80&height=80">
    <div class="pages">
      <a href="/">الرئيسية</a>
      <a href="#prices">الأسعار</a>
      <a href="/#works">الأعمال</a>
      <RouterLink class="page" to="/order">اطلب الان</RouterLink>
    </div>
    <a class="btn" href="https://discord.gg/lamsa">سيرفر الديسكورد</a>
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
  color:#582592;
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
  border-bottom:1px solid #582592;
}

.nav .btn{
  text-decoration:none;
  color:#582592;
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
