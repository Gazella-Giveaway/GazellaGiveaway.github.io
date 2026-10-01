<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Gazella Giveaway — Redeem</title>

<style>
*{
  box-sizing:border-box;
  margin:0;
  padding:0;
}

body{
  min-height:100vh;
  display:flex;
  align-items:center;
  justify-content:center;
  padding:20px;
  overflow:hidden;
  font-family:-apple-system,BlinkMacSystemFont,"SF Pro Display","Segoe UI",sans-serif;
  color:white;
  background:#050507;
}

body::before,
body::after{
  content:"";
  position:fixed;
  width:330px;
  height:330px;
  border-radius:50%;
  filter:blur(90px);
  pointer-events:none;
  animation:floatGlow 7s ease-in-out infinite alternate;
}

body::before{
  background:rgba(115,75,255,.25);
  top:-130px;
  left:-120px;
}

body::after{
  background:rgba(0,210,255,.16);
  bottom:-130px;
  right:-120px;
  animation-delay:-3s;
}

@keyframes floatGlow{
  from{transform:translate(0,0) scale(1)}
  to{transform:translate(45px,30px) scale(1.25)}
}

.card{
  position:relative;
  width:min(440px,100%);
  padding:45px 22px 30px;
  text-align:center;

  background:rgba(255,255,255,.055);
  border:1px solid rgba(255,255,255,.14);
  border-radius:30px;

  backdrop-filter:blur(28px);
  -webkit-backdrop-filter:blur(28px);

  box-shadow:0 30px 100px rgba(0,0,0,.6);

  animation:cardIn .9s cubic-bezier(.2,.8,.2,1);
}

@keyframes cardIn{
  from{
    opacity:0;
    transform:translateY(45px) scale(.94);
  }
  to{
    opacity:1;
    transform:translateY(0) scale(1);
  }
}

.icon{
  width:68px;
  height:68px;
  margin:0 auto 20px;

  display:flex;
  align-items:center;
  justify-content:center;

  border-radius:22px;
  background:rgba(255,255,255,.08);
  border:1px solid rgba(255,255,255,.15);

  font-size:30px;

  animation:bob 3s ease-in-out infinite;
}

@keyframes bob{
  0%,100%{transform:translateY(0) rotate(0)}
  50%{transform:translateY(-9px) rotate(5deg)}
}

.label{
  font-size:10px;
  letter-spacing:4px;
  opacity:.5;
}

h1{
  margin-top:8px;
  font-size:42px;
  letter-spacing:-3px;
}

.amount{
  margin:14px 0 18px;

  font-size:clamp(50px,15vw,68px);
  font-weight:950;
  letter-spacing:-4px;

  background:linear-gradient(
    100deg,
    #fff,
    #bba8ff,
    #70eaff,
    #fff
  );

  background-size:250% auto;
  -webkit-background-clip:text;
  background-clip:text;
  color:transparent;

  animation:shine 4s linear infinite;
}

@keyframes shine{
  to{background-position:250% center}
}

.message{
  color:rgba(255,255,255,.57);
  font-size:14px;
  line-height:1.7;
}

.instagram{
  position:relative;
  overflow:hidden;

  display:flex;
  align-items:center;
  gap:13px;

  width:100%;
  margin-top:28px;
  padding:16px;

  text-decoration:none;
  color:white;

  border-radius:18px;
  border:1px solid rgba(255,255,255,.14);
  background:rgba(255,255,255,.06);

  transition:.3s;
}

.instagram::before{
  content:"";
  position:absolute;
  top:0;
  left:-120%;
  width:70%;
  height:100%;

  background:linear-gradient(
    90deg,
    transparent,
    rgba(255,255,255,.18),
    transparent
  );

  transform:skewX(-20deg);
  animation:buttonShine 3.5s infinite;
}

@keyframes buttonShine{
  0%{left:-120%}
  45%,100%{left:150%}
}

.instagram:active{
  transform:scale(.97);
}

.ig{
  width:46px;
  height:46px;
  flex-shrink:0;

  display:flex;
  align-items:center;
  justify-content:center;

  border-radius:14px;

  background:linear-gradient(
    135deg,
    #833ab4,
    #fd1d1d,
    #fcb045
  );

  font-size:24px;
}

.text{
  flex:1;
  text-align:left;
}

.text small{
  display:block;
  margin-bottom:3px;
  font-size:8px;
  letter-spacing:2px;
  opacity:.5;
}

.text strong{
  font-size:15px;
}

.arrow{
  font-size:21px;
  opacity:.6;
}

.note{
  margin-top:17px;
  font-size:10px;
  color:rgba(255,255,255,.35);
}

.note strong{
  color:rgba(255,255,255,.7);
}

@media(max-width:420px){
  .card{
    padding:38px 17px 27px;
  }

  h1{
    font-size:36px;
  }

  .amount{
    font-size:51px;
  }
}
</style>
</head>

<body>

<div class="card">

  <div class="icon">✦</div>

  <div class="label">GAZELLA GIVEAWAY</div>

  <h1>YOU MADE IT.</h1>

  <div class="amount">₹25,000</div>

  <p class="message">
    Congratulations. You achieved a perfect score.
    Continue your redemption through Instagram.
  </p>

  <a
    class="instagram"
    href="https://www.instagram.com/gazelle.giveaway/"
    target="_blank"
    rel="noopener noreferrer"
  >

    <div class="ig">◎</div>

    <div class="text">
      <small>REDEEM THROUGH</small>
      <strong>Instagram DM</strong>
    </div>

    <div class="arrow">↗</div>

  </a>

  <p class="note">
    Send <strong>REDEEM</strong> in your Instagram message.
  </p>

</div>

</body>
</html>
