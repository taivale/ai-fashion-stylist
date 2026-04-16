<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width,initial-scale=1.0,viewport-fit=cover"/>
<meta name="theme-color" content="#2A1F1B"/>
<meta name="apple-mobile-web-app-capable" content="yes"/>
<meta name="apple-mobile-web-app-status-bar-style" content="black-translucent"/>
<meta name="apple-mobile-web-app-title" content="Stylist IA"/>
<title>AI Fashion Stylist</title>
<link rel="preconnect" href="https://fonts.googleapis.com"/>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,600;0,700;1,400&family=DM+Sans:wght@300;400;500;600&display=swap" rel="stylesheet"/>
<style>
*{box-sizing:border-box;margin:0;padding:0;-webkit-tap-highlight-color:transparent}
html,body{height:100%;overflow:hidden}
body{font-family:'DM Sans',-apple-system,sans-serif;background:#F7F4F0;color:#1A1410;-webkit-font-smoothing:antialiased}
:root{
  --bg:#F7F4F0;--sf:#FFF;--alt:#EFE9E2;
  --tx:#1A1410;--txs:#7A6A5E;--txm:#B0A49A;
  --ac:#B8825A;--acd:#96623A;--acl:#F2E6D8;
  --bd:#E2D5C8;--ok:#5A9870;--err:#C04040;
  --night:#2A1F1B;
  --serif:'Playfair Display',Georgia,serif;
  --sans:'DM Sans',-apple-system,sans-serif;
}
@keyframes spin{to{transform:rotate(360deg)}}
@keyframes up{from{opacity:0;transform:translateY(14px)}to{opacity:1;transform:translateY(0)}}
@keyframes in{from{opacity:0}to{opacity:1}}
@keyframes su{from{opacity:0;transform:translateY(100%)}to{opacity:1;transform:translateY(0)}}
@keyframes pulse{0%,100%{opacity:1}50%{opacity:.4}}
::-webkit-scrollbar{width:0;height:3px}
::-webkit-scrollbar-thumb{background:var(--bd);border-radius:4px}
#app{max-width:430px;margin:0 auto;height:100vh;height:100dvh;display:flex;flex-direction:column;overflow:hidden;background:var(--bg)}
#hdr{background:linear-gradient(160deg,var(--night) 0%,#3A2818 60%,var(--ac) 100%);padding:16px 18px 14px;padding-top:calc(16px + env(safe-area-inset-top,0px));flex-shrink:0;z-index:50}
#main{flex:1;overflow-y:auto;overflow-x:hidden;-webkit-overflow-scrolling:touch}
#nav{background:var(--sf);border-top:1px solid var(--bd);display:flex;flex-shrink:0;padding-bottom:calc(6px + env(safe-area-inset-bottom,0px));z-index:50}
.nb{flex:1;display:flex;flex-direction:column;align-items:center;gap:3px;padding:10px 2px 6px;background:none;border:none;color:var(--txm);font-size:9px;font-weight:400;cursor:pointer;transition:color .2s;font-family:var(--sans)}
.nb.on{color:var(--ac)}
.scr{padding:14px 14px 80px;animation:up .4s ease}
.card{background:var(--sf);border-radius:14px;box-shadow:0 2px 10px rgba(26,20,16,.05)}
.cp{padding:16px}
.btn{width:100%;padding:15px;border-radius:50px;border:none;background:linear-gradient(135deg,var(--ac),var(--acd));color:#FFF;font-size:14px;font-weight:700;font-family:var(--sans);cursor:pointer;letter-spacing:.3px;box-shadow:0 5px 18px rgba(184,130,90,.4)}
.btn:disabled{background:var(--bd);color:var(--txm);box-shadow:none;cursor:not-allowed}
.btn2{width:100%;padding:13px;border-radius:50px;border:1.5px solid var(--ac);background:none;color:var(--ac);font-size:14px;font-weight:600;font-family:var(--sans);cursor:pointer}
.chip{padding:7px 13px;border-radius:20px;border:1.5px solid var(--bd);background:var(--sf);color:var(--txs);font-size:12px;font-family:var(--sans);cursor:pointer;white-space:nowrap;transition:all .15s}
.chip.on{background:var(--ac);color:#FFF;border-color:var(--ac);font-weight:600}
.tag{font-size:10px;padding:2px 7px;background:var(--alt);border-radius:20px;color:var(--txs)}
.sp{border:3px solid var(--bd);border-top-color:var(--ac);border-radius:50%;animation:spin .85s linear infinite;flex-shrink:0}
.mo{position:fixed;inset:0;background:rgba(26,20,16,.55);backdrop-filter:blur(4px);display:flex;flex-direction:column;justify-content:flex-end;z-index:200}
.ms{background:var(--sf);border-radius:22px 22px 0 0;max-height:94vh;overflow-y:auto;-webkit-overflow-scrolling:touch;animation:su .32s cubic-bezier(.32,.72,0,1)}
.mh{width:36px;height:4px;border-radius:2px;background:var(--bd);margin:14px auto 0}
.fl{font-size:11px;font-weight:700;text-transform:uppercase;letter-spacing:.8px;color:var(--txs);display:block;margin-bottom:8px}
</style>
</head>
<body>
<div id="app">
  <div id="hdr">
    <div style="display:flex;align-items:center;justify-content:space-between">
      <div style="display:flex;align-items:center;gap:8px">
        <span style="color:var(--ac);font-size:17px">&#10022;</span>
        <span id="htitle" style="font-family:var(--serif);font-size:20px;font-weight:700;color:#FFF">Meu Closet</span>
      </div>
      <div style="display:flex;gap:8px;align-items:center">
        <span id="hbadge"></span>
        <button id="hadd" onclick="openUpload()" style="width:36px;height:36px;border-radius:50%;background:var(--ac);color:#FFF;border:none;font-size:22px;display:flex;align-items:center;justify-content:center;cursor:pointer;box-shadow:0 3px 12px rgba(184,130,90,.5)">+</button>
      </div>
    </div>
  </div>
  <main id="main"></main>
  <nav id="nav">
    <button class="nb on" id="n0" onclick="goTab(0)">
      <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round"><rect x="3" y="3" width="18" height="18" rx="2"/><line x1="12" y1="3" x2="12" y2="21"/></svg>
      Closet
    </button>
    <button class="nb" id="n1" onclick="goTab(1)">
      <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round"><path d="M12 2l2.9 6.3L22 9.3l-5 4.9 1.2 6.9L12 17.8l-6.2 3.3L7 14.2 2 9.3l7.1-1L12 2z"/></svg>
      Stylist
    </button>
    <button class="nb" id="n2" onclick="goTab(2)">
      <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round"><path d="M20.84 4.61a5.5 5.5 0 0 0-7.78 0L12 5.67l-1.06-1.06a5.5 5.5 0 0 0-7.78 7.78l1.06 1.06L12 21.23l7.78-7.78 1.06-1.06a5.5 5.5 0 0 0 0-7.78z"/></svg>
      Looks
    </button>
    <button class="nb" id="n3" onclick="goTab(3)">
      <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round"><rect x="2" y="7" width="20" height="14" rx="2"/><path d="M16 7V5a2 2 0 0 0-2-2h-4a2 2 0 0 0-2 2v2"/></svg>
      Mala
    </button>
    <button class="nb" id="n4" onclick="goTab(4)">
      <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="10"/><circle cx="12" cy="12" r="4"/></svg>
      Cores
    </button>
  </nav>
</div>
<div id="umo" class="mo" style="display:none" onclick="if(event.target===this&&S.uStep==='capture')closeU()">
  <div class="ms"><div class="mh"></div><div id="uco"></div></div>
</div>
<script>
// ═══════════════════════════════════════════════════
// TAXONOMIA COMPLETA DE PEÇAS
// ═══════════════════════════════════════════════════
const TAX = {
  'Blusa':{'cat':'Parte de Cima','role':'TOP','emoji':'👚'},
  'Camiseta':{'cat':'Parte de Cima','role':'TOP','emoji':'👕'},
  'Regata':{'cat':'Parte de Cima','role':'TOP','emoji':'🎽'},
  'Cropped':{'cat':'Parte de Cima','role':'TOP','emoji':'👚'},
  'Camisa':{'cat':'Parte de Cima','role':'TOP','emoji':'👔'},
  'Top':{'cat':'Parte de Cima','role':'TOP','emoji':'👙'},
  'Body':{'cat':'Parte de Cima','role':'TOP','emoji':'🩱'},
  'Manga longa':{'cat':'Parte de Cima','role':'TOP','emoji':'👕'},
  'Gola alta':{'cat':'Parte de Cima','role':'TOP','emoji':'👕'},
  'Um ombro':{'cat':'Parte de Cima','role':'TOP','emoji':'👚'},
  'Calça':{'cat':'Parte de Baixo','role':'BOT','emoji':'👖'},
  'Calça jeans':{'cat':'Parte de Baixo','role':'BOT','emoji':'👖'},
  'Pantacourt':{'cat':'Parte de Baixo','role':'BOT','emoji':'👖'},
  'Culotte':{'cat':'Parte de Baixo','role':'BOT','emoji':'👖'},
  'Saia curta':{'cat':'Parte de Baixo','role':'BOT','emoji':'🩱'},
  'Saia midi':{'cat':'Parte de Baixo','role':'BOT','emoji':'🩱'},
  'Saia longa':{'cat':'Parte de Baixo','role':'BOT','emoji':'🩱'},
  'Saia mini':{'cat':'Parte de Baixo','role':'BOT','emoji':'🩱'},
  'Saia de couro':{'cat':'Parte de Baixo','role':'BOT','emoji':'🩱'},
  'Short':{'cat':'Parte de Baixo','role':'BOT','emoji':'🩲'},
  'Bermuda':{'cat':'Parte de Baixo','role':'BOT','emoji':'🩲'},
  'Legging':{'cat':'Parte de Baixo','role':'BOT','emoji':'🩲'},
  'Vestido curto':{'cat':'Peça Inteira','role':'FULL','emoji':'👗'},
  'Vestido midi':{'cat':'Peça Inteira','role':'FULL','emoji':'👗'},
  'Vestido longo':{'cat':'Peça Inteira','role':'FULL','emoji':'👗'},
  'Macacão':{'cat':'Peça Inteira','role':'FULL','emoji':'🦺'},
  'Macaquinho':{'cat':'Peça Inteira','role':'FULL','emoji':'🦺'},
  'Conjunto':{'cat':'Peça Inteira','role':'FULL','emoji':'👗'},
  'Blazer':{'cat':'Terceira Peça','role':'LAYER','emoji':'🧥'},
  'Cardigan':{'cat':'Terceira Peça','role':'LAYER','emoji':'🧥'},
  'Casaco':{'cat':'Terceira Peça','role':'LAYER','emoji':'🧥'},
  'Trench coat':{'cat':'Terceira Peça','role':'LAYER','emoji':'🧥'},
  'Jaqueta jeans':{'cat':'Terceira Peça','role':'LAYER','emoji':'🧥'},
  'Jaqueta couro':{'cat':'Terceira Peça','role':'LAYER','emoji':'🧥'},
  'Kimono':{'cat':'Terceira Peça','role':'LAYER','emoji':'🥻'},
  'Sobretudo':{'cat':'Terceira Peça','role':'LAYER','emoji':'🧥'},
  'Colete':{'cat':'Terceira Peça','role':'LAYER','emoji':'🦺'},
  'Tenis':{'cat':'Calcado','role':'SHOE','emoji':'👟'},
  'Sandalia rasteira':{'cat':'Calcado','role':'SHOE','emoji':'🩴'},
  'Sandalia salto':{'cat':'Calcado','role':'SHOE','emoji':'👠'},
  'Sandalia plataforma':{'cat':'Calcado','role':'SHOE','emoji':'👠'},
  'Scarpin':{'cat':'Calcado','role':'SHOE','emoji':'👠'},
  'Sapatilha':{'cat':'Calcado','role':'SHOE','emoji':'🥿'},
  'Bota cano curto':{'cat':'Calcado','role':'SHOE','emoji':'👢'},
  'Bota cano longo':{'cat':'Calcado','role':'SHOE','emoji':'👢'},
  'Ankle boot':{'cat':'Calcado','role':'SHOE','emoji':'👢'},
  'Mule':{'cat':'Calcado','role':'SHOE','emoji':'🥿'},
  'Mocassim':{'cat':'Calcado','role':'SHOE','emoji':'🥿'},
  'Bolsa tote':{'cat':'Acessorio','role':'ACC','emoji':'👜'},
  'Bolsa clutch':{'cat':'Acessorio','role':'ACC','emoji':'👛'},
  'Bolsa crossbody':{'cat':'Acessorio','role':'ACC','emoji':'👜'},
  'Mochila':{'cat':'Acessorio','role':'ACC','emoji':'🎒'},
  'Cinto':{'cat':'Acessorio','role':'ACC','emoji':'🪡'},
  'Colar':{'cat':'Acessorio','role':'ACC','emoji':'📿'},
  'Brinco':{'cat':'Acessorio','role':'ACC','emoji':'💎'},
  'Pulseira':{'cat':'Acessorio','role':'ACC','emoji':'📿'},
  'Oculos de sol':{'cat':'Acessorio','role':'ACC','emoji':'🕶'},
  'Chapeu':{'cat':'Acessorio','role':'ACC','emoji':'🎩'},
  'Bone':{'cat':'Acessorio','role':'ACC','emoji':'🧢'},
  'Echarpe':{'cat':'Acessorio','role':'ACC','emoji':'🧣'},
  'Cachecol':{'cat':'Acessorio','role':'ACC','emoji':'🧣'},
  'Meia-calca':{'cat':'Sem Foto','role':'NOIMG','emoji':'🧦'},
  'Meia':{'cat':'Sem Foto','role':'NOIMG','emoji':'🧦'},
  'Segunda pele':{'cat':'Sem Foto','role':'NOIMG','emoji':'👙'},
  'Luvas':{'cat':'Sem Foto','role':'NOIMG','emoji':'🧤'},
  'Camisola':{'cat':'Sem Foto','role':'NOIMG','emoji':'🌙'},
  'Pijama':{'cat':'Sem Foto','role':'NOIMG','emoji':'😴'},
  'Maio':{'cat':'Moda Praia','role':'BEACH','emoji':'🩱'},
  'Biquini':{'cat':'Moda Praia','role':'BEACH','emoji':'👙'},
  'Canga':{'cat':'Moda Praia','role':'BEACH','emoji':'🏖'},
  'Saida de praia':{'cat':'Moda Praia','role':'BEACH','emoji':'🏖'},
};

const TIPOS = Object.keys(TAX);
const CORES = ['Preto','Branco','Off-white','Bege','Caramelo','Marrom','Cinza','Azul-marinho','Azul-claro','Jeans claro','Jeans escuro','Verde-escuro','Verde-oliva','Verde-menta','Vermelho','Bordo','Rosa','Rosa-claro','Lilas','Roxo','Amarelo','Mostarda','Laranja','Coral','Terracota','Dourado','Prateado'];
const ESTAMPAS = ['Liso','Listrado','Poa','Floral','Animal print','Xadrez','Tie-dye','Geometrico','Tweed','Etnico','Abstrato'];
const ESTILOS = ['Casual','Elegante','Classico','Moderno','Romantico','Esportivo','Minimalista','Sofisticado','Casual elegante','Boho','Streetwear'];
const OCASIOES = ['Trabalho','Casual dia a dia','Jantar','Festa','Praia/Piscina','Viagem','Evento formal','Happy hour','Reuniao','Final de semana','Academia','Passeio'];
const CLIMAS = ['Quente','Ameno','Frio','Chuva'];
const CI = {Quente:'☀️',Ameno:'🌤',Frio:'🧊',Chuva:'🌧'};

// ═══════════════════════════════════════════════════
// REGRAS DE MONTAGEM DE LOOKS
// ═══════════════════════════════════════════════════
// Fórmula A: TOP + BOT [+ LAYER] + SHOE [+ ACC]
// Fórmula B: FULL [+ LAYER] + SHOE [+ ACC]
// Nunca 2 TOP, 2 BOT, 2 FULL, 2 SHOE no mesmo look

function buildValidLooks(garments) {
  const byR = {TOP:[],BOT:[],FULL:[],LAYER:[],SHOE:[],ACC:[]};
  for (const g of garments) {
    const r = TAX[g.tipo]?.role;
    if (r && byR[r]) byR[r].push(g);
  }
  const sh = a => [...a].sort(() => Math.random()-.5);
  const [tops,bots,fulls,layers,shoes,accs] = ['TOP','BOT','FULL','LAYER','SHOE','ACC'].map(k=>sh(byR[k]));
  const looks = [];

  // Formula A
  for (let i=0; i<Math.min(2,tops.length) && looks.length<2; i++) {
    if (!bots.length) break;
    const p = [tops[i], bots[i%bots.length]];
    if (layers.length) p.push(layers[i%layers.length]);
    if (shoes.length) p.push(shoes[i%shoes.length]);
    if (accs.length) p.push(accs[i%accs.length]);
    looks.push({formula:'A',pieces:p});
  }

  // Formula B
  for (let i=0; i<fulls.length && looks.length<3; i++) {
    const p = [fulls[i]];
    if (layers.length) p.push(layers[i%layers.length]);
    if (shoes.length) p.push(shoes[i%shoes.length]);
    if (accs.length) p.push(accs[i%accs.length]);
    looks.push({formula:'B',pieces:p});
  }

  // More Formula A if needed
  if (tops.length && bots.length && looks.length < 3) {
    const t = tops[looks.length%tops.length], b = bots[looks.length%bots.length];
    const p = [t,b];
    if (layers.length>1) p.push(layers[1]);
    if (shoes.length) p.push(shoes[looks.length%shoes.length]);
    if (accs.length>1) p.push(accs[1]);
    looks.push({formula:'A',pieces:p});
  }

  // Fallback
  if (!looks.length) {
    const s2=sh(garments);
    for(let i=0;i<Math.min(3,Math.ceil(garments.length/2));i++)
      looks.push({formula:'fallback',pieces:s2.slice(i*2,i*2+3).filter(Boolean)});
  }

  return looks.slice(0,3);
}

// ═══════════════════════════════════════════════════
// ESTADO
// ═══════════════════════════════════════════════════
let S = {
  tab:0, garments:[], favLooks:[],
  uStep:'capture', uFile:null, uUrl:null, uCls:null,
  stPhase:'input', stOc:'', stCl:'', stLooks:[], stIdx:0,
  malaPhase:'form', malaTrip:{destino:'',dias:'',clima:'',estilo:''}, malaPack:null,
  cTab:'paleta', cGrupo:'Todos', cSel:null, cHarm:'colorBlocking', bCores:[], builderMsg:'',
  wFilt:'', delId:null,
};
try{S.garments=JSON.parse(localStorage.getItem('fs_g')||'[]')}catch{}
try{S.favLooks=JSON.parse(localStorage.getItem('fs_fav')||'[]')}catch{}
function save(){localStorage.setItem('fs_g',JSON.stringify(S.garments));localStorage.setItem('fs_fav',JSON.stringify(S.favLooks))}

const $=id=>document.getElementById(id);
const uid=()=>Date.now().toString(36)+Math.random().toString(36).slice(2,5);
const delay=ms=>new Promise(r=>setTimeout(r,ms));
const chips=(items,sel,fn,multi=false)=>items.map(v=>`<button class="chip ${(multi?sel.includes(v):sel===v)?'on':''}" onclick="${fn}(this.dataset.v)" data-v="${v.replace(/"/g,'&quot;')}">${v}</button>`).join('');

// ═══════════════════════════════════════════════════
// NAVEGAÇÃO
// ═══════════════════════════════════════════════════
const TITLES=['Meu Closet','Stylist IA','Looks Salvos','Mala Inteligente','Módulo de Cores'];
function goTab(t){
  S.tab=t;
  document.querySelectorAll('.nb').forEach((b,i)=>b.classList.toggle('on',i===t));
  $('htitle').textContent=TITLES[t];
  $('hadd').style.display=t===0?'flex':'none';
  $('hbadge').innerHTML=t===0?`<span style="font-size:10px;color:rgba(255,255,255,.4)">${S.garments.length} peças</span>`:t===2?`<span style="font-size:10px;color:rgba(255,255,255,.4)">${S.favLooks.length} looks</span>`:'';
  render();
}
function render(){
  const f=[rCloset,rStylist,rFavs,rMala,rCores];
  $('main').innerHTML=(f[S.tab]||rCloset)();
}

// ═══════════════════════════════════════════════════
// CLOSET
// ═══════════════════════════════════════════════════
function rCloset(){
  const g=S.garments;
  if(!g.length) return `<div class="scr" style="display:flex;flex-direction:column;align-items:center;text-align:center;padding:60px 20px">
    <div style="width:80px;height:80px;border-radius:50%;background:var(--acl);display:flex;align-items:center;justify-content:center;font-size:40px;margin-bottom:18px">👗</div>
    <h3 style="font-family:var(--serif);font-size:22px;font-weight:700;margin-bottom:8px">Closet vazio</h3>
    <p style="font-size:14px;color:var(--txs);line-height:1.6;max-width:240px;margin-bottom:24px">Adicione peças pelo <strong>+</strong> acima ou fotografe suas roupas</p>
    </div>`;

  const cats=[...new Set(g.map(x=>TAX[x.tipo]?.cat||'Outros'))];
  const filt=S.wFilt;
  const list=filt?g.filter(x=>(TAX[x.tipo]?.cat||'Outros')===filt||x.tipo===filt):g;
  const cnt=r=>g.filter(x=>TAX[x.tipo]?.role===r).length;

  return `<div class="scr">
    <div style="display:flex;gap:7px;margin-bottom:14px;overflow-x:auto;padding-bottom:4px">
      ${[['👗',g.length,'total'],['👚',cnt('TOP'),'cima'],['👖',cnt('BOT'),'baixo'],['👗',cnt('FULL'),'inteira'],['🧥',cnt('LAYER'),'camada'],['👟',cnt('SHOE'),'calçado'],['👜',cnt('ACC'),'acessório']].map(([e,n,l])=>
        `<div style="flex-shrink:0;background:var(--sf);border-radius:10px;padding:9px 10px;text-align:center;min-width:52px">
          <span style="font-size:14px;display:block">${e}</span>
          <span style="font-family:var(--serif);font-size:17px;font-weight:700;color:var(--ac);display:block">${n}</span>
          <span style="font-size:9px;color:var(--txs)">${l}</span>
        </div>`).join('')}
    </div>
    <div style="display:flex;gap:6px;overflow-x:auto;margin-bottom:14px;padding-bottom:4px">
      <button class="chip ${!filt?'on':''}" onclick="S.wFilt='';render()">Tudo</button>
      ${cats.map(c=>`<button class="chip ${filt===c?'on':''}" onclick="S.wFilt='${c}';render()" style="flex-shrink:0">${c}</button>`).join('')}
    </div>
    <div style="display:grid;grid-template-columns:repeat(2,1fr);gap:10px">
      ${list.map((g,i)=>{
        const tx=TAX[g.tipo]||{emoji:'👗'};
        return `<div class="card" style="overflow:hidden;animation:up .3s ease ${i*40}ms both;cursor:pointer" onclick="S.delId=S.delId==='${g.id}'?null:'${g.id}';render()">
          <div style="aspect-ratio:3/4;background:var(--alt);position:relative;overflow:hidden;display:flex;align-items:center;justify-content:center">
            ${g.imageUrl?`<img src="${g.imageUrl}" style="width:100%;height:100%;object-fit:cover;display:block" onerror="this.style.display='none'">`:''}
            <div style="position:absolute;inset:0;display:${g.imageUrl?'none':'flex'};align-items:center;justify-content:center;flex-direction:column;gap:4px">
              <span style="font-size:36px">${tx.emoji}</span>
              <span style="font-size:10px;color:var(--txm)">${g.tipo}</span>
            </div>
            ${g.estampa&&g.estampa!=='Liso'?`<div style="position:absolute;top:6px;left:6px;padding:3px 8px;background:rgba(26,20,16,.6);border-radius:20px;font-size:9px;color:#FFF">${g.estampa}</div>`:''}
            ${S.delId===g.id?`<div style="position:absolute;inset:0;background:rgba(26,20,16,.65);display:flex;align-items:center;justify-content:center;animation:in .15s ease">
              <button onclick="rmG('${g.id}');event.stopPropagation()" style="padding:10px 20px;border-radius:50px;background:var(--err);color:#FFF;border:none;font-size:13px;font-weight:700;font-family:var(--sans);cursor:pointer">🗑 Remover</button>
            </div>`:''}
          </div>
          <div style="padding:9px 11px 11px">
            <span style="font-size:12px;font-weight:700;display:block;margin-bottom:4px">${g.tipo}</span>
            <div style="display:flex;gap:4px;flex-wrap:wrap"><span class="tag">${g.cor}</span><span class="tag">${tx.cat||''}</span></div>
          </div>
        </div>`;
      }).join('')}
    </div>
  </div>`;
}
function rmG(id){S.garments=S.garments.filter(g=>g.id!==id);S.delId=null;save();render();goTab(0)}

// ═══════════════════════════════════════════════════
// UPLOAD
// ═══════════════════════════════════════════════════
function openUpload(){S.uStep='capture';S.uFile=null;S.uUrl=null;S.uCls=null;renderU();$('umo').style.display='flex'}
function closeU(){$('umo').style.display='none'}

const DEMOS=[
  {url:'https://images.unsplash.com/photo-1594938298603-c8148c4dae35?w=300&h=380&fit=crop',label:'Vestido'},
  {url:'https://images.unsplash.com/photo-1558171813-4c088753af8f?w=300&h=380&fit=crop',label:'Casaco'},
  {url:'https://images.unsplash.com/photo-1551488831-00ddcb6c6bd3?w=300&h=380&fit=crop',label:'Camisa'},
  {url:'https://images.unsplash.com/photo-1583743814966-8936f5b7be1a?w=300&h=380&fit=crop',label:'Calca'},
  {url:'https://images.unsplash.com/photo-1562157873-818bc0726f68?w=300&h=380&fit=crop',label:'Saia'},
  {url:'https://images.unsplash.com/photo-1596755094514-f87e34085b2c?w=300&h=380&fit=crop',label:'Blusa'},
];

function renderU(){
  const step=S.uStep;
  let h='';
  if(step==='capture'){
    h=`<div style="padding:18px 18px 36px">
      <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:18px">
        <h3 style="font-family:var(--serif);font-size:22px;font-weight:700">Nova Peça</h3>
        <button onclick="closeU()" style="background:none;border:none;color:var(--txs);font-size:26px;line-height:1;cursor:pointer">×</button>
      </div>
      <div style="display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:18px">
        <label style="display:flex;flex-direction:column;align-items:center;gap:8px;padding:20px 12px;border:2px dashed var(--bd);border-radius:14px;cursor:pointer;text-align:center" for="fi-cam">
          <span style="font-size:32px">📷</span>
          <span style="font-size:13px;font-weight:600;color:var(--tx)">Câmera</span>
          <span style="font-size:11px;color:var(--txm)">Tirar foto agora</span>
          <input id="fi-cam" type="file" accept="image/*" capture="environment" style="display:none" onchange="handleFile(event)">
        </label>
        <label style="display:flex;flex-direction:column;align-items:center;gap:8px;padding:20px 12px;border:2px dashed var(--bd);border-radius:14px;cursor:pointer;text-align:center" for="fi-gal">
          <span style="font-size:32px">🖼</span>
          <span style="font-size:13px;font-weight:600;color:var(--tx)">Galeria</span>
          <span style="font-size:11px;color:var(--txm)">Escolher foto</span>
          <input id="fi-gal" type="file" accept="image/*" style="display:none" onchange="handleFile(event)">
        </label>
      </div>
      <p style="font-size:11px;color:var(--txm);text-align:center;margin-bottom:10px">ou use uma imagem de exemplo:</p>
      <div style="display:flex;gap:7px;overflow-x:auto;padding-bottom:4px">
        ${DEMOS.map(d=>`<div onclick="useDemo('${d.url}')" style="flex-shrink:0;text-align:center;cursor:pointer">
          <div style="width:60px;height:75px;border-radius:10px;overflow:hidden;border:2px solid var(--bd)"><img src="${d.url}" style="width:100%;height:100%;object-fit:cover"></div>
          <span style="font-size:9px;color:var(--txs);display:block;margin-top:3px">${d.label}</span>
        </div>`).join('')}
      </div>
    </div>`;
  } else if(step==='processing'){
    h=`<div style="padding:60px 20px;display:flex;flex-direction:column;align-items:center;gap:14px">
      ${S.uUrl?`<img src="${S.uUrl}" style="width:90px;height:114px;object-fit:cover;border-radius:12px;opacity:.75">`:''}
      <div class="sp" style="width:40px;height:40px"></div>
      <p style="font-family:var(--serif);font-size:20px;font-weight:700">Analisando a peça...</p>
      <div style="display:flex;gap:6px;flex-wrap:wrap;justify-content:center">
        ${['tipo','cor','estampa','estilo','ocasião'].map((l,i)=>`<span style="font-size:11px;padding:4px 10px;background:var(--alt);border-radius:20px;color:var(--txs);animation:pulse 1.2s ease ${i*.3}s infinite">${l}</span>`).join('')}
      </div>
    </div>`;
  } else if(step==='review'&&S.uCls){
    const c=S.uCls;
    const tiposHTML=TIPOS.map(v=>{const tx=TAX[v];return`<button class="chip ${c.tipo===v?'on':''}" style="display:flex;align-items:center;gap:4px" onclick="S.uCls.tipo=this.dataset.v;renderU()" data-v="${v.replace(/"/g,'&quot;')}">${tx?.emoji||''} ${v}</button>`;}).join('');
    h=`<div style="padding:16px 16px 40px">
      <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:14px">
        <h3 style="font-family:var(--serif);font-size:20px;font-weight:700">Confirmar Peça</h3>
        <button onclick="closeU()" style="background:none;border:none;color:var(--txs);font-size:24px;line-height:1;cursor:pointer">×</button>
      </div>
      <div style="display:flex;gap:12px;align-items:flex-start;margin-bottom:16px">
        <div style="width:84px;height:108px;border-radius:12px;overflow:hidden;background:var(--alt);flex-shrink:0;display:flex;align-items:center;justify-content:center">
          ${S.uUrl?`<img src="${S.uUrl}" style="width:100%;height:100%;object-fit:cover">`:`<span style="font-size:32px">${TAX[c.tipo]?.emoji||'👗'}</span>`}
        </div>
        <div>
          <div style="display:inline-flex;align-items:center;gap:5px;padding:5px 12px;border-radius:20px;background:${c.confianca==='alta'?'rgba(90,152,112,.15)':'var(--acl)'};margin-bottom:8px">
            <span style="font-size:12px;font-weight:700;color:${c.confianca==='alta'?'var(--ok)':'var(--ac)'}">${c.confianca==='alta'?'✓ Alta precisão':'⚠ Verifique os campos'}</span>
          </div>
          <p style="font-size:12px;color:var(--txs);line-height:1.5">Toque para corrigir qualquer campo.</p>
        </div>
      </div>
      <span class="fl">Tipo da peça</span>
      <div style="display:flex;flex-wrap:wrap;gap:5px;margin-bottom:14px">${tiposHTML}</div>
      <span class="fl">Cor principal</span>
      <div style="display:flex;flex-wrap:wrap;gap:5px;margin-bottom:14px">${CORES.map(v=>`<button class="chip ${c.cor===v?'on':''}" onclick="S.uCls.cor=this.dataset.v;renderU()" data-v="${v}">${v}</button>`).join('')}</div>
      <span class="fl">Estampa / Textura</span>
      <div style="display:flex;flex-wrap:wrap;gap:5px;margin-bottom:14px">${ESTAMPAS.map(v=>`<button class="chip ${(c.estampa||'Liso')===v?'on':''}" onclick="S.uCls.estampa=this.dataset.v;renderU()" data-v="${v}">${v}</button>`).join('')}</div>
      <span class="fl">Estilo</span>
      <div style="display:flex;flex-wrap:wrap;gap:5px;margin-bottom:14px">${ESTILOS.map(v=>`<button class="chip ${c.estilo===v?'on':''}" onclick="S.uCls.estilo=this.dataset.v;renderU()" data-v="${v}">${v}</button>`).join('')}</div>
      <span class="fl">Ocasiões (várias)</span>
      <div style="display:flex;flex-wrap:wrap;gap:5px;margin-bottom:20px">${OCASIOES.map(v=>`<button class="chip ${c.ocasioes.includes(v)?'on':''}" onclick="togOc(this.dataset.v)" data-v="${v}">${v}</button>`).join('')}</div>
      <button class="btn" onclick="saveG()">✓ Salvar no Closet</button>
    </div>`;
  }
  $('uco').innerHTML=h;
}

function togOc(v){if(!S.uCls)return;const oc=S.uCls.ocasioes;S.uCls.ocasioes=oc.includes(v)?oc.filter(o=>o!==v):[...oc,v];renderU()}
async function handleFile(e){const f=e.target.files?.[0];if(!f)return;S.uFile=f;S.uUrl=URL.createObjectURL(f);await classify()}
async function useDemo(url){S.uUrl=url;S.uFile={name:'demo.jpg',type:'image/jpeg'};await classify()}
async function classify(){
  S.uStep='processing';renderU();await delay(1600);
  const tops=Object.keys(TAX).filter(k=>['TOP','BOT','FULL'].includes(TAX[k].role));
  const tipo=tops[Math.floor(Math.random()*tops.length)];
  S.uCls={tipo,cor:CORES[Math.floor(Math.random()*8)],estampa:'Liso',estilo:ESTILOS[Math.floor(Math.random()*ESTILOS.length)],ocasioes:[OCASIOES[0],OCASIOES[1]],confianca:'alta'};
  S.uStep='review';renderU();
}
function saveG(){
  if(!S.uCls)return;
  S.garments.unshift({id:uid(),imageUrl:S.uUrl,...S.uCls,createdAt:new Date().toISOString()});
  save();closeU();goTab(0);
}

// ═══════════════════════════════════════════════════
// STYLIST
// ═══════════════════════════════════════════════════
function rStylist(){
  const g=S.garments;
  const hasTop=g.some(x=>TAX[x.tipo]?.role==='TOP');
  const hasBot=g.some(x=>['BOT','FULL'].includes(TAX[x.tipo]?.role));
  if(!hasTop||!hasBot) return `<div class="scr" style="text-align:center;padding:60px 20px">
    <div style="font-size:48px;margin-bottom:14px">✨</div>
    <h3 style="font-family:var(--serif);font-size:22px;margin-bottom:8px">Adicione mais peças</h3>
    <p style="font-size:14px;color:var(--txs);line-height:1.6;max-width:250px;margin:0 auto">Preciso de pelo menos uma parte de cima e uma parte de baixo (ou vestido).</p>
    <div style="margin-top:12px;font-size:12px;color:var(--txm)">
      Tops: ${g.filter(x=>TAX[x.tipo]?.role==='TOP').length} |
      Baixo: ${g.filter(x=>TAX[x.tipo]?.role==='BOT').length} |
      Inteiras: ${g.filter(x=>TAX[x.tipo]?.role==='FULL').length}
    </div>
  </div>`;

  if(S.stPhase==='loading') return `<div class="scr" style="display:flex;flex-direction:column;align-items:center;padding:60px 20px;gap:14px">
    <div class="sp" style="width:44px;height:44px"></div>
    <p style="font-family:var(--serif);font-size:22px;font-weight:700">Montando seus looks</p>
    <p style="font-size:13px;color:var(--txs)">Aplicando regras de composição...</p>
    <div style="display:flex;flex-wrap:wrap;gap:7px;justify-content:center">
      ${['proporção','paleta coesa','regras de moda','ocasião','clima'].map((t,i)=>`<span style="font-size:11px;padding:4px 11px;background:var(--alt);border-radius:20px;color:var(--txs);animation:pulse 1.4s ease ${i*.3}s infinite">${t}</span>`).join('')}
    </div>
  </div>`;

  if(S.stPhase==='result') return rStylistResult();

  return `<div class="scr"><div class="card cp" style="margin-bottom:12px">
    <p style="font-size:15px;font-weight:500;margin-bottom:18px;display:flex;align-items:center;gap:8px"><span style="color:var(--ac)">✦</span> Para onde você vai?</p>
    <span class="fl">Ocasião</span>
    <div style="display:flex;flex-wrap:wrap;gap:6px;margin-bottom:18px">${OCASIOES.map(v=>`<button class="chip ${S.stOc===v?'on':''}" onclick="S.stOc=this.dataset.v;render()" data-v="${v}">${v}</button>`).join('')}</div>
    <span class="fl">Clima</span>
    <div style="display:flex;gap:8px;margin-bottom:20px">
      ${CLIMAS.map(c=>`<button onclick="S.stCl=this.dataset.v;render()" data-v="${c}" style="flex:1;padding:12px 4px;border-radius:12px;border:1.5px solid ${S.stCl===c?'var(--ac)':'var(--bd)'};background:${S.stCl===c?'var(--acl)':'var(--sf)'};color:${S.stCl===c?'var(--acd)':'var(--txs)'};font-size:11px;font-weight:${S.stCl===c?700:400};cursor:pointer;display:flex;flex-direction:column;align-items:center;gap:5px;font-family:var(--sans);transition:all .15s"><span style="font-size:20px">${CI[c]}</span>${c}</button>`).join('')}
    </div>
    <button class="btn" ${!S.stOc||!S.stCl?'disabled':''} onclick="gerarLooks()">✦ Gerar 3 Looks</button>
  </div></div>`;
}

async function gerarLooks(){
  S.stPhase='loading';render();await delay(1800);
  const raw=buildValidLooks(S.garments);
  const exps=[
    `Composição equilibrada para ${S.stOc.toLowerCase()}. Proporção e paleta trabalhadas — cada peça tem seu papel. Look que parece fácil mas tem muito pensamento por trás.`,
    `O segredo aqui é a camada: a terceira peça estrutura sem pesar. Ideal para clima ${S.stCl.toLowerCase()} — você adapta conforme o dia.`,
    `Look de intenção clara. As peças dialogam em estilo e criam uma silhueta que transmite confiança para ${S.stOc.toLowerCase()}.`,
  ];
  const dicas=['Um cinto fino definiria a silhueta e daria personalidade ao conjunto.','Brincos médios em dourado elevam sem esforço.','Uma bolsa estruturada completaria com sofisticação discreta.'];
  const humores=['Clássico','Casual elegante','Moderno'];
  S.stLooks=raw.map((l,i)=>({...l,humor:humores[i]||'Elegante',explicacao:exps[i]||exps[0],dica:dicas[i]||dicas[0],ocasiao:S.stOc,clima:S.stCl,savedAt:new Date().toISOString()}));
  S.stIdx=0;S.stPhase='result';render();
}

function rStylistResult(){
  const looks=S.stLooks, look=looks[S.stIdx];
  if(!look)return '';
  const MB={'Clássico':'#F0EDE8','Casual elegante':'var(--acl)','Moderno':'#E8EEF0','Elegante':'#EBE8F0'};
  const MT={'Clássico':'#6B5E4E','Casual elegante':'var(--acd)','Moderno':'#3D5A6B','Elegante':'#5E4E6B'};
  const isFav=S.favLooks.some(f=>JSON.stringify(f.pieces?.map(p=>p.id))===JSON.stringify(look.pieces?.map(p=>p.id)));
  return `<div class="scr">
    <div style="display:flex;gap:3px;background:var(--sf);border-radius:14px;padding:4px;margin-bottom:12px;box-shadow:0 2px 8px rgba(26,20,16,.05)">
      ${looks.map((l,i)=>`<button onclick="S.stIdx=${i};render()" style="flex:1;padding:10px 4px;border:none;border-radius:10px;background:${S.stIdx===i?'var(--ac)':'transparent'};color:${S.stIdx===i?'#FFF':'var(--txm)'};font-size:13px;font-weight:${S.stIdx===i?700:400};cursor:pointer;font-family:var(--sans);transition:all .2s">Look ${i+1}</button>`).join('')}
    </div>
    <div class="card" style="overflow:hidden;animation:up .3s ease">
      <div style="display:flex;justify-content:space-between;align-items:center;padding:16px 18px 0">
        <span style="padding:5px 14px;border-radius:20px;font-size:11px;font-weight:700;background:${MB[look.humor]||'var(--alt)'};color:${MT[look.humor]||'var(--txs)'}">${look.humor}</span>
        <button onclick="toggleFav(${S.stIdx})" style="width:38px;height:38px;border-radius:50%;border:1.5px solid ${isFav?'#E8A0A0':'var(--bd)'};background:${isFav?'#FDE8E8':'var(--alt)'};color:${isFav?'#C85C5C':'var(--txm)'};font-size:18px;cursor:pointer;display:flex;align-items:center;justify-content:center;transition:all .2s">${isFav?'♥':'♡'}</button>
      </div>
      <div style="display:flex;gap:10px;padding:14px 18px;overflow-x:auto">
        ${(look.pieces||[]).map(p=>{const tx=TAX[p.tipo]||{emoji:'👗',cat:''};return`<div style="flex-shrink:0;text-align:center">
          <div style="width:80px;height:100px;border-radius:11px;overflow:hidden;background:var(--alt);border:1px solid var(--bd);margin-bottom:6px;display:flex;align-items:center;justify-content:center;position:relative">
            ${p.imageUrl?`<img src="${p.imageUrl}" style="width:100%;height:100%;object-fit:cover;display:block" onerror="this.style.display='none'">`:`<span style="font-size:28px">${tx.emoji}</span>`}
            <div style="position:absolute;bottom:3px;right:3px;font-size:8px;padding:2px 5px;background:rgba(26,20,16,.5);border-radius:8px;color:#FFF">${tx.cat?.split(' ')[0]||''}</div>
          </div>
          <span style="display:block;font-size:11px;font-weight:700;color:var(--tx)">${p.tipo}</span>
          <span style="display:block;font-size:10px;color:var(--txs)">${p.cor}</span>
        </div>`;}).join('')}
      </div>
      <div style="margin:0 18px 12px;padding:13px 15px;background:var(--bg);border-radius:11px;border:1px solid var(--bd)">
        <p style="font-size:14px;line-height:1.7;color:var(--tx);font-family:var(--serif);font-style:italic">${look.explicacao}</p>
      </div>
      <div style="margin:0 18px 18px;padding:12px 14px;background:var(--acl);border-radius:11px;display:flex;gap:10px">
        <span style="font-size:17px;flex-shrink:0">💡</span>
        <div>
          <p style="font-size:10px;font-weight:700;color:var(--acd);text-transform:uppercase;letter-spacing:.8px;margin-bottom:3px">Dica da Stylist</p>
          <p style="font-size:13px;color:var(--acd);line-height:1.5">${look.dica}</p>
        </div>
      </div>
    </div>
    <div style="display:flex;gap:10px;margin-top:12px">
      <button class="btn2" style="flex:1" onclick="S.stPhase='input';S.stOc='';S.stCl='';render()">← Nova consulta</button>
      <button class="btn" style="flex:1" onclick="gerarLooks()">↺ Refazer</button>
    </div>
  </div>`;
}

function toggleFav(idx){
  const look=S.stLooks[idx];if(!look)return;
  const key=JSON.stringify(look.pieces?.map(p=>p.id));
  const i=S.favLooks.findIndex(f=>JSON.stringify(f.pieces?.map(p=>p.id))===key);
  if(i>=0)S.favLooks.splice(i,1);else S.favLooks.unshift({...look,id:uid()});
  save();render();goTab(S.tab);
}

// ═══════════════════════════════════════════════════
// LOOKS SALVOS
// ═══════════════════════════════════════════════════
function rFavs(){
  if(!S.favLooks.length) return `<div class="scr" style="text-align:center;padding:60px 20px">
    <div style="font-size:48px;margin-bottom:14px">♡</div>
    <h3 style="font-family:var(--serif);font-size:22px;margin-bottom:8px">Nenhum look salvo</h3>
    <p style="font-size:14px;color:var(--txs);line-height:1.6;max-width:240px;margin:0 auto 20px">Toque no ♡ nos looks da Stylist para salvar aqui</p>
    <button class="btn" style="width:auto;padding:13px 24px;font-size:14px" onclick="goTab(1)">✦ Ir para Stylist</button>
  </div>`;
  return `<div class="scr">
    <p style="font-size:13px;color:var(--txs);margin-bottom:14px">${S.favLooks.length} look${S.favLooks.length!==1?'s':''} salvo${S.favLooks.length!==1?'s':''}. Toque ♥ para remover.</p>
    ${S.favLooks.map((look,i)=>{
      const MB={'Clássico':'#F0EDE8','Casual elegante':'var(--acl)','Moderno':'#E8EEF0','Elegante':'#EBE8F0'};
      const MT={'Clássico':'#6B5E4E','Casual elegante':'var(--acd)','Moderno':'#3D5A6B','Elegante':'#5E4E6B'};
      return`<div class="card" style="overflow:hidden;margin-bottom:12px;animation:up .3s ease ${i*60}ms both">
        <div style="display:flex;justify-content:space-between;align-items:center;padding:14px 16px 0">
          <div>
            <span style="padding:4px 12px;border-radius:20px;font-size:10px;font-weight:700;background:${MB[look.humor]||'var(--alt)'};color:${MT[look.humor]||'var(--txs)'}">${look.humor||'Look'}</span>
            ${look.ocasiao?`<span style="font-size:10px;color:var(--txm);margin-left:6px">${look.ocasiao} · ${look.clima||''}</span>`:''}
          </div>
          <button onclick="S.favLooks=S.favLooks.filter(f=>f.id!=='${look.id}');save();render()" style="background:none;border:none;color:#C85C5C;font-size:20px;cursor:pointer">♥</button>
        </div>
        <div style="display:flex;gap:8px;padding:12px 16px;overflow-x:auto">
          ${(look.pieces||[]).map(p=>`<div style="flex-shrink:0;text-align:center">
            <div style="width:70px;height:88px;border-radius:10px;overflow:hidden;background:var(--alt);border:1px solid var(--bd);margin-bottom:5px;display:flex;align-items:center;justify-content:center">
              ${p.imageUrl?`<img src="${p.imageUrl}" style="width:100%;height:100%;object-fit:cover" onerror="this.style.display='none'">`:`<span style="font-size:24px">${TAX[p.tipo]?.emoji||'👗'}</span>`}
            </div>
            <span style="display:block;font-size:10px;font-weight:600;color:var(--tx)">${p.tipo}</span>
          </div>`).join('')}
        </div>
        <div style="padding:0 16px 14px"><p style="font-size:12px;color:var(--txs);line-height:1.5;font-style:italic;font-family:var(--serif)">${look.explicacao||''}</p></div>
      </div>`;
    }).join('')}
  </div>`;
}

// ═══════════════════════════════════════════════════
// MALA INTELIGENTE
// ═══════════════════════════════════════════════════
function rMala(){
  if(S.malaPhase==='loading') return `<div class="scr" style="display:flex;flex-direction:column;align-items:center;padding:60px 20px;gap:14px">
    <div style="font-size:40px">🧳</div><div class="sp" style="width:40px;height:40px"></div>
    <p style="font-family:var(--serif);font-size:20px;font-weight:700">Montando sua mala</p>
    <p style="font-size:13px;color:var(--txs)">Otimizando ${S.garments.length} peças para ${S.malaTrip.dias} dias...</p>
  </div>`;
  if(S.malaPhase==='result'&&S.malaPack) return rMalaResult();
  const t=S.malaTrip;
  return `<div class="scr">
    <div style="background:linear-gradient(145deg,var(--night),#5C3020);border-radius:18px;padding:26px 20px 20px;margin-bottom:12px;position:relative;overflow:hidden">
      <div style="position:absolute;top:-40px;right:-40px;width:130px;height:130px;border-radius:50%;border:1px solid rgba(184,130,90,.2)"></div>
      <p style="font-size:10px;letter-spacing:2px;text-transform:uppercase;color:rgba(255,255,255,.35);margin-bottom:8px">Destino</p>
      <input value="${t.destino}" oninput="S.malaTrip.destino=this.value" placeholder="Europa, Paris, Japão..." style="width:100%;background:none;border:none;outline:none;font-family:var(--serif);font-size:24px;font-weight:700;color:#FFF"/>
    </div>
    <div class="card cp" style="margin-bottom:10px">
      <span class="fl">Duração</span>
      <div style="display:flex;gap:8px;align-items:center">
        <input type="number" min="1" max="90" value="${t.dias}" oninput="S.malaTrip.dias=this.value" placeholder="19" style="width:72px;padding:10px;border:1.5px solid var(--bd);border-radius:10px;font-size:22px;font-weight:700;color:var(--ac);font-family:var(--serif);outline:none;text-align:center"/>
        <span style="font-size:14px;color:var(--txs)">dias</span>
        ${t.dias?`<span style="margin-left:auto;font-size:11px;color:var(--ac);padding:4px 10px;background:var(--acl);border-radius:20px">~${Math.ceil(Number(t.dias)/3)} peças base</span>`:''}
      </div>
    </div>
    <div class="card cp" style="margin-bottom:10px">
      <span class="fl">Clima esperado</span>
      <div style="display:flex;gap:6px">
        ${[...CLIMAS,'Variável'].map(c=>`<button onclick="S.malaTrip.clima=this.dataset.v;render()" data-v="${c}" style="flex:1;padding:10px 3px;border-radius:11px;border:1.5px solid ${t.clima===c?'var(--ac)':'var(--bd)'};background:${t.clima===c?'var(--acl)':'var(--sf)'};color:${t.clima===c?'var(--acd)':'var(--txs)'};font-size:10px;font-weight:${t.clima===c?700:400};cursor:pointer;display:flex;flex-direction:column;align-items:center;gap:4px;font-family:var(--sans)"><span style="font-size:17px">${CI[c]||'🌦'}</span>${c}</button>`).join('')}
      </div>
    </div>
    <div class="card cp" style="margin-bottom:16px">
      <span class="fl">Seu estilo</span>
      <div style="display:flex;flex-wrap:wrap;gap:6px">
        ${['Clássico','Casual elegante','Moderno','Minimalista','Sofisticado'].map(e=>`<button class="chip ${t.estilo===e?'on':''}" onclick="S.malaTrip.estilo=this.dataset.v;render()" data-v="${e}">${e}</button>`).join('')}
      </div>
    </div>
    <button class="btn" ${!t.destino||!t.dias||!t.clima?'disabled':''} onclick="gerarMala()">🧳 Montar Mala para ${t.destino||'o destino'}</button>
    ${S.garments.length<3?`<p style="font-size:12px;color:var(--txm);text-align:center;margin-top:10px">Adicione peças ao closet primeiro (${S.garments.length}/3 mínimo)</p>`:''}
  </div>`;
}

async function gerarMala(){
  if(!S.malaTrip.destino||!S.malaTrip.dias||!S.malaTrip.clima)return;
  S.malaPhase='loading';render();await delay(2000);
  const dias=Number(S.malaTrip.dias);
  const NEUTROS=['Preto','Branco','Off-white','Bege','Caramelo','Cinza'];
  const scored=[...S.garments].map(g=>({...g,_s:(g.ocasioes?.length||0)*3+(NEUTROS.some(n=>g.cor?.includes(n))?4:0)+(TAX[g.tipo]?.role==='LAYER'?-1:1)})).sort((a,b)=>b._s-a._s);
  const sel=scored.slice(0,Math.min(Math.ceil(dias/3)+3,scored.length));
  const vLooks=buildValidLooks(sel);
  const ocs=['Passeio','Jantar','Transporte','Noite'];
  const ds=[`Para explorar ${S.malaTrip.destino} com estilo e conforto.`,`Para restaurantes — estrutura sem exagero.`,`Conforto no aeroporto/trem com estilo.`,`Look com intenção para as noites em ${S.malaTrip.destino}.`];
  S.malaPack={
    resumo:`${sel.length} peças para ${dias} dias em ${S.malaTrip.destino}. Paleta coesa, combinações maximizadas.`,
    pecas:sel,
    looks:ocs.map((oc,i)=>({...vLooks[i%vLooks.length],ocasiao:oc,descricao:ds[i]})),
    dicas:[`Em ${S.malaTrip.destino}, carregue sempre uma terceira peça — temperaturas mudam ao longo do dia.`,'Paleta neutra: peças que combinam entre si.','Uma bolsa de dia vira clutch à noite com o conteúdo reduzido.'],
  };
  S.malaPhase='result';render();
}

function rMalaResult(){
  const p=S.malaPack,t=S.malaTrip;
  const OC={'Passeio':{icon:'🗺',bg:'#EAF0EA',tx:'#4B6B4E'},'Jantar':{icon:'🍷',bg:'#F5EAEA',tx:'#8B4A4A'},'Transporte':{icon:'✈️',bg:'#EAF0F5',tx:'#4A6B8B'},'Noite':{icon:'🌙',bg:'#EEEAF5',tx:'#4A4A6B'}};
  return `<div class="scr">
    <div style="background:var(--night);padding:18px 18px 16px;border-radius:16px;margin-bottom:12px">
      <p style="font-size:10px;color:rgba(255,255,255,.35);letter-spacing:1.5px;text-transform:uppercase;margin-bottom:6px">${t.destino} · ${t.dias} dias · ${t.clima}</p>
      <p style="font-family:var(--serif);font-size:15px;font-style:italic;color:rgba(255,255,255,.8);line-height:1.5">${p.resumo}</p>
    </div>
    <div style="display:flex;gap:8px;margin-bottom:12px">
      ${[[p.pecas.length,'peças','🧳'],[p.looks.length,'ocasiões','✨'],[t.dias,'dias','🗓']].map(([n,l,e])=>`<div style="flex:1;background:var(--sf);border-radius:12px;padding:13px 8px;text-align:center"><span style="font-size:19px;display:block;margin-bottom:2px">${e}</span><span style="font-family:var(--serif);font-size:22px;font-weight:700;color:var(--ac);display:block">${n}</span><span style="font-size:9px;color:var(--txs)">${l}</span></div>`).join('')}
    </div>
    <p style="font-size:11px;font-weight:700;text-transform:uppercase;letter-spacing:.8px;color:var(--txs);margin-bottom:9px">Peças selecionadas</p>
    <div style="display:grid;grid-template-columns:repeat(3,1fr);gap:7px;margin-bottom:12px">
      ${p.pecas.map((g,i)=>`<div class="card" style="overflow:hidden;animation:up .3s ease ${i*25}ms both">
        <div style="aspect-ratio:3/4;background:var(--alt);display:flex;align-items:center;justify-content:center;overflow:hidden">
          ${g.imageUrl?`<img src="${g.imageUrl}" style="width:100%;height:100%;object-fit:cover" onerror="this.style.display='none'">`:`<span style="font-size:26px">${TAX[g.tipo]?.emoji||'👗'}</span>`}
        </div>
        <div style="padding:7px 8px 8px"><p style="font-size:10px;font-weight:700;color:var(--tx)">${g.tipo}</p><p style="font-size:9px;color:var(--txs)">${g.cor}</p></div>
      </div>`).join('')}
    </div>
    <p style="font-size:11px;font-weight:700;text-transform:uppercase;letter-spacing:.8px;color:var(--txs);margin-bottom:9px">Looks por ocasião</p>
    ${p.looks.map((look,i)=>{const cfg=OC[look.ocasiao]||{icon:'👗',bg:'var(--alt)',tx:'var(--txs)'};return`<div class="card" style="overflow:hidden;margin-bottom:10px;animation:up .3s ease ${i*80}ms both">
      <div style="padding:12px 14px 10px;border-bottom:1px solid var(--bd);display:flex;align-items:center;gap:9px">
        <span style="width:32px;height:32px;border-radius:50%;background:${cfg.bg};display:flex;align-items:center;justify-content:center;font-size:15px;flex-shrink:0">${cfg.icon}</span>
        <p style="font-size:11px;font-weight:700;color:${cfg.tx};text-transform:uppercase;letter-spacing:.8px">${look.ocasiao}</p>
      </div>
      <div style="display:flex;gap:7px;padding:11px 13px;overflow-x:auto">
        ${(look.pieces||[]).map(pp=>`<div style="flex-shrink:0;text-align:center">
          <div style="width:62px;height:78px;border-radius:9px;overflow:hidden;background:var(--alt);border:1px solid var(--bd);margin-bottom:4px;display:flex;align-items:center;justify-content:center">
            ${pp.imageUrl?`<img src="${pp.imageUrl}" style="width:100%;height:100%;object-fit:cover" onerror="this.style.display='none'">`:`<span style="font-size:22px">${TAX[pp.tipo]?.emoji||'👗'}</span>`}
          </div>
          <span style="font-size:9px;font-weight:600;color:var(--tx)">${pp.tipo}</span>
        </div>`).join('')}
      </div>
      <div style="padding:0 13px 13px"><p style="font-size:12px;color:var(--txs);line-height:1.5;font-style:italic;font-family:var(--serif)">${look.descricao}</p></div>
    </div>`;}).join('')}
    <div class="card cp" style="background:var(--acl);margin-bottom:12px">
      <p style="font-size:11px;font-weight:700;text-transform:uppercase;letter-spacing:.8px;color:var(--acd);margin-bottom:9px">💡 Dicas para ${t.destino}</p>
      ${p.dicas.map(d=>`<p style="font-size:13px;color:var(--acd);line-height:1.5;margin-bottom:7px">• ${d}</p>`).join('')}
    </div>
    <button class="btn2" onclick="S.malaPhase='form';S.malaPack=null;render()">← Planejar outra viagem</button>
  </div>`;
}

// ═══════════════════════════════════════════════════
// MÓDULO DE CORES
// ═══════════════════════════════════════════════════
const PANTONE=[
  {id:'p01',nome:'Tickled Pink',hex:'#F4A7B0',grupo:'Rosa'},
  {id:'p02',nome:'Amethyst Orchid',hex:'#9B7BB8',grupo:'Roxo'},
  {id:'p03',nome:'Caramel',hex:'#B8783A',grupo:'Terroso'},
  {id:'p04',nome:'Dutch Canal',hex:'#8FA8C8',grupo:'Azul'},
  {id:'p05',nome:'Shale Green',hex:'#7A8C6A',grupo:'Verde'},
  {id:'p06',nome:'Burnished Lilac',hex:'#C4A8B8',grupo:'Rosa'},
  {id:'p07',nome:'Teaberry',hex:'#C84060',grupo:'Vermelho'},
  {id:'p08',nome:'Pale Banana',hex:'#F0E080',grupo:'Amarelo'},
  {id:'p09',nome:'Mandarin Orange',hex:'#E87840',grupo:'Laranja'},
  {id:'p10',nome:'Amaranth',hex:'#7A2848',grupo:'Vinho'},
  {id:'p11',nome:'Palm',hex:'#A8B840',grupo:'Verde'},
  {id:'p12',nome:'Evening Blue',hex:'#2A3050',grupo:'Azul'},
  {id:'p13',nome:'Choc.Truffle',hex:'#5A2830',grupo:'Marrom'},
  {id:'p14',nome:'Ether',hex:'#A8C4C8',grupo:'Azul'},
  {id:'p15',nome:'White Onyx',hex:'#E8E4DC',grupo:'Neutro'},
  {id:'p16',nome:'Angora',hex:'#D8C8B0',grupo:'Neutro'},
  {id:'p17',nome:'Ultra Violet',hex:'#702082',grupo:'Roxo'},
  {id:'p18',nome:'Green Olive',hex:'#6B7040',grupo:'Verde'},
  {id:'p19',nome:'Mocha Mousse',hex:'#A07850',grupo:'Terroso'},
  {id:'p20',nome:'Butter Yellow',hex:'#FCE8A8',grupo:'Amarelo'},
  {id:'p21',nome:'Celadon',hex:'#A8C8B0',grupo:'Verde'},
  {id:'p22',nome:'Leather Brown',hex:'#8B4820',grupo:'Marrom'},
  {id:'p23',nome:'All Aboard',hex:'#5080B8',grupo:'Azul'},
  {id:'p24',nome:'Nantucket',hex:'#A0C0D8',grupo:'Azul'},
  {id:'p25',nome:'Pink Marsh.',hex:'#F8D0D8',grupo:'Rosa'},
  {id:'p26',nome:'Choc.Dark',hex:'#4F2C1D',grupo:'Marrom'},
  {id:'p27',nome:'Blood Red',hex:'#7A1820',grupo:'Vermelho'},
  {id:'p28',nome:'Ultimate Gray',hex:'#939597',grupo:'Neutro'},
  {id:'p29',nome:'Neon Navy',hex:'#1A2050',grupo:'Azul'},
];
const HD={
  colorBlocking:{label:'Color Blocking',icon:'▦',desc:'Tendência SS 2026',grupos:[['Teaberry','Dutch Canal','Pale Banana'],['Amethyst Orchid','Palm','Mandarin Orange'],['Tickled Pink','Evening Blue','Pale Banana'],['Ultra Violet','Butter Yellow','All Aboard'],['Blood Red','Celadon','Butter Yellow']]},
  analogas:{label:'Análogas',icon:'〰',desc:'Vizinhas — harmônicas',grupos:[['Tickled Pink','Burnished Lilac','Amethyst Orchid'],['Dutch Canal','Ether','Nantucket'],['Caramel','Mocha Mousse','Angora'],['Palm','Shale Green','Green Olive']]},
  complementares:{label:'Compl.',icon:'⊕',desc:'Opostos — contraste',grupos:[['Teaberry','Shale Green'],['Amethyst Orchid','Pale Banana'],['Mandarin Orange','Dutch Canal'],['Ultra Violet','Butter Yellow']]},
  monocromatico:{label:'Mono.',icon:'◧',desc:'Tons da mesma família',grupos:[['Pink Marsh.','Tickled Pink','Burnished Lilac'],['Butter Yellow','Pale Banana','Angora'],['Ether','Dutch Canal','All Aboard','Evening Blue'],['Angora','White Onyx','Mocha Mousse']]},
  neutroDestaque:{label:'Neutro+Cor',icon:'◉',desc:'Base neutra + destaque',grupos:[['White Onyx','Angora','Teaberry'],['Ultimate Gray','Evening Blue','Tickled Pink'],['Choc.Truffle','White Onyx','Dutch Canal'],['Angora','Mocha Mousse','Amethyst Orchid']]},
};
const isLt=hex=>{const r=parseInt(hex.slice(1,3),16),g=parseInt(hex.slice(3,5),16),b=parseInt(hex.slice(5,7),16);return(r*299+g*587+b*114)/1000>155};
const tT=hex=>isLt(hex)?'rgba(0,0,0,.75)':'rgba(255,255,255,.9)';

function rCores(){
  return `<div style="animation:up .4s ease">
    <div style="display:flex;gap:2px;background:var(--sf);border-bottom:1px solid var(--bd);position:sticky;top:0;z-index:10">
      ${[['paleta','🎨 Paleta'],['harmonias','⊕ Harmonias'],['builder','▦ Builder']].map(([id,l])=>`<button onclick="S.cTab='${id}';render()" style="flex:1;padding:12px 4px;border:none;border-bottom:2.5px solid ${S.cTab===id?'var(--ac)':'transparent'};background:none;color:${S.cTab===id?'var(--ac)':'var(--txm)'};font-size:12px;font-weight:${S.cTab===id?700:400};cursor:pointer;font-family:var(--sans)">${l}</button>`).join('')}
    </div>
    <div style="padding:14px 14px 80px">
      ${S.cTab==='paleta'?rCP():S.cTab==='harmonias'?rCH():rCB()}
    </div>
  </div>`;
}

function rCP(){
  const grupos=['Todos',...new Set(PANTONE.map(c=>c.grupo))];
  const list=S.cGrupo==='Todos'?PANTONE:PANTONE.filter(c=>c.grupo===S.cGrupo);
  const sel=S.cSel;
  return `
    <div style="display:flex;gap:6px;overflow-x:auto;margin-bottom:14px;padding-bottom:4px">
      ${grupos.map(g=>`<button class="chip ${S.cGrupo===g?'on':''}" onclick="S.cGrupo='${g}';render()" style="flex-shrink:0">${g}</button>`).join('')}
    </div>
    <div style="display:grid;grid-template-columns:repeat(3,1fr);gap:7px;margin-bottom:${sel?'14px':'0'}">
      ${list.map((c,i)=>`
        <button onclick="S.cSel=S.cSel&&S.cSel.id==='${c.id}'?null:JSON.parse(this.dataset.c);render()" data-c='${JSON.stringify(c).replace(/'/g,"&#39;")}' style="border-radius:12px;border:2.5px solid ${sel?.id===c.id?'var(--ac)':'transparent'};overflow:hidden;background:none;padding:0;cursor:pointer;transform:${sel?.id===c.id?'scale(1.04)':'scale(1)'};transition:all .2s;box-shadow:${sel?.id===c.id?'0 4px 14px '+c.hex+'60':'0 2px 6px rgba(0,0,0,.06)'};animation:up .3s ease ${i*22}ms both">
          <div style="height:58px;background:${c.hex};position:relative">${sel?.id===c.id?`<div style="position:absolute;top:4px;right:4px;width:17px;height:17px;border-radius:50%;background:rgba(255,255,255,.9);display:flex;align-items:center;justify-content:center;font-size:9px;font-weight:700;color:var(--ac)">✓</div>`:''}</div>
          <div style="padding:5px 6px 7px;background:#FFF;text-align:left"><p style="font-size:10px;font-weight:700;color:var(--tx);line-height:1.2">${c.nome}</p><p style="font-size:9px;color:var(--txm)">${c.grupo}</p></div>
        </button>`).join('')}
    </div>
    ${sel?`<div style="border-radius:16px;overflow:hidden;box-shadow:0 6px 24px ${sel.hex}40;animation:up .3s ease">
      <div style="background:${sel.hex};padding:16px 16px 12px">
        <p style="font-family:var(--serif);font-size:20px;font-weight:700;color:${tT(sel.hex)};margin-bottom:1px">${sel.nome}</p>
        <p style="font-size:11px;color:${tT(sel.hex)};opacity:.65">${sel.hex.toUpperCase()} · ${sel.grupo}</p>
      </div>
      <div style="background:#FFF;padding:13px 15px">
        <p style="font-size:11px;font-weight:700;text-transform:uppercase;letter-spacing:.8px;color:var(--txs);margin-bottom:9px">Combina com</p>
        ${(()=>{const g=Object.values(HD).flatMap(h=>h.grupos).find(g=>g.includes(sel.nome));if(!g)return`<p style="font-size:12px;color:var(--txm)">Explore as harmonias na aba ⊕</p>`;return`<div style="display:flex;gap:8px;flex-wrap:wrap">${g.map(n=>{const c=PANTONE.find(p=>p.nome===n);return c?`<div style="text-align:center"><div style="width:42px;height:42px;border-radius:9px;background:${c.hex};border:1px solid rgba(0,0,0,.08);margin-bottom:3px"></div><p style="font-size:9px;color:var(--txs)">${c.nome.split(' ')[0]}</p></div>`:''}).join('')}</div>`;})()}
      </div>
    </div>`:''}`;
}

function rCH(){
  const h=HD[S.cHarm];
  return `
    <div style="display:flex;gap:6px;overflow-x:auto;margin-bottom:12px;padding-bottom:4px">
      ${Object.entries(HD).map(([k,h])=>`<button class="chip ${S.cHarm===k?'on':''}" onclick="S.cHarm='${k}';render()" style="flex-shrink:0">${h.icon} ${h.label}</button>`).join('')}
    </div>
    <div style="background:var(--acl);border-radius:12px;padding:11px 13px;margin-bottom:13px">
      <p style="font-size:13px;font-weight:700;color:var(--acd);margin-bottom:2px">${h.icon} ${h.label}</p>
      <p style="font-size:12px;color:var(--acd)">${h.desc}</p>
    </div>
    ${h.grupos.map((grupo,i)=>{const cores=grupo.map(n=>PANTONE.find(p=>p.nome===n)).filter(Boolean);return`<div class="card" style="overflow:hidden;margin-bottom:10px;animation:up .3s ease ${i*60}ms both">
      <div style="display:flex;height:44px">${cores.map(c=>`<div style="flex:1;background:${c.hex}"></div>`).join('')}</div>
      <div style="padding:11px 13px">
        <div style="display:flex;gap:7px;margin-bottom:9px;flex-wrap:wrap">${cores.map(c=>`<div style="display:flex;align-items:center;gap:3px"><div style="width:10px;height:10px;border-radius:50%;background:${c.hex};border:1px solid rgba(0,0,0,.1)"></div><span style="font-size:10px;color:var(--tx);font-weight:500">${c.nome}</span></div>`).join('')}</div>
        <div style="display:flex;gap:4px">${cores.map((c,j)=>`<div style="flex:1;padding:6px 4px;border-radius:8px;background:${c.hex};text-align:center"><p style="font-size:7px;font-weight:700;text-transform:uppercase;color:${tT(c.hex)};opacity:.7;margin-bottom:1px">${['principal','segunda','detalhe'][j]||'+'}</p><p style="font-size:8px;font-weight:600;color:${tT(c.hex)}">${c.nome.split(' ')[0]}</p></div>`).join('')}</div>
      </div>
    </div>`;}).join('')}`;
}

function rCB(){
  const bc=S.bCores;
  return `
    <p style="font-family:var(--serif);font-size:18px;font-weight:700;margin-bottom:4px">Color Blocking Builder</p>
    <p style="font-size:13px;color:var(--txs);margin-bottom:13px;line-height:1.5">Selecione 2 a 4 cores e avalie</p>
    <div style="border-radius:15px;overflow:hidden;margin-bottom:11px">
      <div style="height:68px;display:flex">${bc.length===0?`<div style="flex:1;background:var(--alt);display:flex;align-items:center;justify-content:center"><p style="font-size:12px;color:var(--txm)">Selecione cores abaixo</p></div>`:bc.map(c=>`<div style="flex:1;background:${c.hex};display:flex;align-items:flex-end;justify-content:center;padding-bottom:5px"><p style="font-size:8px;font-weight:700;color:${tT(c.hex)};text-align:center">${c.nome.split(' ')[0]}</p></div>`).join('')}</div>
      ${S.builderMsg?`<div style="padding:9px 13px;background:${S.builderMsg.includes('✦')?'var(--acl)':'#FDE8E8'}"><p style="font-size:12px;color:${S.builderMsg.includes('✦')?'var(--acd)':'var(--err)'};line-height:1.5">${S.builderMsg}</p></div>`:''}
    </div>
    <div style="display:flex;gap:7px;margin-bottom:${bc.length?'11px':'13px'}">
      <button onclick="avaliarB()" ${bc.length<2?'disabled':''} class="btn" style="flex:2;padding:11px;font-size:13px">Avaliar</button>
      <button onclick="S.bCores=[];S.builderMsg='';render()" class="btn2" style="flex:1;padding:11px;font-size:13px">Limpar</button>
    </div>
    ${bc.length?`<div style="display:flex;gap:5px;flex-wrap:wrap;margin-bottom:11px">${bc.map(c=>`<button onclick="togB('${c.id}')" style="display:flex;align-items:center;gap:4px;padding:5px 9px 5px 7px;border-radius:20px;border:1.5px solid var(--ac);background:var(--acl);cursor:pointer"><div style="width:13px;height:13px;border-radius:50%;background:${c.hex};border:1px solid rgba(0,0,0,.1)"></div><span style="font-size:11px;font-weight:600;color:var(--acd)">${c.nome.split(' ')[0]}</span><span style="color:var(--acd);opacity:.6;font-size:11px">×</span></button>`).join('')}</div>`:''}
    <p style="font-size:10px;font-weight:700;text-transform:uppercase;letter-spacing:.8px;color:var(--txs);margin-bottom:9px">Pantone SS 2026</p>
    <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:5px">
      ${PANTONE.map((c,i)=>{const sel=bc.some(x=>x.id===c.id);return`<button onclick="togB('${c.id}')" style="border-radius:9px;border:2px solid ${sel?'var(--ac)':'transparent'};overflow:hidden;background:none;padding:0;cursor:pointer;transform:${sel?'scale(1.06)':'scale(1)'};transition:all .15s;animation:up .3s ease ${i*14}ms both">
        <div style="height:42px;background:${c.hex};position:relative">${sel?`<div style="position:absolute;inset:0;background:rgba(0,0,0,.2);display:flex;align-items:center;justify-content:center"><span style="font-size:12px;font-weight:700;color:#FFF">✓</span></div>`:''}</div>
        <div style="padding:3px 2px 4px;background:#FFF"><p style="font-size:8px;font-weight:600;color:var(--tx);text-align:center">${c.nome.split(' ')[0]}</p></div>
      </button>`;}).join('')}
    </div>`;
}

function togB(id){
  const c=PANTONE.find(p=>p.id===id);if(!c)return;
  if(S.bCores.some(x=>x.id===id))S.bCores=S.bCores.filter(x=>x.id!==id);
  else if(S.bCores.length<4)S.bCores.push(c);
  else{S.builderMsg='Máximo 4 cores';setTimeout(()=>{S.builderMsg='';render()},1500);}
  render();
}
function avaliarB(){
  const bc=S.bCores;if(bc.length<2){S.builderMsg='Selecione pelo menos 2 cores';render();return;}
  const grupos=bc.map(c=>c.grupo),uniq=[...new Set(grupos)];
  let m='';
  if(uniq.length===1)m='✦ MONOCROMÁTICO — elegância máxima. Varie as texturas.';
  else if(grupos.includes('Neutro')&&uniq.length===2)m=`✦ Neutro + Cor — look certeiro. ${bc.find(c=>c.grupo!=='Neutro')?.nome} é seu ponto focal.`;
  else if(uniq.length>=3&&!grupos.includes('Neutro'))m=`✦ COLOR BLOCKING SS 2026! ${bc.length} blocos de cor. Peças sólidas + acessórios neutros.`;
  else m='✦ Combinação harmoniosa. Uma cor domina (70%), a outra aparece (30%).';
  S.builderMsg=m;render();
}

// ═══════════════════════════════════════════════════
// INIT
// ═══════════════════════════════════════════════════
goTab(0);
</script>
</body>
</html>
