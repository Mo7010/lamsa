<template>
  <footer>
      <div class="left">
          <img src="https://media.discordapp.net/attachments/1229488327124586607/1229489909648199810/772BDE8C-F7B0-422A-8B7D-CD8162611EBF.png?ex=662fdeb5&is=661d69b5&hm=92eaeed4cc570f537d0f7c50082f96fb73f51b2e6ab7fce9f14d646114f6add2&=&format=webp&quality=lossless&width=400&height=400" alt="tetra logo">
          <h4>© 2024 Lamsa Services</h4>
          <h4>Developed By fr3o.n</h4>
      </div>
      <list>
          <nav>
          <a href="#">Home</a>
          <a href="#">About</a>
          <a href="#works">Works</a>
          <a href="#prices">Prices</a>
          <a href="https://discord.gg/l-m1">Order</a>
      </nav>
      <nav>
          <a href="https://discord.gg/l-m1">الرئيسية</a>
          <a href="#">عنا</a>
          <a href="#works">الاعمال</a>
          <a href="#prices">الاسعار</a>
          <a href="https://discord.gg/l-m1">التواصل</a>
      </nav>
      </list>
  </footer>
</template>

<style scoped>

list{
  display:flex;
  gap:60px;
}

footer {
  margin-top:200px;
          background-image:repeating-linear-gradient(90deg, rgba(0,0,0, 0.06) 0px, rgba(0,0,0, 0.06) 1px,transparent 1px, transparent 21px,rgba(0,0,0, 0.06) 21px, rgba(0,0,0, 0.06) 22px,transparent 22px, transparent 72px),repeating-linear-gradient(0deg, rgba(0,0,0, 0.06) 0px, rgba(0,0,0, 0.06) 1px,transparent 1px, transparent 21px,rgba(0,0,0, 0.06) 21px, rgba(0,0,0, 0.06) 22px,transparent 22px, transparent 72px),repeating-linear-gradient(135deg, rgba(0,0,0, 0.06) 0px, rgba(0,0,0, 0.06) 1px,transparent 1px, transparent 21px,rgba(0,0,0, 0.06) 21px, rgba(0,0,0, 0.06) 22px,transparent 22px, transparent 72px),linear-gradient(90deg, #3C6CFF,#3C6CFF);
          color: #fff;
          padding: 20px 0;
          text-align: center;
          width: 100%;
          min-height: 40vh;
          display: flex;
          flex-direction:row;
          flex-wrap:wrap;
          gap:80px;
          justify-content:space-around;
          align-items: center;
      }

      nav{
          display:flex;
          flex-direction:column;
          gap:30px;
      }

      footer a {
          color: #fff;
          text-decoration: none;
          margin: 0 10px;
      }

      footer img {
          width:400px;
          height:400px;
          margin-left:10px;
      }

  @media (max-width: 700px){
    .footer img{
      width:300px;
      height:300px;
    }
  }
</style>
