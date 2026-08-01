# forvalerie
<html lang="en"><head><meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>Happy National Girlfriend's Day ❤️</title>
<style>
body{margin:0;font-family:Arial,sans-serif;background:linear-gradient(#ffd6e7,#fff);overflow-x:hidden;color:#5a2a3a}
#hearts{position:fixed;inset:0;pointer-events:none}
.heart{position:absolute;color:#ff5c8a;animation:float 8s linear infinite;font-size:20px}
@keyframes float{from{transform:translateY(100vh)}to{transform:translateY(-10vh)}}
.center{display:flex;min-height:100vh;align-items:center;justify-content:center;flex-direction:column}
#envelope{width:260px;height:170px;background:#fff;border:2px solid #d88;position:relative;cursor:pointer;box-shadow:0 10px 30px rgba(0,0,0,.2)}
#flap{position:absolute;left:0;top:0;width:0;height:0;border-left:130px solid transparent;border-right:130px solid transparent;border-top:90px solid #f6a;transform-origin:top;transition:1s}
#letter{display:none;max-width:800px;background:#fff;padding:30px;border-radius:16px;box-shadow:0 8px 25px rgba(0,0,0,.2);margin:30px}
button{padding:12px 22px;border:none;border-radius:25px;background:#e91e63;color:#fff;font-size:18px;cursor:pointer}
#timer{display:flex;gap:10px;flex-wrap:wrap;justify-content:center;margin:20px 0}
.box{background:#ffe7ef;padding:10px 14px;border-radius:10px;text-align:center}
canvas{position:fixed;inset:0;pointer-events:none}
</style></head><body>
<div id="hearts"></div><canvas id="c"></canvas>
<div class="center" id="intro">
<h1>Happy National Girlfriend's Day ❤️</h1>
<p>For Valerie</p>
<button onclick="openLetter()">Open My Heart ❤️</button>
<div id="envelope"><div id="flap"></div></div>

</div>
<div id="letter">
<h2>My Love,</h2>
<p>
Happy National Girlfriend’s Day, my love. Even though we are very far apart right now, I just wanted to let you know how much you mean to me. I believe there shouldn’t be a day to celebrate girlfriends. To me everyday should be used to celebrate how much I love you and you love me. One day isn’t enough to show this. 
</p>

<p>

I remember when we first started talking. I was pretty nervous being with you first. Not because I was embarrassed, but because of how you thought about me. I didn’t know if I was being annoying or if you liked me at that moment. But now I realize how much you loved me and I am very thankful for it. 
</p>

<p>
I remember the first time I went over to your house and we went to the float parade. I looked lost there, not because I didn’t want to be there, but because I didn’t know how to act. I wanted to be a good impression to your grandparents and sister, but I didn’t know how. Then I started getting more confident and a little more talkative. If I could go back in time, I would be more close to you and hugging you more.
</p>

<p>
Going on, I just wanted to share with you the things I like about you the most. This is impossible because I love everything about you. 
Your gorgeous smile.
The fun times we've had together.
Every invitation to your house.
Your constant support.
Your natural beauty—you truly don't need makeup to be the most beautiful girl in the world.
And I could keep writing forever.
</p>

<p>
But what I also love from you is how distant doesn’t affect the love we have. If not it only made it stronger. This distance is proof that nothing can pull us apart, even if we can’t physically see each other. I want to appreciate the patience you have for me. Me talking about how the distance is making us stronger isn’t excuse to not wanting to see you. You should know that what I want the most is to be able to spend time with you and being close to you. You should know how much I want to live with you, share our own bed, our own house, everything.
</p>

<p>
And I hope our future will look like that. 
I want a future where you are waiting for me to get back from work, and not having to ask each other, “When can we call?” 
Instead I want it to be, “When are you coming home for dinner?” 
I really hope we can have a family together and taking our kids to the park every weekend, or going to the movies and watching Toy Story 8, or Cars 6. 
I would love to also bring you flowers everyday and you having a whole flower collection.
</p>

<p>
But enough yapping. 
I am really thankful you are my girlfriend and for trusting me these 8 months. 
I promise you I will stay committed with you no matter what distance is between us. 
I love you so much Valerie and I hope we continue to grow together.
</p>

<p>
I love you so much, Valerie.
Thank you for making my life brighter every single day.
I hope we continue growing together, creating memories, chasing our dreams, and loving each other more with every passing day.
❤️
</p>

<div id="timer"></div>
<h3>With all my love,<br>Diego ❤️<br>(Your future husband)</h3>
<p style="text-align:center">Forever isn't long enough with you. ❤️</p>
</div>
<script>
for(let i=0;i<40;i++){let h=document.createElement('div');h.className='heart';h.innerHTML='❤';h.style.left=Math.random()*100+'%';h.style.animationDelay=Math.random()*8+'s';h.style.fontSize=(12+Math.random()*24)+'px';document.getElementById('hearts').appendChild(h);}
function openLetter(){document.getElementById('flap').style.transform='rotateX(180deg)';setTimeout(()=>{document.getElementById('intro').style.display='none';document.getElementById('letter').style.display='block';confetti();},900);}
const start=new Date("2025-11-08T00:00:00");
function upd(){let now=new Date();let diff=now-start;let s=Math.floor(diff/1000);let sec=s%60,min=Math.floor(s/60)%60,hr=Math.floor(s/3600)%24,days=Math.floor(s/86400);let y=Math.floor(days/365);days%=365;let mo=Math.floor(days/30);days%=30;
document.getElementById('timer').innerHTML=`<div class=box>${y}<br>Years</div><div class=box>${mo}<br>Months</div><div class=box>${days}<br>Days</div><div class=box>${hr}<br>Hours</div><div class=box>${min}<br>Minutes</div><div class=box>${sec}<br>Seconds</div>`;}
setInterval(upd,1000);upd();
const cv=document.getElementById('c'),ctx=cv.getContext('2d');cv.width=innerWidth;cv.height=innerHeight;let p=[];
function confetti(){for(let i=0;i<200;i++)p.push({x:innerWidth/2,y:120,vx:(Math.random()-0.5)*8,vy:Math.random()*-8,c:`hsl(${Math.random()*360},100%,60%)`});}
function anim(){ctx.clearRect(0,0,cv.width,cv.height);p.forEach(o=>{o.x+=o.vx;o.y+=o.vy;o.vy+=.15;ctx.fillStyle=o.c;ctx.fillRect(o.x,o.y,5,5)});requestAnimationFrame(anim);}anim();
</script></body></html>
