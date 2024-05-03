<script>
import NavBar from '@/components/NavBar.vue'
import { RouterLink } from 'vue-router'

export default{
    name:'Home',
    data(){
        return{

        }
    },
    components:{
        NavBar,
    },
    methods:{
        sendApply(){
            const webhookUrl = 'https://discord.com/api/webhooks/1229743795868930099/1rV2n6IxG_JNFBWB0vcl4a1WB-plW3gd8O1Aa7ehdSMNohVk2m0hQbAGWkPDplRA-Xq3'
            const user = document.getElementById("userinput").value
            const country = document.getElementById("countryinput").value
            const birthday = document.getElementById("birthinput").value
            const work = document.getElementById("workinput").value
            const languages = document.getElementById("langinput").value
            const price = document.getElementById("priceinput").value
            
            const applyMessage = {
                content: '**طلب جديد:**',
                embeds: [{
                    title: 'تفاصيل الطلب',
                    color: 0x4E40CC,
                    fields: [
                        { name: 'الايدي', value: user },
                        { name: 'الحزمة', value: birthday },
                        { name: 'تفاصيل الطلب', value: country },
                        { name: 'لون التصميم', value: work },
                        { name: 'فكرة التصميم', value: languages },
                        { name: 'طريقة الدفع', value: price },
                    ]
                }]
            };


            if(user === '' || country === '' || birthday === '' || work === '' || languages === ''){
                alert("Please Complete The Apply Form")
            } else{


                fetch(webhookUrl, {
                method: 'POST',
                headers: {
                    'Content-Type': 'application/json'
                },
                body: JSON.stringify(applyMessage)
            }).then(response => {
                if (!response.ok) {
                    throw new Error('Error, Please Try Again');
                }
                alert('تم الارسال سيتم التواصل معك في الخاص');
                document.getElementById("userinput").value = '';
                document.getElementById("countryinput").value = '';
                document.getElementById("birthinput").value = '';
                document.getElementById("workinput").value = '';
                document.getElementById("langinput").value = '';
                document.getElementById("priceinput").value = '';
            }).catch(error => {
                console.error('حدث خطأ:', error);
                alert('Error, Please Try Again');
                document.getElementById("userinput").value = '';
                document.getElementById("countryinput").value = '';
                document.getElementById("birthinput").value = '';
                document.getElementById("workinput").value = '';
                document.getElementById("langinput").value = '';
                document.getElementById("priceinput").value = '';
            });
            }
        }
    }
}

</script>

<template>
    <div class="main">
        <div class="apply">
            <div class="cont">
                <RouterLink to="/">
                    <img src="https://media.discordapp.net/attachments/1229488327124586607/1235930332235169885/C98CBA3F-7E7E-49D8-A8F0-0826D4BFB9CF.png?ex=66362951&is=6634d7d1&hm=77d717e6aa41eb54e9c6ee01132bd5b28b8c61350dc2398f4818927e8a3678fe&=&format=webp&quality=lossless&width=200&height=200" alt="Lamsa Logo">
                </RouterLink>
                <div class="inp">
                    <label>ايدي الديسكورد حقك</label>
                    <input id="userinput" placeholder="Id" type="number">
                </div>
                <div class="inp">
                    <label>اسم الحزمة او تصميم فردي</label>
                    <input id="countryinput" placeholder="Package" type="text">
                </div>
                <div class="inp">
                    <label>تفاصيل الطلب</label>
                    <input id="birthinput" placeholder="Order Info" type="text">
                </div>
                <div class="inp">
                    <label>لون التصميم</label>
                    <input id="workinput" placeholder="Ex: Color Code #FFFF type="text">
                </div>
                <div class="inp">
                    <label>فكرة التصميم</label>
                    <input id="langinput" placeholder="Design Idea" type="text">
                </div>
                <div class="inp">
                    <label>طريقة الدفع</label>
                    <input id="priceinput" placeholder="Ex: Paypal" type="text">
                </div>
                <div class="inp">
                    <label>انتهينا</label>
                    <a class="btn" @click="sendApply">Submit</a>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>

.main{
    min-height:100vh;
}
.apply{
    width:100%;
    display:flex;
    justify-content:center;
    align-items:center;
}

.cont{
    width:100%;
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
    gap:80px;
    padding:60px 20px;
    border-radius:6px;
    background-image: repeating-linear-gradient(90deg, rgba(0,0,0, 0.06) 0px, rgba(0,0,0, 0.06) 1px,transparent 1px, transparent 21px,rgba(0,0,0, 0.06) 21px, rgba(0,0,0, 0.06) 22px,transparent 22px, transparent 72px),repeating-linear-gradient(0deg, rgba(0,0,0, 0.06) 0px, rgba(0,0,0, 0.06) 1px,transparent 1px, transparent 21px,rgba(0,0,0, 0.06) 21px, rgba(0,0,0, 0.06) 22px,transparent 22px, transparent 72px),repeating-linear-gradient(135deg, rgba(0,0,0, 0.06) 0px, rgba(0,0,0, 0.06) 1px,transparent 1px, transparent 21px,rgba(0,0,0, 0.06) 21px, rgba(0,0,0, 0.06) 22px,transparent 22px, transparent 72px),linear-gradient(90deg, #EFA528,#EFA528 );
    border-left:4px solid rgb(228, 228, 228);
}

.inp{
    display:flex;
    flex-direction:column;
    gap:20px;
}

.inp label{
    text-transform:uppercase;
    text-align:center;
    width:60vw;
    padding:12px 0;
    color:gray;
    background-color:whitesmoke;
    border-radius:8px;
    border-bottom:4px solid rgb(155, 155, 155);
    cursor:fixed;
}

.inp input{
    border:none;
    text-transform:uppercase;
    padding:12px 22px;
    color:gray;
    background-color:#582592;
    border-radius:8px;
    border-bottom:4px solid #3B0C52;
}

.btn{
    text-transform:uppercase;
    text-align:center;
    width:60vw;
    padding:12px 0;
    color:white;
    background-color:#582592;
    border-radius:8px;
    border-bottom:4px solid #3B0C52;
    cursor:pointer;
}

.btn:hover{
    border-bottom:2px solid #3B0C52;
}

@media (max-width:700px) {
    .cont img{
        width:300px;
    }
  }

</style>
