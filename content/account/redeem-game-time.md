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
.wrap{display:flex;justify-content:center;padding:2rem 1rem;min-height:500px}
.panel{width:100%;max-width:480px;background:#f5f0e8;border:1px solid #b8966a;position:relative}
.corner{position:absolute;width:16px;height:16px;border-color:#8a6030;border-style:solid}
.corner-tl{top:5px;left:5px;border-width:2px 0 0 2px}
.corner-tr{top:5px;right:5px;border-width:2px 2px 0 0}
.corner-bl{bottom:5px;left:5px;border-width:0 0 2px 2px}
.corner-br{bottom:5px;right:5px;border-width:0 2px 2px 0}
.header{padding:28px 28px 22px;border-bottom:1px solid #d4b896;text-align:center;background:#ede7d8}
.logo-sigil{width:52px;height:52px;margin:0 auto 14px}
.logo-sigil svg{width:52px;height:52px}
.game-title{font-family:'Cinzel',serif;font-size:10px;letter-spacing:3px;color:#9a7040;text-transform:uppercase;margin-bottom:6px}
.page-title{font-family:'Cinzel',serif;font-size:21px;color:#3a2810;letter-spacing:0.5px;line-height:1.2;margin-bottom:4px}
.page-sub{font-family:'Crimson Text',Georgia,serif;font-style:italic;font-size:15px;color:#7a5a38}
.divider{height:1px;background:linear-gradient(90deg,transparent,#c4a070 20%,#8a6030 50%,#c4a070 80%,transparent);margin:0 24px}
.body{padding:28px}
.field-group{margin-bottom:20px}
.field-label{font-family:'Cinzel',serif;font-size:10px;letter-spacing:2px;color:#7a5a38;text-transform:uppercase;margin-bottom:7px;display:block}
.field-input{width:100%;background:#faf7f2;border:1px solid #c4a878;color:#1e1408;font-family:'Crimson Text',Georgia,serif;font-size:17px;padding:10px 14px;outline:none;transition:border-color 0.2s}
.field-input:focus{border-color:#8a6030;background:#fff}
.field-input::placeholder{color:#b8a080;font-style:italic}
.field-input.code-input{letter-spacing:3px;font-size:16px;text-transform:uppercase;text-align:center}
.btn-redeem{width:100%;background:#2e1e08;border:1px solid #5a3c18;color:#d4a84c;font-family:'Cinzel',serif;font-size:12px;letter-spacing:3px;padding:14px;cursor:pointer;text-transform:uppercase;margin-top:6px;transition:all 0.2s}
.btn-redeem:hover:not(:disabled){background:#3e2c10;border-color:#8a6a2a;color:#e8c870}
.btn-redeem:disabled{opacity:0.4;cursor:default}
.validation-box{margin-top:20px;background:#ede7d8;border:1px solid #d4b896;padding:16px;min-height:90px;display:none}
.v-line{font-family:'Crimson Text',Georgia,serif;font-size:14px;color:#a08060;margin-bottom:7px;display:flex;align-items:center;gap:8px;opacity:0;transition:opacity 0.3s}
.v-line.show{opacity:1}
.v-line.ok{color:#2a6a3a}
.v-line.ok::before{content:'';display:inline-block;width:8px;height:8px;background:#3a8a50;border-radius:50%;flex-shrink:0}
.v-line.pending{color:#7a5a38}
.v-line.pending::before{content:'';display:inline-block;width:8px;height:8px;border:1.5px solid #8a6030;border-radius:50%;border-top-color:transparent;flex-shrink:0;animation:spin 0.8s linear infinite}
@keyframes spin{to{transform:rotate(360deg)}}
.success-panel{display:none;text-align:center;padding:4px 0}
.success-icon{width:54px;height:54px;margin:0 auto 14px}
.success-title{font-family:'Cinzel',serif;font-size:17px;color:#2a4a1e;margin-bottom:10px;letter-spacing:1px}
.success-days{font-family:'Cinzel',serif;font-size:52px;color:#3a2810;line-height:1;margin-bottom:2px;font-weight:700}
.success-days-label{font-family:'Cinzel',serif;font-size:11px;letter-spacing:3px;color:#9a7040;text-transform:uppercase;margin-bottom:16px}
.success-msg{font-family:'Crimson Text',Georgia,serif;font-style:italic;font-size:16px;color:#3a2810;line-height:1.7;margin-bottom:18px}
.success-expiry{font-family:'Crimson Text',Georgia,serif;font-size:14px;color:#7a5a38;border-top:1px solid #d4b896;padding-top:14px}
.success-expiry span{color:#3a2810;font-style:italic}
.fool-note{font-family:'Crimson Text',Georgia,serif;font-style:italic;font-size:13px;color:#a09070;margin-top:12px}
.footer-bar{border-top:1px solid #d4b896;padding:11px 24px;display:flex;justify-content:space-between;align-items:center;background:#ede7d8}
.footer-txt{font-family:'Cinzel',serif;font-size:9px;letter-spacing:2px;color:#9a7040;text-transform:uppercase}
.server-dot{width:6px;height:6px;background:#3a7a3a;border-radius:50%;display:inline-block;margin-right:5px}
</style>
<div class="wrap">
  <div class="panel">
    <div class="corner corner-tl"></div>
    <div class="corner corner-tr"></div>
    <div class="corner corner-bl"></div>
    <div class="corner corner-br"></div>
    <div class="header">
      <div class="logo-sigil">
        <svg viewBox="0 0 54 54" xmlns="http://www.w3.org/2000/svg">
          <polygon points="27,3 33,20 50,20 37,31 42,48 27,37 12,48 17,31 4,20 21,20" fill="none" stroke="#b8966a" stroke-width="1.5"/>
          <polygon points="27,9 31.5,21 44,21 34,28 38,41 27,34 16,41 20,28 10,21 22.5,21" fill="none" stroke="#8a6030" stroke-width="0.8"/>
          <circle cx="27" cy="27" r="5" fill="none" stroke="#b8966a" stroke-width="1"/>
          <circle cx="27" cy="27" r="2.2" fill="#8a6030"/>
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
          <svg viewBox="0 0 54 54" xmlns="http://www.w3.org/2000/svg">
            <circle cx="27" cy="27" r="24" fill="none" stroke="#3a8a50" stroke-width="1.5"/>
            <circle cx="27" cy="27" r="17" fill="none" stroke="#c4e0c8" stroke-width="8"/>
            <polyline points="17,27 24,34 37,20" fill="none" stroke="#2a6a3a" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
        </div>
        <div class="success-title">Redemption Successful</div>
        <div class="success-days">30</div>
        <div class="success-days-label">Days Added</div>
        <div class="success-msg">Welcome back, <span id="successName" style="font-style:normal;font-family:'Cinzel',serif;font-size:14px;color:#8a6030"></span>.<br>Your passage through the Shards has been renewed.</div>
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
  const steps=[{id:'v1',delay:900},{id:'v2',delay:1300},{id:'v3',delay:2000},{id:'v4',delay:1000}];
  for(let i=0;i<steps.length;i++){
    const el=document.getElementById(steps[i].id);
    el.classList.add('show','pending');
    await sleep(steps[i].delay);
    el.classList.remove('pending');
    el.classList.add('ok');
  }
  await sleep(400);
  const expiry=new Date();
  expiry.setDate(expiry.getDate()+30);
  const fmt=expiry.toLocaleDateString('en-GB',{day:'2-digit',month:'long',year:'numeric'});
  document.getElementById('successName').textContent=name;
  document.getElementById('expiryDate').textContent=fmt;
  vbox.style.display='none';
  document.getElementById('successPanel').style.display='block';
  btn.style.display='none';
  document.querySelectorAll('.field-group').forEach(el=>el.style.display='none');
}
</script>
