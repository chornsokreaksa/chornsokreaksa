<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>Apple | Cybersecurity Enthusiast</title>
<style>
:root{
  --bg1:#02021a;
  --bg2:#08102a;
  --accent:#6fb3ff;
  --text:#eaf6ff;
}
*{box-sizing:border-box;margin:0;padding:0}
html,body{height:100%}
body{
  font-family:Inter,system-ui,Segoe UI,Roboto,Helvetica,Arial;
  background:linear-gradient(180deg,var(--bg1),var(--bg2));
  color:var(--text);
  display:flex;
  align-items:center;
  justify-content:center;
  padding:24px;
}
.scene{
  width:100%;
  max-width:980px;
  border-radius:12px;
  overflow:hidden;
  position:relative;
  box-shadow:0 10px 30px rgba(0,0,0,0.6);
  background:linear-gradient(180deg,rgba(255,255,255,0.02),rgba(255,255,255,0.01));
}
.stars{
  width:100%;
  height:220px;
  display:block;
  background:radial-gradient(1000px 200px at 20% 20%,rgba(111,179,255,0.06),transparent 8%),
             radial-gradient(800px 180px at 80% 60%,rgba(255,255,255,0.02),transparent 20%);
}
.star-layer{will-change:transform}
.layer-slow{animation:driftLeft 36s linear infinite}
.layer-mid{animation:driftLeft 18s linear infinite}
.layer-fast{animation:driftLeft 9s linear infinite}
@keyframes driftLeft{
  from{transform:translateX(0)}
  to{transform:translateX(-1200px)}
}
.planet-group{transform-origin:900px 220px;animation:spin 28s linear infinite}
@keyframes spin{
  from{transform:translate(900px,220px) rotate(0deg)}
  to{transform:translate(900px,220px) rotate(360deg)}
}
.text{
  padding:18px 24px;
  display:flex;
  align-items:center;
  gap:18px;
}
.text h1{
  font-size:1.25rem;
  margin-bottom:6px;
  color:var(--text);
}
.text p{margin:0;color:#cfefff}
.cta{
  display:inline-block;
  margin-left:auto;
  padding:10px 14px;
  background:linear-gradient(90deg,var(--accent),#95d1ff);
  color:#02102a;
  font-weight:600;
  text-decoration:none;
  border-radius:8px;
  transition:transform 140ms ease;
}
.cta:active{transform:translateY(1px)}
</style>
</head>
<body>
<div class="scene">
  <svg class="stars" viewBox="0 0 1200 400" preserveAspectRatio="xMidYMid slice" aria-hidden="true">
    <defs>
      <radialGradient id="g1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stop-color="#ffffff" stop-opacity="1"/>
        <stop offset="100%" stop-color="#ffffff" stop-opacity="0"/>
      </radialGradient>
    </defs>

    <g class="star-layer layer-slow">
      <circle cx="50" cy="30" r="1.8" fill="#ffffff" opacity="0.9"/>
      <circle cx="150" cy="90" r="1.2" fill="#f2f9ff" opacity="0.8"/>
      <circle cx="320" cy="50" r="1.6" fill="#eaf6ff" opacity="0.85"/>
      <circle cx="500" cy="120" r="1.1" fill="#ffffff" opacity="0.8"/>
      <circle cx="700" cy="40" r="2.0" fill="#fff9f2" opacity="0.95"/>
      <circle cx="920" cy="170" r="1.3" fill="#eaf6ff" opacity="0.8"/>
    </g>

    <g class="star-layer layer-mid">
      <circle cx="120" cy="200" r="1.4" fill="#ffffff"/>
      <circle cx="260" cy="70" r="1.7" fill="#fff6e6"/>
      <circle cx="420" cy="220" r="1.5" fill="#eaf6ff"/>
      <circle cx="610" cy="160" r="2.2" fill="#fff"/>
      <circle cx="860" cy="100" r="1.2" fill="#fff"/>
    </g>

    <g class="star-layer layer-fast">
      <circle cx="200" cy="20" r="1.0" fill="#fff"/>
      <circle cx="340" cy="140" r="1.0" fill="#fff"/>
      <circle cx="760" cy="60" r="1.3" fill="#fff"/>
      <circle cx="1080" cy="200" r="1.1" fill="#fff"/>
    </g>

    <g class="planet-group" transform="translate(900,220)">
      <circle class="orbit" r="90" fill="none" stroke="#ffffff22" stroke-width="1"/>
      <g class="planet" transform="translate(0,-90)">
        <circle r="22" fill="#6fb3ff"/>
        <circle r="22" fill="url(#g1)" opacity="0.18"/>
      </g>
    </g>

    <g class="shoot" opacity="0.0">
      <path d="M-40 60 Q 60 40 140 30" stroke="#fff" stroke-width="1.2" fill="none" stroke-linecap="round"/>
    </g>
  </svg>

  <div class="text">
    <h1>Apple</h1>
    <p>Cybersecurity Enthusiast</p>
    <a class="cta" href="https://github.com/chornsokreaksa">View Projects</a>
  </div>
  </div>
<script>
(function(){
  const shoot=document.querySelector('.shoot');
  function fire(){
    shoot.style.opacity='1';
    shoot.animate(
      [{opacity:1,transform:'translateX(0)'},{opacity:0,transform:'translateX(400px)'}],
      {duration:1100,easing:'cubic-bezier(0.22,0.88,0.31,1)'}
    );
    setTimeout(()=>shoot.style.opacity='0',1100);
  }
  setInterval(()=>{if(Math.random()>0.7)fire();},2500);
})();
</script>
</body>
</html>
