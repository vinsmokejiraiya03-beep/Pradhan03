<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Guess the Teacher</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Caveat:wght@600;700&family=Poppins:wght@400;500;600;700&display=swap" rel="stylesheet">
<style>
  :root{
    --bg-deep:#151F1A;
    --board:#24352E;
    --board-light:#31473D;
    --chalk:#F6F3EC;
    --chalk-dim:#C9D2CA;
    --gold:#E8B339;
    --coral:#E85D4E;
    --teal:#7FA9A0;
    --radius:18px;
  }
  *{box-sizing:border-box;}
  html,body{height:100%;}
  body{
    margin:0;
    min-height:100vh;
    background:
      radial-gradient(1400px 800px at 15% -15%, #35513F 0%, transparent 55%),
      radial-gradient(1100px 700px at 105% 10%, #2E4A3E 0%, transparent 50%),
      radial-gradient(1200px 800px at 50% 120%, #1C2C22 0%, transparent 55%),
      linear-gradient(180deg, #182620 0%, #131E19 100%);
    color:var(--chalk);
    font-family:'Poppins',sans-serif;
    overflow-x:hidden;
  }
  .hidden{display:none !important;}

  .doodles{position:fixed; inset:0; z-index:0; pointer-events:none;}
  .doodle{position:absolute; stroke:var(--chalk); fill:none; stroke-width:1.3; opacity:.06;}
  .d1{width:120px; top:6%; left:4%; animation:floatD1 9s ease-in-out infinite;}
  .d2{width:90px; bottom:8%; left:8%; animation:floatD2 10s ease-in-out infinite 1.4s;}
  .d3{width:130px; top:10%; right:5%; animation:floatD3 8s ease-in-out infinite .8s;}
  .d4{width:100px; bottom:6%; right:7%; animation:floatD4 11s ease-in-out infinite 2.2s;}
  @keyframes floatD1{0%,100%{transform:rotate(-12deg) translateY(0);} 50%{transform:rotate(-8deg) translateY(-14px);}}
  @keyframes floatD2{0%,100%{transform:rotate(8deg) translateY(0);} 50%{transform:rotate(12deg) translateY(-10px);}}
  @keyframes floatD3{0%,100%{transform:rotate(10deg) translateY(0);} 50%{transform:rotate(6deg) translateY(-16px);}}
  @keyframes floatD4{0%,100%{transform:rotate(-10deg) translateY(0);} 50%{transform:rotate(-14deg) translateY(-12px);}}

  /* ---------- chalk dust texture ---------- */
  .dust{
    position:fixed; inset:0; pointer-events:none; z-index:0; opacity:.5;
    background-image:
      radial-gradient(1px 1px at 10% 20%, rgba(246,243,236,.25) 50%, transparent 51%),
      radial-gradient(1px 1px at 80% 60%, rgba(246,243,236,.18) 50%, transparent 51%),
      radial-gradient(1.5px 1.5px at 40% 80%, rgba(246,243,236,.15) 50%, transparent 51%),
      radial-gradient(1px 1px at 65% 15%, rgba(246,243,236,.2) 50%, transparent 51%),
      radial-gradient(1.5px 1.5px at 90% 85%, rgba(246,243,236,.15) 50%, transparent 51%);
    background-size:600px 600px;
  }

  /* ================= SETUP SCREEN ================= */
  #setup-screen{
    position:relative; z-index:1;
    max-width:1080px; margin:0 auto;
    padding:48px 24px 120px;
  }
  .eyebrow-free-title{
    font-family:'Caveat',cursive;
    font-weight:700;
    font-size:clamp(40px, 6vw, 64px);
    line-height:1;
    margin:0 0 6px;
    color:var(--gold);
    text-shadow:0 2px 0 rgba(0,0,0,.2);
  }
  .subtitle{
    color:var(--chalk-dim);
    font-size:15px;
    max-width:560px;
    margin:0 0 34px;
    line-height:1.6;
  }
  .grid{
    display:grid;
    grid-template-columns:repeat(auto-fill, minmax(190px, 1fr));
    gap:22px;
  }
  .card{
    background:var(--board);
    border:1px solid rgba(246,243,236,.08);
    border-radius:var(--radius);
    padding:14px;
    position:relative;
    display:flex; flex-direction:column; gap:10px;
    box-shadow:0 10px 24px rgba(0,0,0,.25);
  }
  .photo-slot{
    width:100%; aspect-ratio:1/1;
    border-radius:12px;
    border:2px dashed rgba(246,243,236,.28);
    background:var(--board-light);
    display:flex; align-items:center; justify-content:center;
    cursor:pointer; overflow:hidden; position:relative;
  }
  .photo-slot img{width:100%; height:100%; object-fit:cover; display:block;}
  .photo-slot .placeholder-icon{color:rgba(246,243,236,.4); text-align:center; padding:10px;}
  .photo-slot .placeholder-icon svg{width:44px; height:44px; margin-bottom:6px;}
  .photo-slot .placeholder-icon span{display:block; font-size:12px;}
  .photo-slot:hover{border-color:var(--gold);}
  .name-input{
    width:100%;
    background:var(--board-light);
    border:1px solid rgba(246,243,236,.12);
    color:var(--chalk);
    font-family:'Poppins',sans-serif;
    font-size:14px;
    font-weight:500;
    padding:9px 10px;
    border-radius:8px;
    outline:none;
  }
  .name-input:focus{border-color:var(--gold);}
  .remove-btn{
    position:absolute; top:8px; right:8px;
    width:26px; height:26px; border-radius:50%;
    background:rgba(21,31,26,.7);
    border:1px solid rgba(246,243,236,.2);
    color:var(--chalk); cursor:pointer;
    display:flex; align-items:center; justify-content:center;
    font-size:14px; line-height:1; z-index:2;
  }
  .remove-btn:hover{background:var(--coral); border-color:var(--coral);}
  .add-card{
    border:2px dashed rgba(246,243,236,.25);
    border-radius:var(--radius);
    display:flex; align-items:center; justify-content:center;
    flex-direction:column; gap:6px;
    color:var(--chalk-dim);
    cursor:pointer; min-height:190px;
    background:transparent;
  }
  .add-card:hover{border-color:var(--gold); color:var(--gold);}
  .add-card span.plus{font-size:30px; line-height:1;}
  .add-card span.label{font-size:13px;}

  .setup-footer{
    position:fixed; left:0; right:0; bottom:0; z-index:5;
    background:linear-gradient(180deg, transparent, rgba(21,31,26,.92) 30%);
    padding:26px 24px 22px;
    display:flex; align-items:center; justify-content:center; gap:16px;
  }
  .btn{
    font-family:'Poppins',sans-serif;
    font-weight:600;
    font-size:14px;
    border-radius:999px;
    padding:13px 26px;
    border:none;
    cursor:pointer;
    display:inline-flex; align-items:center; gap:8px;
    transition:transform .15s ease;
  }
  .btn:active{transform:scale(.96);}
  .btn-primary{background:var(--gold); color:#1E1608;}
  .btn-primary:disabled{opacity:.4; cursor:not-allowed;}
  .btn-ghost{background:rgba(246,243,236,.08); color:var(--chalk); border:1px solid rgba(246,243,236,.18);}
  .btn{position:relative; overflow:hidden;}
  .btn .ripple{
    position:absolute; border-radius:50%; pointer-events:none;
    background:rgba(255,255,255,.55); transform:scale(0); opacity:.6;
    animation:rippleGrow .55s ease-out forwards;
  }
  @keyframes rippleGrow{ to{ transform:scale(1); opacity:0; } }
  .btn-primary .ripple{background:rgba(30,22,8,.35);}
  .count-pill{color:var(--chalk-dim); font-size:13px;}

  /* ================= PRESENT SCREEN ================= */
  #present-screen{
    position:fixed; inset:0; z-index:10;
    display:flex; flex-direction:column;
    background:
      radial-gradient(1400px 900px at 50% 0%, #2C4139 0%, transparent 55%),
      var(--bg-deep);
    overflow:hidden;
  }
  #present-screen::before{
    content:"Can you?";
    position:absolute;
    top:50%; left:50%;
    transform:translate(-50%,-50%) rotate(-16deg);
    font-family:'Caveat',cursive;
    font-weight:700;
    font-size:min(26vw, 420px);
    line-height:1;
    color:rgba(246,243,236,.06);
    white-space:nowrap;
    z-index:0;
    pointer-events:none;
    user-select:none;
  }
  .present-topbar{
    display:flex; align-items:center; justify-content:space-between;
    padding:18px 20px;
    position:relative; z-index:3;
  }
  .icon-btn{
    width:40px; height:40px; border-radius:50%;
    background:rgba(246,243,236,.08);
    border:1px solid rgba(246,243,236,.16);
    color:var(--chalk); cursor:pointer;
    display:flex; align-items:center; justify-content:center;
    font-size:16px;
  }
  .icon-btn:hover{background:rgba(246,243,236,.16);}
  .dots{display:flex; gap:8px;}
  .dot{width:8px; height:8px; border-radius:50%; background:rgba(246,243,236,.25); cursor:pointer; transition:background .2s, transform .2s;}
  .dot.active{background:var(--gold); transform:scale(1.3);}

  .stage-wrap{
    flex:1; display:flex; align-items:center; justify-content:center;
    position:relative; padding:10px 90px 40px;
  }
  .stage-wrap::before{
    content:"";
    position:absolute; left:50%; top:50%; transform:translate(-50%,-50%) scale(1);
    width:70vw; height:70vw; max-width:1000px; max-height:1000px;
    background:radial-gradient(circle, rgba(232,179,57,.14) 0%, rgba(232,179,57,0) 62%);
    animation:glowPulse 7s ease-in-out infinite;
    z-index:0; pointer-events:none;
  }
  @keyframes glowPulse{
    0%,100%{ transform:translate(-50%,-50%) scale(1); opacity:.75;}
    50%{ transform:translate(-50%,-50%) scale(1.08); opacity:1;}
  }
  .nav-arrow{
    position:absolute; top:50%; transform:translateY(-50%);
    width:60px; height:60px; border-radius:50%;
    background:rgba(246,243,236,.06);
    border:1px solid rgba(246,243,236,.15);
    color:var(--chalk); font-size:24px; cursor:pointer;
    display:flex; align-items:center; justify-content:center;
    z-index:4;
  }
  .nav-arrow:hover{background:rgba(246,243,236,.14);}
  .nav-arrow:disabled{opacity:.25; cursor:not-allowed;}
  .nav-prev{left:18px;}
  .nav-next{right:18px;}

  .board-frame{
    width:min(880px, 88vw);
    background:var(--board);
    border-radius:28px;
    border:1px solid rgba(246,243,236,.08);
    box-shadow:0 40px 90px rgba(0,0,0,.45), inset 0 0 0 10px var(--board-light);
    padding:56px 60px 50px;
    position:relative; z-index:1;
    overflow:hidden;
    min-height:min(760px, 82vh);
    display:flex; flex-direction:column; align-items:center;
    justify-content:center;
    transition:box-shadow .4s ease;
    perspective:1000px;
  }
  .board-frame.urgent-glow{
    animation:urgentGlow 1s ease-in-out infinite;
  }
  @keyframes urgentGlow{
    0%,100%{ box-shadow:0 40px 90px rgba(0,0,0,.45), inset 0 0 0 10px var(--board-light), 0 0 0 0 rgba(232,93,78,.35); }
    50%{ box-shadow:0 40px 90px rgba(0,0,0,.45), inset 0 0 0 10px var(--board-light), 0 0 0 16px rgba(232,93,78,0); }
  }
  .board-frame.shake{ animation:boardShake .45s ease; }
  @keyframes boardShake{
    0%,100%{ transform:translateX(0); }
    20%{ transform:translateX(-8px) rotate(-.4deg); }
    40%{ transform:translateX(7px) rotate(.4deg); }
    60%{ transform:translateX(-5px); }
    80%{ transform:translateX(4px); }
  }
  .flash-overlay{
    position:fixed; inset:0; z-index:20; background:#fff; opacity:0;
    pointer-events:none;
  }
  .flash-overlay.go{ animation:cameraFlash .5s ease-out; }
  @keyframes cameraFlash{ 0%{opacity:0;} 12%{opacity:.85;} 100%{opacity:0;} }

  /* ---- reveal transition variants (randomized each time) ---- */
  @keyframes revealZoomPop{
    0%{ transform:scale(.55); opacity:0; }
    65%{ transform:scale(1.06); opacity:1; }
    100%{ transform:scale(1); opacity:1; }
  }
  @keyframes revealSlideUp{
    0%{ transform:translateY(70px); opacity:0; }
    100%{ transform:translateY(0); opacity:1; }
  }
  @keyframes revealSpinIn{
    0%{ transform:rotate(-16deg) scale(.7); opacity:0; }
    100%{ transform:rotate(0deg) scale(1); opacity:1; }
  }
  @keyframes revealFlip{
    0%{ transform:rotateY(90deg); opacity:0; }
    100%{ transform:rotateY(0deg); opacity:1; }
  }
  @keyframes revealSlideLeft{
    0%{ transform:translateX(90px); opacity:0; }
    100%{ transform:translateX(0); opacity:1; }
  }
  @keyframes revealDropBounce{
    0%{ transform:translateY(-90px); opacity:0; }
    60%{ transform:translateY(14px); opacity:1; }
    80%{ transform:translateY(-6px); }
    100%{ transform:translateY(0); }
  }
  .phase.reveal-anim-zoom{ animation:revealZoomPop .6s cubic-bezier(.34,1.56,.64,1) both; }
  .phase.reveal-anim-slideup{ animation:revealSlideUp .55s ease-out both; }
  .phase.reveal-anim-spin{ animation:revealSpinIn .6s ease-out both; }
  .phase.reveal-anim-flip{ animation:revealFlip .6s ease-out both; transform-style:preserve-3d; }
  .phase.reveal-anim-slideleft{ animation:revealSlideLeft .55s ease-out both; }
  .phase.reveal-anim-drop{ animation:revealDropBounce .65s cubic-bezier(.34,1.56,.64,1) both; }

  .phase{
    width:100%;
    display:flex; flex-direction:column; align-items:center;
    animation:riseIn .5s ease both;
    position:relative;
    z-index:1;
  }
  @keyframes riseIn{from{opacity:0; transform:translateY(14px);} to{opacity:1; transform:translateY(0);}}

  .prompt{
    font-family:'Caveat',cursive; font-weight:700;
    font-size:clamp(30px, 4vw, 42px); color:var(--gold);
    margin:0 0 26px; text-align:center;
  }

  .photo-frame{
    width:min(360px, 40vw); height:min(360px, 40vw); border-radius:20px;
    overflow:hidden; background:var(--board-light);
    border:4px solid rgba(246,243,236,.15);
    display:flex; align-items:center; justify-content:center;
    margin-bottom:30px;
  }
  .photo-frame img{width:100%; height:100%; object-fit:cover;}
  .photo-frame .placeholder-icon{color:rgba(246,243,236,.35); text-align:center;}
  .photo-frame .placeholder-icon svg{width:72px; height:72px;}

  .timer-ring-wrap{position:relative; width:190px; height:190px; margin:6px 0 14px;}
  .timer-ring-wrap svg{transform:rotate(-90deg); width:190px; height:190px;}
  .timer-ring-bg{fill:none; stroke:rgba(246,243,236,.12); stroke-width:8;}
  .timer-ring-fg{fill:none; stroke:var(--gold); stroke-width:8; stroke-linecap:round; transition:stroke-dashoffset 1s linear, stroke .3s;}
  .timer-ring-fg.urgent{stroke:var(--coral);}
  .timer-num{
    position:absolute; inset:0; display:flex; align-items:center; justify-content:center;
    font-size:50px; font-weight:700; font-family:'Poppins',sans-serif;
  }
  .timer-num.tick{ animation:tickPop .3s cubic-bezier(.34,1.56,.64,1); }
  @keyframes tickPop{ 0%{transform:scale(1);} 35%{transform:scale(1.28);} 100%{transform:scale(1);} }
  .timer-num.urgent-num{ color:var(--coral); }
  .timer-ring-wrap.urgent-wrap{ animation:ringUrgentPulse .5s ease-in-out infinite; }
  @keyframes ringUrgentPulse{ 0%,100%{transform:scale(1);} 50%{transform:scale(1.06);} }

  .times-up-banner{
    font-family:'Caveat',cursive; font-weight:700;
    font-size:0; color:#fff;
    text-align:center;
    max-height:0; overflow:hidden;
    opacity:0; transform:scale(.7);
    border-radius:14px;
  }
  .times-up-banner.shown{
    font-size:clamp(26px, 4vw, 40px);
    max-height:120px;
    opacity:1; transform:scale(1);
    background:var(--coral);
    color:#fff;
    padding:12px 28px;
    margin:0 0 20px;
    box-shadow:0 10px 24px rgba(232,93,78,.45);
    animation:timesUpPop .5s cubic-bezier(.34,1.56,.64,1) both,
              timesUpShake .4s ease .5s,
              timesUpGlow 1.1s ease-in-out infinite .9s;
  }
  @keyframes timesUpPop{0%{opacity:0; transform:scale(.5);} 70%{opacity:1; transform:scale(1.12);} 100%{opacity:1; transform:scale(1);}}
  @keyframes timesUpShake{0%,100%{transform:scale(1) rotate(0);} 25%{transform:scale(1) rotate(-3deg);} 75%{transform:scale(1) rotate(3deg);}}
  @keyframes timesUpGlow{
    0%,100%{ box-shadow:0 10px 24px rgba(232,93,78,.45); }
    50%{ box-shadow:0 10px 36px rgba(232,93,78,.8), 0 0 0 9px rgba(232,93,78,.16); }
  }

  .pulse-btn{animation:btnPulse 1.1s ease-in-out infinite;}
  @keyframes btnPulse{0%,100%{box-shadow:0 0 0 0 rgba(232,179,57,.55);} 50%{box-shadow:0 0 0 14px rgba(232,179,57,0);}}

  .stage-actions{display:flex; gap:14px; flex-wrap:wrap; justify-content:center;}
  #present-screen .btn{font-size:16px; padding:15px 30px;}

  .hint-text{
    min-height:56px;
    display:flex; align-items:center; justify-content:center;
    color:#1E1608;
    background:var(--gold);
    font-family:'Poppins',sans-serif;
    font-weight:700;
    font-size:clamp(18px, 2.6vw, 26px);
    padding:12px 26px;
    border-radius:14px;
    text-align:center;
    margin:-6px 0 24px;
    opacity:0;
    transform:translateY(-90px) scale(.92);
    box-shadow:0 10px 22px rgba(0,0,0,.25);
  }
  .hint-text.shown{
    animation:hintDrop .65s cubic-bezier(.34,1.56,.64,1) forwards;
  }
  @keyframes hintDrop{
    0%{ transform:translateY(-90px) scale(.9); opacity:0;}
    60%{ transform:translateY(6px) scale(1.03); opacity:1;}
    100%{ transform:translateY(0) scale(1); opacity:1;}
  }

  .rules-list{
    list-style:none; margin:0 0 30px; padding:0;
    width:100%; max-width:520px;
    display:flex; flex-direction:column; gap:18px;
  }
  .rules-list li{
    display:flex; gap:16px; align-items:flex-start;
    font-size:18px; line-height:1.5; color:var(--chalk-dim);
  }
  .rules-list .rule-badge{
    flex:0 0 auto; width:32px; height:32px; border-radius:50%;
    background:var(--board-light); border:1px solid rgba(246,243,236,.15);
    display:flex; align-items:center; justify-content:center;
    font-size:15px; font-weight:700; color:var(--gold);
    font-family:'Poppins',sans-serif;
  }

  .reveal-name{
    font-family:'Caveat',cursive; font-weight:700;
    font-size:clamp(56px, 10vw, 110px);
    color:var(--chalk);
    text-align:center; margin:50px 0 10px;
    text-shadow:0 3px 0 rgba(0,0,0,.25);
  }
  .reveal-name .letter{
    display:inline-block;
    opacity:0; transform:translateY(30px) rotate(-6deg) scale(.6);
    animation:letterPop .5s cubic-bezier(.34,1.56,.64,1) forwards;
  }
  @keyframes letterPop{
    to{ opacity:1; transform:translateY(0) rotate(0) scale(1); }
  }
  .reveal-sub{color:var(--chalk-dim); font-size:18px; margin-bottom:34px; opacity:0; animation:fadeUp .6s ease forwards; animation-delay:.9s;}
  @keyframes fadeUp{ from{opacity:0; transform:translateY(10px);} to{opacity:1; transform:translateY(0);} }

  /* ---- Thank-you finishing screen ---- */
  .thankyou-decor{ position:absolute; inset:0; pointer-events:none; z-index:0; overflow:hidden; }
  .ty-icon{ position:absolute; stroke:var(--gold); fill:none; stroke-width:1.4; }
  .ty-heart-tl{ width:38px; top:26px; left:30px; opacity:.4; }
  .ty-star-tr{ width:30px; top:24px; right:110px; opacity:.35; }
  .ty-apple-tr{ width:52px; top:54px; right:34px; opacity:.4; }
  .ty-hearts-r{ width:20px; top:150px; right:60px; opacity:.3; }
  .ty-leaf-bl{ width:130px; bottom:38px; left:18px; opacity:.35; transform:rotate(-6deg); }
  .ty-leaf-br{ width:130px; bottom:38px; right:18px; opacity:.35; transform:rotate(6deg) scaleX(-1); }
  .ty-emoji{ font-size:44px; margin-bottom:4px; opacity:0; animation:fadeUp .5s ease forwards; animation-delay:.1s; }
  .ty-title{
    font-family:'Caveat',cursive; font-weight:700;
    font-size:clamp(60px, 10.5vw, 122px);
    color:var(--chalk);
    text-align:center; margin:0 0 4px;
    text-shadow:0 3px 0 rgba(0,0,0,.25);
    opacity:0; animation:fadeUp .6s ease forwards; animation-delay:.2s;
  }
  .ty-divider{ display:flex; align-items:center; gap:14px; margin-bottom:20px; opacity:0; animation:fadeUp .6s ease forwards; animation-delay:.4s; }
  .ty-divider span{ width:56px; height:1px; background:rgba(232,179,57,.5); display:block; }
  .ty-divider-heart{ width:15px; height:15px; fill:var(--gold); flex-shrink:0; }
  .ty-sub{
    color:var(--chalk-dim); font-size:18px; line-height:1.7; text-align:center;
    margin-bottom:26px; opacity:0; animation:fadeUp .6s ease forwards; animation-delay:.55s;
  }
  .ty-highlight{
    font-family:'Caveat',cursive; font-weight:700;
    font-size:clamp(28px, 3.6vw, 40px);
    color:var(--gold); display:inline-block; margin:2px 0;
  }
  .ty-badge{
    border:1px solid rgba(232,179,57,.5);
    border-radius:14px;
    padding:12px 32px;
    text-align:center;
    margin-bottom:26px;
    opacity:0; animation:fadeUp .6s ease forwards; animation-delay:.7s;
  }
  .ty-badge-top{ display:block; font-family:'Caveat',cursive; font-size:19px; color:var(--chalk-dim); letter-spacing:2px; }
  .ty-badge-main{ display:block; font-weight:700; font-size:clamp(19px,2.4vw,26px); letter-spacing:3px; color:var(--chalk); margin-top:2px; }
  .photo-frame{animation:photoPop .55s cubic-bezier(.34,1.56,.64,1) both;}
  @keyframes photoPop{
    0%{ opacity:0; transform:scale(.7) rotate(-4deg); }
    70%{ opacity:1; transform:scale(1.04) rotate(1deg); }
    100%{ opacity:1; transform:scale(1) rotate(0); }
  }
  .stage-actions .btn{animation:fadeUp .5s ease both; animation-delay:.15s;}

  .confetti-canvas{position:absolute; inset:0; pointer-events:none; z-index:2;}

  @media (max-width:640px){
    .board-frame{padding:32px 22px 28px; min-height:auto;}
    .photo-frame{width:200px; height:200px;}
    .nav-arrow{width:44px; height:44px; font-size:17px;}
    .stage-wrap{padding:10px 50px 30px;}
    .timer-ring-wrap{width:150px; height:150px;}
    .timer-ring-wrap svg{width:150px; height:150px;}
  }
</style>
</head>
<body>
<div class="dust"></div>
<div class="flash-overlay" id="flash-overlay"></div>
<div class="doodles" aria-hidden="true">
  <svg class="doodle d1" viewBox="0 0 60 60" xmlns="http://www.w3.org/2000/svg"><path d="M30 4 L36 22 L55 22 L39 33 L45 52 L30 41 L15 52 L21 33 L5 22 L24 22 Z"/></svg>
  <svg class="doodle d2" viewBox="0 0 60 60" xmlns="http://www.w3.org/2000/svg"><path d="M30 14c-6-10-20-8-18 3 1 8 10 15 18 27 8-12 17-19 18-27 2-11-12-13-18-3z"/><path d="M30 14 L32 4"/></svg>
  <svg class="doodle d3" viewBox="0 0 60 40" xmlns="http://www.w3.org/2000/svg"><path d="M2 14 L30 4 L58 14 L30 24 Z"/><path d="M14 18 V30 C14 34 24 36 30 36 C36 36 46 34 46 30 V18"/></svg>
  <svg class="doodle d4" viewBox="0 0 60 50" xmlns="http://www.w3.org/2000/svg"><path d="M30 8 C24 3 10 3 6 8 V42 C10 37 24 37 30 42 C36 37 50 37 54 42 V8 C50 3 36 3 30 8 Z"/><path d="M30 8 V42"/></svg>
</div>

<!-- ===================== SETUP SCREEN ===================== -->
<div id="setup-screen">
  <h1 class="eyebrow-free-title">Guess the Teacher 🍎</h1>
  <p class="subtitle">Add each teacher's childhood photo and name below — these are just placeholders, tap any photo to swap it later. When you're ready, start the presentation and let the class guess.</p>
  <div class="grid" id="teacher-grid"></div>
  <input type="file" id="file-input" accept="image/*" class="hidden">
</div>

<div class="setup-footer">
  <span class="count-pill" id="count-pill"></span>
  <button class="btn btn-ghost" id="reset-btn">Reset all</button>
  <button class="btn btn-ghost" id="download-btn">💾 Download my version</button>
  <button class="btn btn-primary" id="start-btn">Start presentation</button>
</div>

<!-- ===================== PRESENT SCREEN ===================== -->
<div id="present-screen" class="hidden">
  <div class="present-topbar">
    <button class="icon-btn" id="exit-btn" title="Back to setup">✕</button>
    <div class="dots" id="dots"></div>
    <button class="icon-btn" id="fullscreen-btn" title="Fullscreen">⛶</button>
  </div>
  <div class="stage-wrap">
    <button class="nav-arrow nav-prev" id="prev-btn">‹</button>
    <div class="board-frame" id="board-frame"></div>
    <button class="nav-arrow nav-next" id="next-btn">›</button>
  </div>
</div>

<script>
(function(){
  "use strict";

  var STORAGE_KEY = "guess-the-teacher:list";
  var teachers = [];
  var saveTimer = null;

  function placeholderIconSVG(){
    return '<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">'+
      '<path d="M12 3L2 8l10 5 10-5-10-5z" stroke="currentColor" stroke-width="1.3" stroke-linejoin="round"/>'+
      '<path d="M6 10.5V15c0 1.7 2.7 3 6 3s6-1.3 6-3v-4.5" stroke="currentColor" stroke-width="1.3"/>'+
      '</svg>';
  }

  var TOTAL_TIME = 30;
  var HINT_AT = 15;

  function defaultTeachers(){
    return [
      {id: cryptoId(), name: "Teacher 1", photo: "", hint: ""},
      {id: cryptoId(), name: "Teacher 2", photo: "", hint: ""},
      {id: cryptoId(), name: "Teacher 3", photo: "", hint: ""},
      {id: cryptoId(), name: "Teacher 4", photo: "", hint: ""}
    ];
  }
  function cryptoId(){ return Math.random().toString(36).slice(2,10)+Date.now().toString(36); }

  async function loadTeachers(){
    var grid = document.getElementById("teacher-grid");
    grid.innerHTML = '<p style="color:var(--chalk-dim);font-size:14px;">Loading…</p>';
    try{
      var res = await window.storage.get(STORAGE_KEY, false);
      teachers = (res && res.value) ? JSON.parse(res.value) : defaultTeachers();
    }catch(e){
      teachers = defaultTeachers();
    }
    if(!Array.isArray(teachers) || teachers.length===0){ teachers = defaultTeachers(); }
    renderGrid();
  }

  function scheduleSave(){
    clearTimeout(saveTimer);
    saveTimer = setTimeout(saveTeachers, 400);
  }
  async function saveTeachers(){
    try{
      var result = await window.storage.set(STORAGE_KEY, JSON.stringify(teachers), false);
      if(!result){ console.error("Storage save returned null"); }
    }catch(e){
      console.error("Storage save failed", e);
    }
  }

  function renderGrid(){
    var grid = document.getElementById("teacher-grid");
    grid.innerHTML = "";
    teachers.forEach(function(t, idx){
      var card = document.createElement("div");
      card.className = "card";

      var removeBtn = document.createElement("button");
      removeBtn.className = "remove-btn";
      removeBtn.innerHTML = "✕";
      removeBtn.title = "Remove";
      removeBtn.addEventListener("click", function(){
        teachers.splice(idx,1);
        scheduleSave();
        renderGrid();
      });
      card.appendChild(removeBtn);

      var slot = document.createElement("div");
      slot.className = "photo-slot";
      slot.innerHTML = t.photo
        ? '<img src="'+t.photo+'" alt="'+escapeHtml(t.name)+'">'
        : '<div class="placeholder-icon">'+placeholderIconSVG()+'<span>Tap to add photo</span></div>';
      slot.addEventListener("click", function(){
        openFilePicker(function(dataUrl){
          teachers[idx].photo = dataUrl;
          scheduleSave();
          renderGrid();
        });
      });
      card.appendChild(slot);

      var nameInput = document.createElement("input");
      nameInput.className = "name-input";
      nameInput.type = "text";
      nameInput.value = t.name;
      nameInput.placeholder = "Teacher's name";
      nameInput.addEventListener("input", function(){
        teachers[idx].name = nameInput.value;
        scheduleSave();
        updateCountPill();
        renderDots();
      });
      card.appendChild(nameInput);

      var hintInput = document.createElement("input");
      hintInput.className = "name-input";
      hintInput.type = "text";
      hintInput.value = t.hint || "";
      hintInput.placeholder = "Hint (optional), e.g. Loves painting";
      hintInput.addEventListener("input", function(){
        teachers[idx].hint = hintInput.value;
        scheduleSave();
      });
      card.appendChild(hintInput);

      grid.appendChild(card);
    });

    var addCard = document.createElement("div");
    addCard.className = "add-card";
    addCard.innerHTML = '<span class="plus">+</span><span class="label">Add teacher</span>';
    addCard.addEventListener("click", function(){
      teachers.push({id: cryptoId(), name: "Teacher "+(teachers.length+1), photo: "", hint: ""});
      scheduleSave();
      renderGrid();
    });
    grid.appendChild(addCard);

    updateCountPill();
  }

  function escapeHtml(s){
    var d = document.createElement("div");
    d.textContent = s || "";
    return d.innerHTML;
  }

  function updateCountPill(){
    document.getElementById("count-pill").textContent =
      teachers.length + (teachers.length===1 ? " teacher added" : " teachers added");
    document.getElementById("start-btn").disabled = teachers.length===0;
  }

  function openFilePicker(cb){
    var input = document.getElementById("file-input");
    input.value = "";
    input.onchange = function(){
      var file = input.files && input.files[0];
      if(!file) return;
      var reader = new FileReader();
      reader.onload = function(e){
        resizeImage(e.target.result, 900, 0.82, cb);
      };
      reader.readAsDataURL(file);
    };
    input.click();
  }

  function resizeImage(dataUrl, maxDim, quality, cb){
    var img = new Image();
    img.onload = function(){
      var w = img.width, h = img.height;
      var scale = Math.min(1, maxDim / Math.max(w,h));
      var cw = Math.round(w*scale), ch = Math.round(h*scale);
      var canvas = document.createElement("canvas");
      canvas.width = cw; canvas.height = ch;
      var ctx = canvas.getContext("2d");
      ctx.drawImage(img, 0, 0, cw, ch);
      cb(canvas.toDataURL("image/jpeg", quality));
    };
    img.onerror = function(){ cb(dataUrl); };
    img.src = dataUrl;
  }

  document.addEventListener("click", function(e){
    var btn = e.target.closest && e.target.closest(".btn");
    if(!btn) return;
    var rect = btn.getBoundingClientRect();
    var size = Math.max(rect.width, rect.height) * 1.6;
    var ripple = document.createElement("span");
    ripple.className = "ripple";
    ripple.style.width = ripple.style.height = size+"px";
    ripple.style.left = (e.clientX - rect.left - size/2)+"px";
    ripple.style.top = (e.clientY - rect.top - size/2)+"px";
    btn.appendChild(ripple);
    setTimeout(function(){ ripple.remove(); }, 550);
  });

  document.getElementById("download-btn").addEventListener("click", function(){
    downloadStandaloneVersion();
  });

  function downloadStandaloneVersion(){
    try{
      // Serialize current teachers (names, hints, photos as data URLs) safely for embedding in a <script>.
      var json = JSON.stringify(teachers).replace(/<\/script/gi, "<\\/script");

      // Grab the current page's full HTML.
      var html = document.documentElement.outerHTML;

      // Bake the current data straight into defaultTeachers() so this exact
      // set of teachers/photos/hints becomes the file's built-in content —
      // no external storage needed, works fully offline when reopened.
      var pattern = /function defaultTeachers\(\)\{[\s\S]*?\n  \}/;
      var replacement = "function defaultTeachers(){\n    return " + json + ";\n  }";

      if(pattern.test(html)){
        html = html.replace(pattern, replacement);
      } else {
        console.error("Could not locate defaultTeachers() to patch; download aborted.");
        alert("Sorry, something went wrong preparing the download. Please try again.");
        return;
      }

      html = "<!DOCTYPE html>\n" + html;

      var blob = new Blob([html], {type: "text/html"});
      var url = URL.createObjectURL(blob);
      var a = document.createElement("a");
      var stamp = new Date().toISOString().slice(0,10);
      a.href = url;
      a.download = "guess-the-teacher-" + stamp + ".html";
      document.body.appendChild(a);
      a.click();
      document.body.removeChild(a);
      setTimeout(function(){ URL.revokeObjectURL(url); }, 2000);
    }catch(e){
      console.error("Download failed", e);
      alert("Sorry, the download didn't work. Please try again.");
    }
  }

  document.getElementById("reset-btn").addEventListener("click", function(){
    if(confirm("Remove all teachers and start fresh?")){
      teachers = defaultTeachers();
      scheduleSave();
      renderGrid();
    }
  });

  /* ================= AUDIO ================= */
  var audioCtx = null;
  function ctx(){
    if(!audioCtx){
      var AC = window.AudioContext || window.webkitAudioContext;
      audioCtx = new AC();
    }
    if(audioCtx.state === "suspended"){ audioCtx.resume(); }
    return audioCtx;
  }
  function tone(freq, start, dur, type, gain){
    var c = ctx();
    var osc = c.createOscillator();
    var g = c.createGain();
    osc.type = type || "sine";
    osc.frequency.value = freq;
    g.gain.setValueAtTime(0, c.currentTime+start);
    g.gain.linearRampToValueAtTime(gain||0.12, c.currentTime+start+0.01);
    g.gain.exponentialRampToValueAtTime(0.0001, c.currentTime+start+dur);
    osc.connect(g); g.connect(c.destination);
    osc.start(c.currentTime+start);
    osc.stop(c.currentTime+start+dur+0.02);
  }
  function noiseBurst(start, dur, gain, filterFreq){
    var c = ctx();
    var bufSize = Math.max(1, Math.floor(c.sampleRate * dur));
    var buf = c.createBuffer(1, bufSize, c.sampleRate);
    var data = buf.getChannelData(0);
    for(var i=0;i<bufSize;i++){ data[i] = (Math.random()*2-1) * (1 - i/bufSize); }
    var src = c.createBufferSource();
    src.buffer = buf;
    var filt = c.createBiquadFilter();
    filt.type = "highpass";
    filt.frequency.value = filterFreq || 1500;
    var g = c.createGain();
    g.gain.setValueAtTime(0, c.currentTime+start);
    g.gain.linearRampToValueAtTime(gain||0.15, c.currentTime+start+0.005);
    g.gain.exponentialRampToValueAtTime(0.0001, c.currentTime+start+dur);
    src.connect(filt); filt.connect(g); g.connect(c.destination);
    src.start(c.currentTime+start);
  }
  function playTick(urgent, pitchBoost){
    var base = urgent ? 1500 : 950;
    var f = base + (pitchBoost||0);
    tone(f, 0, 0.07, "square", urgent?0.11:0.055);
    tone(f*1.5, 0.005, 0.05, "sine", urgent?0.05:0.02);
    if(urgent){ noiseBurst(0, 0.04, 0.06, 3000); }
  }
  function playHeartbeat(){
    tone(90, 0, 0.09, "sine", 0.22);
    tone(70, 0.12, 0.12, "sine", 0.16);
  }
  function playTimeUp(){
    tone(300,0,0.18,"sawtooth",0.1);
    tone(200,0.15,0.28,"sawtooth",0.12);
    tone(150,0.3,0.4,"sawtooth",0.12);
    noiseBurst(0, 0.3, 0.12, 500);
  }
  function playFanfare(){
    var notes = [523.25, 659.25, 783.99, 1046.5, 1318.5];
    notes.forEach(function(f, i){
      tone(f, i*0.1, 0.4, "triangle", 0.1);
      tone(f*2, i*0.1+0.02, 0.25, "sine", 0.035);
    });
    tone(1046.5, 0.45, 0.6, "triangle", 0.11);
    tone(1318.5, 0.45, 0.6, "sine", 0.06);
  }
  function playDrumroll(){
    for(var i=0;i<10;i++){
      noiseBurst(i*0.11, 0.06, 0.09, 800);
      tone(180+Math.random()*40, i*0.11, 0.05, "triangle", 0.05);
    }
  }
  function playWhoosh(dir){
    var c = ctx();
    var bufSize = Math.floor(c.sampleRate * 0.35);
    var buf = c.createBuffer(1, bufSize, c.sampleRate);
    var data = buf.getChannelData(0);
    for(var i=0;i<bufSize;i++){ data[i] = (Math.random()*2-1); }
    var src = c.createBufferSource();
    src.buffer = buf;
    var filt = c.createBiquadFilter();
    filt.type = "bandpass";
    filt.frequency.setValueAtTime(dir==="back"?2200:400, c.currentTime);
    filt.frequency.exponentialRampToValueAtTime(dir==="back"?400:2200, c.currentTime+0.32);
    filt.Q.value = 0.8;
    var g = c.createGain();
    g.gain.setValueAtTime(0.0001, c.currentTime);
    g.gain.linearRampToValueAtTime(0.09, c.currentTime+0.05);
    g.gain.exponentialRampToValueAtTime(0.0001, c.currentTime+0.35);
    src.connect(filt); filt.connect(g); g.connect(c.destination);
    src.start();
  }
  function playPop(){
    tone(1100, 0, 0.08, "sine", 0.08);
    tone(1500, 0.09, 0.12, "sine", 0.08);
  }
  function playShutter(){
    noiseBurst(0, 0.05, 0.1, 4000);
    tone(2000, 0, 0.03, "square", 0.04);
  }
  function playClick(){
    tone(700, 0, 0.05, "sine", 0.07);
  }

  /* ================= PRESENT MODE ================= */
  var setupScreen = document.getElementById("setup-screen");
  var setupFooter = document.querySelector(".setup-footer");
  var presentScreen = document.getElementById("present-screen");
  var boardFrame = document.getElementById("board-frame");

  var curIdx = 0;
  var curPhase = "photo"; // 'photo' | 'reveal'
  var timeLeft = TOTAL_TIME;
  var timerHandle = null;
  var running = false;

  document.getElementById("start-btn").addEventListener("click", function(){
    if(teachers.length===0) return;
    curIdx = 0; curPhase = "rules";
    enterPresent();
  });
  document.getElementById("exit-btn").addEventListener("click", exitPresent);
  document.getElementById("fullscreen-btn").addEventListener("click", function(){
    if(!document.fullscreenElement){
      document.documentElement.requestFullscreen().catch(function(){});
    } else {
      document.exitFullscreen().catch(function(){});
    }
  });
  document.getElementById("prev-btn").addEventListener("click", function(){ goTo(curIdx-1, "photo"); });
  document.getElementById("next-btn").addEventListener("click", function(){
    if(curPhase==="photo"){ goTo(curIdx, "reveal"); }
    else { goTo(curIdx+1, "photo"); }
  });

  document.addEventListener("keydown", function(e){
    if(presentScreen.classList.contains("hidden")) return;
    if(e.key==="ArrowRight"){ document.getElementById("next-btn").click(); }
    else if(e.key==="ArrowLeft"){ document.getElementById("prev-btn").click(); }
    else if(e.key==="Escape"){ exitPresent(); }
  });

  function enterPresent(){
    setupScreen.classList.add("hidden");
    setupFooter.classList.add("hidden");
    presentScreen.classList.remove("hidden");
    renderDots();
    renderStage();
  }
  function exitPresent(){
    stopTimer();
    presentScreen.classList.add("hidden");
    setupScreen.classList.remove("hidden");
    setupFooter.classList.remove("hidden");
  }

  function goTo(idx, phase){
    if(idx<0 || idx>=teachers.length) return;
    var goingBack = (idx < curIdx) || (idx===curIdx && phase==="photo" && curPhase==="reveal");
    stopTimer();
    curIdx = idx; curPhase = phase; timeLeft = TOTAL_TIME;
    playWhoosh(goingBack ? "back" : "forward");
    renderDots();
    renderStage();
  }

  function renderDots(){
    var dots = document.getElementById("dots");
    dots.innerHTML = "";
    teachers.forEach(function(t, i){
      var d = document.createElement("div");
      d.className = "dot" + (i===curIdx ? " active" : "");
      d.title = t.name || ("Teacher "+(i+1));
      d.addEventListener("click", function(){ goTo(i, "photo"); });
      dots.appendChild(d);
    });
    var isRules = curPhase === "rules";
    dots.classList.toggle("hidden", isRules);
    document.getElementById("prev-btn").classList.toggle("hidden", isRules);
    document.getElementById("next-btn").classList.toggle("hidden", isRules);
    document.getElementById("prev-btn").disabled = (curIdx===0 && curPhase==="photo");
    document.getElementById("next-btn").disabled = false;
  }

  function stopTimer(){
    running = false;
    clearInterval(timerHandle);
    timerHandle = null;
  }

  function renderStage(){
    stopTimer();
    var t = teachers[curIdx] || {name:"", photo:"", hint:""};
    if(curPhase === "rules"){
      boardFrame.innerHTML =
        '<div class="phase" id="phase-rules">'+
          '<p class="prompt">How to play 🎓</p>'+
          '<ul class="rules-list">'+
            '<li><span class="rule-badge">1</span><span>A teacher\'s childhood photo appears on screen.</span></li>'+
            '<li><span class="rule-badge">2</span><span>Students have 30 seconds to shout out their guess.</span></li>'+
            '<li><span class="rule-badge">3</span><span>A hint drops halfway through, at the 15-second mark.</span></li>'+
            '<li><span class="rule-badge">4</span><span>When time runs out (or the host reveals early), the name is unveiled!</span></li>'+
          '</ul>'+
          '<div class="stage-actions">'+
            '<button class="btn btn-primary" id="rules-start-btn">Let\'s start!</button>'+
          '</div>'+
        '</div>';
      document.getElementById("rules-start-btn").addEventListener("click", function(){
        playClick();
        goTo(0, "photo");
      });
      return;
    }
    if(curPhase === "photo"){
      timeLeft = TOTAL_TIME;
      boardFrame.innerHTML =
        '<div class="phase" id="phase-photo">'+
          '<p class="prompt">Who was this teacher as a kid? 🧐</p>'+
          '<div class="photo-frame">'+ (t.photo ? '<img src="'+t.photo+'">' : '<div class="placeholder-icon">'+placeholderIconSVG()+'</div>') +'</div>'+
          '<div class="timer-ring-wrap">'+
            '<svg viewBox="0 0 150 150">'+
              '<circle class="timer-ring-bg" cx="75" cy="75" r="65"></circle>'+
              '<circle class="timer-ring-fg" id="ring-fg" cx="75" cy="75" r="65" stroke-dasharray="408.4" stroke-dashoffset="0"></circle>'+
            '</svg>'+
            '<div class="timer-num" id="timer-num">'+TOTAL_TIME+'</div>'+
          '</div>'+
          '<div class="hint-text" id="hint-text"></div>'+
          '<div class="times-up-banner" id="times-up-banner"></div>'+
          '<div class="stage-actions">'+
            '<button class="btn btn-primary" id="start-timer-btn">Start '+TOTAL_TIME+'-second timer</button>'+
            '<button class="btn btn-ghost" id="reveal-now-btn">Reveal now</button>'+
          '</div>'+
        '</div>';
      document.getElementById("start-timer-btn").addEventListener("click", startCountdown);
      document.getElementById("reveal-now-btn").addEventListener("click", function(){
        stopTimer(); playDrumroll(); goTo(curIdx, "reveal");
      });
    } else {
      var revealAnim = pickRevealTransition();
      boardFrame.innerHTML =
        '<canvas class="confetti-canvas" id="confetti"></canvas>'+
        '<div class="phase '+revealAnim+'" id="phase-reveal">'+
          '<div class="photo-frame">'+ (t.photo ? '<img src="'+t.photo+'">' : '<div class="placeholder-icon">'+placeholderIconSVG()+'</div>') +'</div>'+
          '<div class="reveal-name" id="reveal-name"></div>'+
          '<div class="reveal-sub">Was your guess right?</div>'+
          '<div class="stage-actions">'+
            '<button class="btn btn-primary" id="next-teacher-btn">'+ (curIdx < teachers.length-1 ? "Next teacher" : "Finish") +'</button>'+
          '</div>'+
        '</div>';
      playShutter();
      setLetterName(document.getElementById("reveal-name"), t.name || "Teacher");
      setTimeout(function(){
        playFanfare();
        launchConfetti(document.getElementById("confetti"));
      }, 220);
      document.getElementById("next-teacher-btn").addEventListener("click", function(){
        if(curIdx < teachers.length-1){ goTo(curIdx+1, "photo"); }
        else { showThankYou(); }
      });
    }
  }

  function showThankYou(){
    stopTimer();
    document.getElementById("dots").classList.add("hidden");
    document.getElementById("prev-btn").classList.add("hidden");
    document.getElementById("next-btn").classList.add("hidden");
    var revealAnim = pickRevealTransition();
    boardFrame.innerHTML =
      '<canvas class="confetti-canvas" id="confetti"></canvas>'+
      '<div class="phase '+revealAnim+'" id="phase-thankyou">'+
        '<div class="thankyou-decor" aria-hidden="true">'+
          '<svg class="ty-icon ty-heart-tl" viewBox="0 0 60 60"><path d="M30 14c-6-10-20-8-18 3 1 8 10 15 18 27 8-12 17-19 18-27 2-11-12-13-18-3z"/><path d="M30 14 L32 4"/></svg>'+
          '<svg class="ty-icon ty-star-tr" viewBox="0 0 60 60"><path d="M30 4 L36 22 L55 22 L39 33 L45 52 L30 41 L15 52 L21 33 L5 22 L24 22 Z"/></svg>'+
          '<svg class="ty-icon ty-apple-tr" viewBox="0 0 60 70"><path d="M30 20c-9-9-26-5-26 10 0 15 13 30 26 36 13-6 26-21 26-36 0-15-17-19-26-10z"/><path d="M30 20 L30 6 C30 2 35 0 39 3"/></svg>'+
          '<svg class="ty-icon ty-hearts-r" viewBox="0 0 40 100"><path d="M14 10c-3-5-10-4-9 1 0 4 5 7 9 13 4-6 9-9 9-13 1-5-6-6-9-1z"/><path d="M14 56c-3-5-10-4-9 1 0 4 5 7 9 13 4-6 9-9 9-13 1-5-6-6-9-1z"/></svg>'+
          '<svg class="ty-icon ty-leaf-bl" viewBox="0 0 90 40"><path d="M4 36 C28 18 50 12 86 4"/><path d="M16 29 C20 23 24 19 28 17"/><path d="M30 22 C34 16 38 12 42 10"/><path d="M44 15 C48 9 52 6 56 4"/></svg>'+
          '<svg class="ty-icon ty-leaf-br" viewBox="0 0 90 40"><path d="M4 36 C28 18 50 12 86 4"/><path d="M16 29 C20 23 24 19 28 17"/><path d="M30 22 C34 16 38 12 42 10"/><path d="M44 15 C48 9 52 6 56 4"/></svg>'+
        '</div>'+
        '<div class="ty-emoji">🎉</div>'+
        '<div class="ty-title">Thank you!</div>'+
        '<div class="ty-divider"><span></span><svg class="ty-divider-heart" viewBox="0 0 24 24"><path d="M12 21s-7.5-4.6-10-9.4C.4 8 2.7 4.5 6.3 4.5c2 0 3.6 1 5.7 3.3 2.1-2.3 3.7-3.3 5.7-3.3 3.6 0 5.9 3.5 4.3 7.1C19.5 16.4 12 21 12 21z"/></svg><span></span></div>'+
        '<div class="ty-sub">Thanks for playing<br><span class="ty-highlight">Guess the Teacher</span><br>by their childhood photos.</div>'+
        '<div class="ty-badge">'+
          '<span class="ty-badge-top">Happy</span>'+
          '<span class="ty-badge-main">TEACHERS\' DAY</span>'+
        '</div>'+
        '<div class="stage-actions">'+
          '<button class="btn btn-primary" id="thankyou-done-btn">Back to setup</button>'+
        '</div>'+
      '</div>';
    playFanfare();
    launchConfetti(document.getElementById("confetti"));
    document.getElementById("thankyou-done-btn").addEventListener("click", exitPresent);
  }

  function setLetterName(el, name){
    if(!el) return;
    el.innerHTML = "";
    name.split("").forEach(function(ch, i){
      var span = document.createElement("span");
      span.className = "letter";
      span.style.animationDelay = (i*0.045)+"s";
      span.textContent = ch === " " ? "\u00A0" : ch;
      el.appendChild(span);
    });
  }

  function flashScreen(color){
    var flash = document.getElementById("flash-overlay");
    if(!flash) return;
    flash.style.background = color || "#F6F3EC";
    flash.classList.remove("go");
    void flash.offsetWidth;
    flash.classList.add("go");
  }

  var REVEAL_TRANSITIONS = ["reveal-anim-zoom","reveal-anim-slideup","reveal-anim-spin","reveal-anim-flip","reveal-anim-slideleft","reveal-anim-drop"];
  var FLASH_COLORS = ["#F6F3EC","#E8B339","#E85D4E","#7FA9A0"];
  var lastTransition = null;
  function pickRevealTransition(){
    var pool = REVEAL_TRANSITIONS;
    var choice;
    do{ choice = pool[Math.floor(Math.random()*pool.length)]; } while(choice===lastTransition && pool.length>1);
    lastTransition = choice;
    return choice;
  }

  function startCountdown(){
    if(running) return;
    running = true;
    var startBtn = document.getElementById("start-timer-btn");
    if(startBtn) startBtn.disabled = true;
    updateRing(1);
    playTick(false, 0);
    timerHandle = setInterval(function(){
      timeLeft -= 1;
      var frac = Math.max(0, timeLeft/TOTAL_TIME);
      updateRing(frac);
      var numEl = document.getElementById("timer-num");
      var ringWrap = document.querySelector(".timer-ring-wrap");
      if(numEl){
        numEl.textContent = Math.max(0,timeLeft);
        numEl.classList.remove("tick");
        void numEl.offsetWidth; // restart animation
        numEl.classList.add("tick");
        numEl.classList.toggle("urgent-num", timeLeft<=5);
      }
      if(ringWrap){ ringWrap.classList.toggle("urgent-wrap", timeLeft<=5 && timeLeft>0); }
      var boardEl = document.querySelector(".board-frame");
      if(boardEl){ boardEl.classList.toggle("urgent-glow", timeLeft<=5 && timeLeft>0); }
      if(timeLeft === HINT_AT){ dropHint(); }
      if(timeLeft <= 3 && timeLeft > 0){
        playTick(true, (4-timeLeft)*90);
        playHeartbeat();
      } else if(timeLeft <= 5 && timeLeft > 0){
        playTick(true);
      } else if(timeLeft > 5 && timeLeft % 5 === 0){
        playTick(false);
      } else if(timeLeft > 0){
        tone(700, 0, 0.03, "sine", 0.02); // soft second-tick
      }
      if(timeLeft <= 0){
        stopTimer();
        playTimeUp();
        showTimesUp();
      }
    }, 1000);
  }
  function showTimesUp(){
    var banner = document.getElementById("times-up-banner");
    if(banner){
      banner.textContent = "⏰ Time's up!";
      banner.classList.add("shown");
    }
    var board = document.querySelector(".board-frame");
    if(board){
      board.classList.remove("urgent-glow");
      board.classList.add("shake");
      setTimeout(function(){ board.classList.remove("shake"); }, 500);
    }
    var revealBtn = document.getElementById("reveal-now-btn");
    if(revealBtn){
      revealBtn.textContent = "Reveal the teacher!";
      revealBtn.classList.remove("btn-ghost");
      revealBtn.classList.add("btn-primary", "pulse-btn");
    }
  }
  function dropHint(){
    var t = teachers[curIdx];
    var hintEl = document.getElementById("hint-text");
    if(!hintEl || !t || !t.hint) return;
    hintEl.textContent = "💡 Hint: " + t.hint;
    requestAnimationFrame(function(){ hintEl.classList.add("shown"); });
    playPop();
  }
  function updateRing(frac){
    var ring = document.getElementById("ring-fg");
    if(!ring) return;
    var circumference = 408.4;
    ring.style.strokeDashoffset = (circumference * (1-frac));
    ring.classList.toggle("urgent", frac <= 5/TOTAL_TIME);
  }

  /* ================= CONFETTI ================= */
  function launchConfetti(canvas){
    if(!canvas) return;
    var parent = canvas.parentElement.parentElement; // board-frame
    var w = parent.clientWidth, h = parent.clientHeight;
    var dpr = Math.min(window.devicePixelRatio || 1, 2);
    canvas.width = w*dpr; canvas.height = h*dpr;
    canvas.style.width = w+"px"; canvas.style.height = h+"px";
    var ctx2d = canvas.getContext("2d");
    ctx2d.scale(dpr, dpr);
    var colors = ["#E8B339","#E85D4E","#7FA9A0","#F6F3EC","#F2D98C"];
    var pieces = [];
    var count = 110;
    for(var i=0;i<count;i++){
      pieces.push({
        x: Math.random()*w,
        y: -20 - Math.random()*h*0.6,
        r: 4 + Math.random()*6,
        shape: Math.random() < 0.35 ? "circle" : "rect",
        c: colors[Math.floor(Math.random()*colors.length)],
        vy: 2.2 + Math.random()*3.2,
        vx: -1.8 + Math.random()*3.6,
        rot: Math.random()*360,
        vr: -8 + Math.random()*16,
        wobble: Math.random()*Math.PI*2,
        wobbleSpeed: 0.05 + Math.random()*0.08
      });
    }
    var frames = 0;
    var maxFrames = 190;
    function draw(){
      frames++;
      ctx2d.clearRect(0,0,w,h);
      pieces.forEach(function(p){
        p.wobble += p.wobbleSpeed;
        p.x += p.vx + Math.sin(p.wobble)*0.6;
        p.y += p.vy;
        p.vy += 0.02;
        p.rot += p.vr;
        var fade = frames > maxFrames-40 ? Math.max(0,(maxFrames-frames)/40) : 1;
        ctx2d.save();
        ctx2d.globalAlpha = fade;
        ctx2d.translate(p.x, p.y);
        ctx2d.rotate(p.rot*Math.PI/180);
        ctx2d.fillStyle = p.c;
        if(p.shape === "circle"){
          ctx2d.beginPath();
          ctx2d.arc(0,0,p.r/2,0,Math.PI*2);
          ctx2d.fill();
        } else {
          ctx2d.fillRect(-p.r/2, -p.r/2, p.r, p.r*0.6);
        }
        ctx2d.restore();
      });
      if(frames < maxFrames){ requestAnimationFrame(draw); }
      else { ctx2d.clearRect(0,0,w,h); }
    }
    draw();
  }

  loadTeachers();
})();
</script>
</body>
</html>
