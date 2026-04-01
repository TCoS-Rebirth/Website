---
title: "Redeem game time card"
date: 2026-04-01T00:00:00
draft: false
headerimage: "arena.jpg"
---

<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@fontsource/cinzel@5.0.8/400.css">
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@fontsource/cinzel@5.0.8/700.css">
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@fontsource/crimson-text@5.0.8/400.css">
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@fontsource/crimson-text@5.0.8/400-italic.css">

<style>
*{box-sizing:border-box;margin:0;padding:0}
.wrap{display:flex;justify-content:center;align-items:flex-start;padding:2rem 1rem;min-height:520px}
.panel{width:100%;max-width:480px;background:#0b0910;border:1px solid #6b4f1e;position:relative;overflow:hidden}
.panel::before{content:'';position:absolute;inset:0;background:repeating-linear-gradient(0deg,transparent,transparent 40px,rgba(255,255,255,0.012) 40px,rgba(255,255,255,0.012) 41px);pointer-events:none}
.corner{position:absolute;width:18px;height:18px;border-color:#c9a84c;border-style:solid}
.corner-tl{top:6px;left:6px;border-width:2px 0 0 2px}
.corner-tr{top:6px;right:6px;border-width:2px 2px 0 0}
.corner-bl{bottom:6px;left:6px;border-width:0 0 2px 2px}
.corner-br{bottom:6px;right:6px;border-width:0 2px 2px 0}
.header{padding:28px 28px 20px;border-bottom:1px solid #2a1e0e;text-align:center}
.logo-sigil{width:54px;height:54px;margin:0 auto 14px;position:relative}
.logo-sigil svg{width:54px;height:54px}
.game-title{font-family:'Cinzel',serif;font-size:11px;letter-spacing:3px;color:#6b4f1e;text-transform:uppercase;margin-bottom:6px}
.page-title{font-family:'Cinzel',serif;font-size:22px;color:#c9a84c;letter-spacing:1px;line-height:1.2;margin-bottom:4px}
.page-sub{font-family:'Crimson Text',Georgia,serif;font-style:italic;font-size:14px;color:#8a7055;letter-spacing:0.5px}
.divider{height:1px;background:linear-gradient(90deg,transparent,#6b4f1e 30%,#c9a84c 50%,#6b4f1e 70%,transparent);margin:0 28px}
.body{padding:28px}
.field-group{margin-bottom:22px}
.field-label{font-family:'Cinzel',serif;font-size:10px;letter-spacing:2px;color:#8a7055;text-transform:uppercase;margin-bottom:8px;display:block}
.field-input{width:100%;background:#070610;border:1px solid #2a1e0e;color:#d4c5a0;font-family:'Crimson Text',Georgia,serif;font-size:17px;padding:10px 14px;outline:none;letter-spacing:0.5px;transition:border-color 0.2s}
.field-input:focus{border-color:#6b4f1e;background:#0a0815}
.field-input::placeholder{color:#3a2e20;font-style:italic}
.field-input.code-input{letter-spacing:3px;font-size:16px;text-transform:uppercase;text-align:center}
.btn-redeem{width:100%;background:linear-gradient(180deg,#2a1c08 0%,#1a1005 100%);border:1px solid #8a6a2a;color:#c9a84c;font-family:'Cinzel',serif;font-size:13px;letter-spacing:3px;padding:14px;cursor:pointer;text-transform:uppercase;margin-top:6px;transition:all 0.2s;position:relative;overflow:hidden}
.btn-redeem:hover:not(:disabled){background:linear-gradient(180deg,#3a2810 0%,#261808 100%);border-color:#c9a84c;color:#e8d48a}
.btn-redeem:disabled{opacity:0.5;cursor:default}
.validation-box{margin-top:20px;background:#070610;border:1px solid #1a1208;padding:16px;min-height:90px;display:none}
.v-line{font-family:'Crimson Text',Georgia,serif;font-size:14px;color:#5a4030;margin-bottom:6px;display:flex;align-items:center;gap:8px;opacity:0;transition:opacity 0.3s}
.v-line.show{opacity:1}
.v-line.ok{color:#4a8a5a}
.v-line.ok::before{content:'';display:inline-block;width:8px;height:8px;background:#4a8a5a;border-radius:50%;flex-shrink:0}
.v-line.pending{color:#8a7055}
.v-line.pending::before{content:'';display:inline-block;width:8px;height:8px;border:1px solid #8a7055;border-radius:50%;border-top-color:transparent;flex-shrink:0;animation:spin 0.8s linear infinite}
@keyframes spin{to{transform:rotate(360deg)}}
.success-panel{display:none;text-align:center;padding:8px 0}
.success-icon{width:56px;height:56px;margin:0 auto 16px}
.success-title{font-family:'Cinzel',serif;font-size:18px;color:#c9a84c;margin-bottom:8px;letter-spacing:1px}
.success-days{font-family:'Cinzel',serif;font-size:48px;color:#e8d48a;line-height:1;margin-bottom:4px}
.success-days-label{font-family:'Crimson Text',Georgia,serif;font-size:15px;color:#8a7055;letter-spacing:2px;text-transform:uppercase;margin-bottom:16px}
.success-msg{font-family:'Crimson Text',Georgia,serif;font-style:italic;font-size:15px;color:#8a7055;line-height:1.6;margin-bottom:20px}
.success-expiry{font-family:'Crimson Text',Georgia,serif;font-size:13px;color:#4a3820;border-top:1px solid #1a1208;padding-top:14px;margin-top:4px}
.success-expiry span{color:#6b5030}
.fool-note{font-family:'Crimson Text',Georgia,serif;font-style:italic;font-size:13px;color:#2a2010;margin-top:14px}
.footer-bar{border-top:1px solid #1a1208;padding:12px 28px;display:flex;justify-content:space-between;align-items:center}
.footer-txt{font-family:'Cinzel',serif;font-size:9px;letter-spacing:2px;color:#2a1e0e;text-transform:uppercase}
.server-dot{width:6px;height:6px;background:#2a5a2a;border-radius:50%;display:inline-block;margin-right:5px}
</style>

<div class="wrap">
  <div class="panel" id="panel">
    <div class="corner corner-tl"></div>
    <div class="corner corner-tr"></div>
    <div class="corner corner-bl"></div>
    <div class="corner corner-br"></div>

    <div class="header">
      <div class="logo-sigil">
        <svg viewBox="0 0 54 54" xmlns="http://www.w3.org/2000/svg">
          <polygon points="27,4 32,20 49,20 36,30 41,47 27,37 13,47 18,30 5,20 22,20" fill="none" stroke="#6b4f1e" stroke-width="1.5"/>
          <polygon points="27,10 31,21 43,21 33,28 37,40 27,33 17,40 21,28 11,21 23,21" fill="none" stroke="#c9a84c" stroke-width="0.8"/>
          <circle cx="27" cy="27" r="5" fill="none" stroke="#8a6a2a" stroke-width="1"/>
          <circle cx="27" cy="27" r="2" fill="#6b4f1e"/>
        </svg>
      </div>
      <div class="game-title">The Chronicles of Spellborn</div>
      <div class="page-title">Game Time Redemption</div>
      <div class="page-sub">Extend your access to the Shards</div>
    </div>

    <div class="divider"></div>

    <div class="body" id="formBody">
      <div class="field-group">
        <label class="field-label" for="accountName">Account Name</label>
        <input class="field-input" type="text" id="accountName" placeholder="Enter your account name" autocomplete="off" spellcheck="false">
      </div>
      <div class="field-group">
        <label class="field-label" for="gameCode">Game Time Code</label>
        <input class="field-input code-input" type="text" id="gameCode" placeholder="XXXXX-XXXXX-XXXXX" autocomplete="off" spellcheck="false" maxlength="17">
      </div>

      <button class="btn-redeem" id="redeemBtn" onclick="startValidation()">Redeem Game Time</button>

      <div class="validation-box" id="validationBox">
        <div class="v-line" id="v1">Establishing connection to Enclave servers...</div>
        <div class="v-line" id="v2">Authenticating account credentials...</div>
        <div class="v-line" id="v3">Verifying game time code...</div>
        <div class="v-line" id="v4">Processing subscription extension...</div>
      </div>

      <div class="success-panel" id="successPanel">
        <div class="success-icon">
          <svg viewBox="0 0 56 56" xmlns="http://www.w3.org/2000/svg">
            <circle cx="28" cy="28" r="25" fill="none" stroke="#4a8a5a" stroke-width="1.5"/>
            <circle cx="28" cy="28" r="18" fill="none" stroke="#2a5a3a" stroke-width="0.8"/>
            <polyline points="18,28 25,35 38,21" fill="none" stroke="#4a9e5a" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
        </div>
        <div class="success-title">Redemption Successful</div>
        <div class="success-days">30</div>
        <div class="success-days-label">Days Added</div>
        <div class="success-msg" id="successMsg">Welcome back, <span id="successName" style="color:#c9a84c;font-style:normal;font-family:'Cinzel',serif;font-size:13px"></span>.<br>Your passage through the Shards has been renewed.</div>
        <div class="success-expiry">New subscription expiry: <span id="expiryDate"></span></div>
        <div class="fool-note">Happy April Fools' Day — from the Spellborn Reborn team.</div>
      </div>
    </div>

    <div class="footer-bar">
      <div class="footer-txt"><span class="server-dot"></span>Shard servers online</div>
      <div class="footer-txt">spellborn.org</div>
    </div>
  </div>
</div>

<script>
const codeInput = document.getElementById('gameCode');
codeInput.addEventListener('input', function(e) {
  let v = e.target.value.replace(/[^a-zA-Z0-9]/g,'').toUpperCase();
  let out = '';
  for(let i=0;i<v.length&&i<15;i++){
    if(i===5||i===10) out+='-';
    out+=v[i];
  }
  e.target.value=out;
});

function sleep(ms){return new Promise(r=>setTimeout(r,ms))}

async function startValidation(){
  const name = document.getElementById('accountName').value.trim();
  const code = document.getElementById('gameCode').value.trim();
  if(!name){document.getElementById('accountName').focus();return;}
  if(code.replace(/-/g,'').length<15){document.getElementById('gameCode').focus();return;}

  const btn = document.getElementById('redeemBtn');
  btn.disabled=true;
  const vbox = document.getElementById('validationBox');
  vbox.style.display='block';

  const steps = [
    {id:'v1', delay:800},
    {id:'v2', delay:1400},
    {id:'v3', delay:2200},
    {id:'v4', delay:1000},
  ];

  for(let i=0;i<steps.length;i++){
    const el=document.getElementById(steps[i].id);
    el.classList.add('show','pending');
    await sleep(steps[i].delay);
    el.classList.remove('pending');
    el.classList.add('ok');
  }

  await sleep(400);

  const expiry = new Date();
  expiry.setDate(expiry.getDate()+30);
  const fmt = expiry.toLocaleDateString('en-GB',{day:'2-digit',month:'long',year:'numeric'});

  document.getElementById('successName').textContent=name;
  document.getElementById('expiryDate').textContent=fmt;

  vbox.style.display='none';
  document.getElementById('successPanel').style.display='block';
  btn.style.display='none';
  document.querySelectorAll('.field-group').forEach(el=>el.style.display='none');
}
</script>
