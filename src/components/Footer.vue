<template>
  <footer>
      <div class="left">
          <img src="https://media.discordapp.net/attachments/1229488327124586607/1235930332235169885/C98CBA3F-7E7E-49D8-A8F0-0826D4BFB9CF.png?ex=66362951&is=6634d7d1&hm=77d717e6aa41eb54e9c6ee01132bd5b28b8c61350dc2398f4818927e8a3678fe&=&format=webp&quality=lossless&width=676&height=676" alt="tetra logo">
          <h4>© 2024 Lamsa Services</h4>
      </div>
      <list>
          <nav>
          <a href="/">Home</a>
          <a href="/">About</a>
          <a href="#works">Works</a>
          <a href="#prices">Prices</a>
          <a href="https://discord.gg/lamsa">Contact</a>
      </nav>
      <nav>
          <a href="/order">الطلب</a>
          <a href="/">عنا</a>
          <a href="#works">الاعمال</a>
          <a href="#prices">الاسعار</a>
          <a href="https://discord.gg/lamsa">التواصل</a>
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
          background-image:repeating-linear-gradient(90deg, rgba(0,0,0, 0.06) 0px, rgba(0,0,0, 0.06) 1px,transparent 1px, transparent 21px,rgba(0,0,0, 0.06) 21px, rgba(0,0,0, 0.06) 22px,transparent 22px, transparent 72px),repeating-linear-gradient(0deg, rgba(0,0,0, 0.06) 0px, rgba(0,0,0, 0.06) 1px,transparent 1px, transparent 21px,rgba(0,0,0, 0.06) 21px, rgba(0,0,0, 0.06) 22px,transparent 22px, transparent 72px),repeating-linear-gradient(135deg, rgba(0,0,0, 0.06) 0px, rgba(0,0,0, 0.06) 1px,transparent 1px, transparent 21px,rgba(0,0,0, 0.06) 21px, rgba(0,0,0, 0.06) 22px,transparent 22px, transparent 72px),linear-gradient(90deg, #EFA528 ,#EFA528 );
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
</style>
