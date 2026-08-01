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
Happy National Girlfriend’s Day, my love.
Even though we are very far apart right now, I just wanted to let you know how much you mean to me.
I believe there shouldn’t be a day to celebrate girlfriends. To me, every day should be used to celebrate how much I love you and how much you love me. One day simply isn’t enough to show this.
</p>

<p>
I remember when we first started talking. I was pretty nervous being with you at first. Not because I was embarrassed, but because I cared so much about what you thought of me. I didn’t know if I was being annoying or if you liked me at that moment.
But now I realize just how much you loved me, and I am so thankful for it.
</p>

<p>
I remember the first time I went over to your house and we went to the float parade. I looked a little lost—not because I didn’t want to be there, but because I didn’t know how to act. I wanted to make a good impression on your grandparents and your sister, but I wasn't sure how.
Eventually I became more confident and started talking more.
If I could go back in time, I would spend even more of those moments close to you, hugging you a little tighter.
</p>

<p>
There are so many things I love about you that it's impossible to list them all because I honestly love everything about you.
Your gorgeous smile.
The fun times we've had together.
Every invitation to your house.
Your constant support.
Your natural beauty—you truly don't need makeup to be the most beautiful girl in the world.
And I could keep writing forever.
</p>

<p>
One of the things I admire the most is how distance has never weakened what we have.
If anything, it has only made us stronger.
Our love proves that nothing can pull us apart, even when we can't physically be together.
I appreciate your patience more than words can express.
And while I say distance makes us stronger, that will never mean I don't want to see you.
The thing I want most is to spend every day beside you.
I want us to live together, share our own home, sleep in the same bed, and build our entire life together.
</p>

<p>
I dream about our future all the time.
A future where you're waiting for me to come home from work.
A future where instead of asking, "When can we call?" we ask,
"When are you coming home for dinner?"
I hope we can have a family together.
Taking our kids to the park every weekend.
Going to the movies to watch Toy Story 8 or Cars 6.
Bringing you flowers every single day until you have your own beautiful flower collection.
Those are the moments I look forward to the most.
</p>

<p>
But enough of me talking forever.
I just want you to know how incredibly thankful I am that you're my girlfriend.
Thank you for trusting me these past eight months.
I promise I will stay committed to you no matter how many miles separate us.
Distance will never change how deeply I love you.
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
