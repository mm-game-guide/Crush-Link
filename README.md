<!DOCTYPE html><html lang="my">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>For You 💗</title><style>
*{
  box-sizing:border-box;
}

body{
  margin:0;
  min-height:100vh;
  display:flex;
  justify-content:center;
  align-items:center;
  font-family:Arial,sans-serif;
  background:linear-gradient(135deg,#ffdde5,#f8c8dc,#ffe6ee);
  overflow:hidden;
}

.hearts{
  position:fixed;
  inset:0;
  pointer-events:none;
}

.heart{
  position:absolute;
  bottom:-30px;
  font-size:22px;
  animation:float 6s linear infinite;
  opacity:.7;
}

.heart:nth-child(1){left:10%;animation-delay:0s}
.heart:nth-child(2){left:30%;animation-delay:2s}
.heart:nth-child(3){left:50%;animation-delay:4s}
.heart:nth-child(4){left:70%;animation-delay:1s}
.heart:nth-child(5){left:90%;animation-delay:3s}

@keyframes float{
  0%{
    transform:translateY(0) scale(1);
    opacity:0;
  }
  20%{opacity:.8}
  100%{
    transform:translateY(-110vh) scale(1.5);
    opacity:0;
  }
}

.card{
  width:90%;
  max-width:420px;
  padding:35px 25px;
  text-align:center;
  background:rgba(255,255,255,.78);
  border-radius:25px;
  box-shadow:0 15px 40px rgba(150,60,90,.2);
  position:relative;
  z-index:2;
}

.heart-big{
  font-size:60px;
  animation:pulse 1.5s infinite;
}

@keyframes pulse{
  50%{transform:scale(1.12)}
}

h1{
  color:#d94f7b;
  margin:15px 0 10px;
}

p{
  color:#555;
  line-height:1.8;
}

button{
  margin-top:15px;
  padding:13px 25px;
  border:0;
  border-radius:30px;
  background:#e85d88;
  color:white;
  font-size:16px;
  font-weight:bold;
  cursor:pointer;
}

#message{
  display:none;
  margin-top:25px;
  color:#c43d68;
  font-size:17px;
  line-height:1.9;
}

.small{
  margin-top:20px;
  color:#999;
  font-size:12px;
}
</style></head><body><div class="hearts">
  <div class="heart">💗</div>
  <div class="heart">💕</div>
  <div class="heart">💖</div>
  <div class="heart">💞</div>
  <div class="heart">💗</div>
</div><div class="card">  <div class="heart-big">💗</div>  <h1>For You</h1>  <p>
    ဒီစာမျက်နှာလေးက<br>
    မင်းအတွက် သီးသန့်လုပ်ထားတာပါ 🌷
  </p>  <button onclick="showMessage()">
    💌 နှိပ်ကြည့်ပါ
  </button>  <div id="message">
    မင်းနဲ့စကားပြောရတဲ့အချိန်တိုင်း<br>
    ငါ့အတွက် ပျော်စရာလေးတစ်ခု ဖြစ်နေတယ်။ 💗<br><br>တစ်ခုတော့ ဝန်ခံချင်တယ်…<br>
မင်းကို သဘောကျနေမိပြီထင်တယ်။ 🙈💕

  </div>  <div class="small">
    Made with 💗
  </div></div><script>
function showMessage(){
  document.getElementById("message").style.display="block";
}
</script></body>
</html>
