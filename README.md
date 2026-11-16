[הבר הווירטואלי שלי.html](https://github.com/user-attachments/files/34938258/default.html)
<!doctype html>
<html lang="he" dir="rtl">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>הבר הווירטואלי שלי</title>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Heebo:wght@400;600;800&family=Frank+Ruhl+Libre:wght@700;900&display=swap">
<style>
:root{--bg:#efe9dc;--panel:#fbf8f1;--ink:#241f18;--mute:#72695a;--line:#d9cfba;--accent:#9c4a14;--onaccent:#fff;--plank:#8b5a33;--plank2:#5e3a1e;--wall:#e4dac6;--danger:#a32a2a;box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px);color-scheme:light}
@media (prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#101a17;--panel:#18241f;--ink:#efe7d5;--mute:#a29a86;--line:#2c3c35;--accent:#e9a23b;--onaccent:#1a1206;--plank:#7a4e2b;--plank2:#4a2d17;--wall:#15211c;--danger:#ef7a7a;color-scheme:dark}}
:root[data-theme="dark"]{--bg:#101a17;--panel:#18241f;--ink:#efe7d5;--mute:#a29a86;--line:#2c3c35;--accent:#e9a23b;--onaccent:#1a1206;--plank:#7a4e2b;--plank2:#4a2d17;--wall:#15211c;--danger:#ef7a7a;color-scheme:dark}
html{scroll-padding-top:env(safe-area-inset-top,0px)}
*{box-sizing:border-box}
body{margin:0;background:var(--bg);color:var(--ink);font:400 16px/1.5 Heebo,system-ui,sans-serif}
.wrap{max-width:980px;margin:0 auto;padding:20px 16px 60px}
h1{font:900 clamp(30px,6vw,46px)/1.1 "Frank Ruhl Libre",Georgia,serif;margin:0 0 4px}
.sub{color:var(--mute);margin:0 0 18px}
.stats{display:flex;gap:10px;flex-wrap:wrap;margin-bottom:18px}
.stat{background:var(--panel);border:1px solid var(--line);border-radius:10px;padding:8px 14px;min-width:110px}
.stat b{display:block;font-size:24px;font-weight:800}
.stat span{color:var(--mute);font-size:13px}
.bar{display:flex;gap:8px;flex-wrap:wrap;align-items:center;margin-bottom:16px}
input,select,textarea,button{font:inherit;color:var(--ink)}
input,select,textarea{background:var(--panel);border:1px solid var(--line);border-radius:8px;padding:9px 11px;width:100%}
.bar input{flex:1 1 180px;width:auto}.bar select{flex:0 1 150px;width:auto}
button{cursor:pointer;border:1px solid var(--line);background:var(--panel);border-radius:8px;padding:9px 14px}
button:hover{border-color:var(--accent)}
button:focus-visible,input:focus-visible,select:focus-visible,textarea:focus-visible,.bottle:focus-visible{outline:3px solid var(--accent);outline-offset:2px}
.primary{background:var(--accent);color:var(--onaccent);border-color:var(--accent);font-weight:600}
.danger{color:var(--danger)}
.tabs{display:inline-flex;border:1px solid var(--line);border-radius:8px;overflow:hidden}
.tabs button{border:0;border-radius:0;background:transparent}
.tabs button[aria-pressed="true"]{background:var(--ink);color:var(--bg)}
/* shelves */
.cabinet{background:var(--wall);border:1px solid var(--line);border-radius:12px;padding:14px 14px 4px}
.shelf{margin-bottom:22px}
.shelf h2{font:700 15px Heebo,sans-serif;color:var(--mute);margin:0 0 6px 0}
.row{display:flex;flex-wrap:wrap;gap:14px;align-items:flex-end;padding:0 10px;min-height:60px;border-bottom:14px solid var(--plank);box-shadow:0 5px 0 var(--plank2)}
.bottle{all:unset;cursor:pointer;display:flex;flex-direction:column;align-items:center;width:62px;position:relative;margin-bottom:0}
.bottle .cap{width:12px;height:8px;background:var(--plank2);border-radius:2px 2px 0 0}
.bottle .neck{width:16px;height:30px;background:var(--c);opacity:.85;border-radius:3px 3px 0 0;position:relative;overflow:hidden}
.bottle .body{width:62px;height:118px;border-radius:14px 14px 5px 5px;background:color-mix(in srgb,var(--c) 22%,transparent);border:2px solid color-mix(in srgb,var(--c) 70%,#000);position:relative;overflow:hidden}
.bottle .liq{position:absolute;inset:auto 0 0 0;background:var(--c);opacity:.9}
.bottle .lab{position:absolute;inset:38px 5px auto 5px;background:#f6efdc;color:#2a2418;border-radius:3px;font-size:10.5px;line-height:1.15;text-align:center;padding:4px 2px;font-weight:600;overflow:hidden;max-height:50px}
.bottle:hover .body{transform:translateY(-4px)}.bottle .body{transition:transform .15s}
.qty{position:absolute;top:34px;inset-inline-start:-6px;background:var(--accent);color:var(--onaccent);border-radius:20px;font-size:12px;font-weight:800;padding:0 6px;z-index:2}
.low{outline:2px dashed var(--danger);outline-offset:3px;border-radius:8px}
/* list */
.list{background:var(--panel);border:1px solid var(--line);border-radius:12px;overflow:hidden}
.item{display:grid;grid-template-columns:14px 1fr auto auto;gap:12px;align-items:center;padding:10px 14px;border-bottom:1px solid var(--line)}
.item:last-child{border:0}
.dot{width:14px;height:14px;border-radius:50%;background:var(--c)}
.item small{color:var(--mute);display:block}
.step{display:flex;align-items:center;gap:6px}
.step button{padding:2px 10px;font-size:18px;line-height:1.3}
.tag{font-size:12px;color:var(--danger);font-weight:600}
.empty{padding:36px 16px;text-align:center;color:var(--mute)}
/* dialog */
dialog{border:1px solid var(--line);background:var(--panel);color:var(--ink);border-radius:14px;padding:20px;width:min(520px,94vw)}
dialog::backdrop{background:rgba(0,0,0,.55)}
dialog h3{margin:0 0 12px;font:700 22px "Frank Ruhl Libre",serif}
.grid{display:grid;grid-template-columns:1fr 1fr;gap:10px}
.grid .full{grid-column:1/-1}
label{font-size:13px;color:var(--mute);display:block;margin-bottom:3px}
.actions{display:flex;gap:8px;margin-top:14px;flex-wrap:wrap}
.actions .sp{flex:1}
#toast{position:fixed;inset-inline:0;bottom:calc(20px + env(safe-area-inset-bottom,0px));text-align:center;pointer-events:none}
#toast span{background:var(--ink);color:var(--bg);padding:8px 16px;border-radius:20px;display:none}
@media (max-width:520px){.item{grid-template-columns:14px 1fr auto}.item .step{grid-column:2/-1}}
</style>
</head>
<body>
<div class="wrap">
  <h1>הבר הווירטואלי שלי</h1>
  <p class="sub">כל הבקבוקים שלך במקום אחד. הנתונים נשמרים בדפדפן שלך.</p>
  <div class="stats" id="stats"></div>
  <div class="bar">
    <input id="q" type="search" placeholder="חיפוש לפי שם, מותג או הערה" aria-label="חיפוש">
    <select id="cat" aria-label="סינון לפי קטגוריה"></select>
    <div class="tabs" role="group" aria-label="תצוגה">
      <button id="tBar" aria-pressed="true">הבר</button>
      <button id="tList" aria-pressed="false">רשימה</button>
    </div>
    <button class="primary" id="add">הוספת בקבוק</button>
    <button id="data">גיבוי וייבוא</button>
  </div>
  <div id="view"></div>
</div>

<dialog id="dlg">
  <h3 id="dTitle">בקבוק חדש</h3>
  <div class="grid">
    <div class="full"><label for="fName">שם</label><input id="fName" placeholder="למשל: Jameson"></div>
    <div><label for="fCat">קטגוריה</label><select id="fCat"></select></div>
    <div><label for="fBrand">מותג / יצרן</label><input id="fBrand"></div>
    <div><label for="fVol">נפח (מ״ל)</label><input id="fVol" type="number" min="0" value="700"></div>
    <div><label for="fAbv">אחוז אלכוהול</label><input id="fAbv" type="number" min="0" max="100" step="0.1" value="40"></div>
    <div><label for="fQty">כמות בקבוקים</label><input id="fQty" type="number" min="0" value="1"></div>
    <div><label for="fRem">נשאר בבקבוק: <b id="remOut">100</b>%</label><input id="fRem" type="range" min="0" max="100" step="5" value="100"></div>
    <div class="full"><label for="fNote">הערות</label><textarea id="fNote" rows="2"></textarea></div>
  </div>
  <div class="actions">
    <button class="primary" id="save">שמירה</button>
    <button id="cancel">ביטול</button>
    <span class="sp"></span>
    <button class="danger" id="del">מחיקה</button>
  </div>
</dialog>

<dialog id="dlg2">
  <h3>גיבוי וייבוא</h3>
  <p class="sub">העתק את הטקסט ושמור אותו אצלך, או הדבק גיבוי קודם וייבא.</p>
  <textarea id="json" rows="9" dir="ltr" spellcheck="false"></textarea>
  <div class="actions">
    <button id="copy">העתקה</button>
    <button class="primary" id="imp">ייבוא (מחליף את הרשימה)</button>
    <span class="sp"></span>
    <button id="close2">סגירה</button>
  </div>
</dialog>
<div id="toast" aria-live="polite"><span></span></div>

<script>
const CATS={'וויסקי':'#c47a1c','וודקה':'#7fb6cf','רום':'#8a3f1c','ג’ין':'#4fa58a','טקילה':'#d8b640','ליקר':'#b03d78','קוניאק וברנדי':'#9a5126','יין':'#8a2040','בירה':'#d1a02a','אחר':'#6f8796'};
const KEY='virtual-bar-v1';
let items=[],view='bar',editId=null;
const $=id=>document.getElementById(id);
const esc=s=>String(s??'').replace(/[&<>"']/g,c=>({'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;',"'":'&#39;'}[c]));
function load(){try{const r=localStorage.getItem(KEY);items=r?JSON.parse(r):[];if(!Array.isArray(items))items=[]}catch(e){items=[]}}
function save(){try{localStorage.setItem(KEY,JSON.stringify(items))}catch(e){toast('השמירה בדפדפן לא זמינה')}}
function toast(t){const s=$('toast').firstElementChild;s.textContent=t;s.style.display='inline-block';clearTimeout(toast.t);toast.t=setTimeout(()=>s.style.display='none',2200)}
const color=c=>CATS[c]||CATS['אחר'];
function filtered(){
  const q=$('q').value.trim().toLowerCase(),c=$('cat').value;
  return items.filter(i=>(!c||i.cat===c)&&(!q||[i.name,i.brand,i.note,i.cat].join(' ').toLowerCase().includes(q)));
}
function stats(){
  const total=items.reduce((a,i)=>a+(+i.qty||0),0);
  const low=items.filter(i=>i.rem<=20||i.qty==0).length;
  $('stats').innerHTML=`<div class="stat"><b>${items.length}</b><span>פריטים</span></div><div class="stat"><b>${total}</b><span>בקבוקים</span></div><div class="stat"><b>${low}</b><span>עומדים להיגמר</span></div>`;
}
function render(){
  stats();
  const list=filtered(),v=$('view');
  if(!items.length){v.innerHTML=`<div class="empty">הבר ריק. הוסף את הבקבוק הראשון שלך.<br><br><button id="demo">טעינת דוגמאות</button></div>`;return}
  if(!list.length){v.innerHTML='<div class="empty">לא נמצאו בקבוקים שמתאימים לחיפוש.</div>';return}
  if(view==='bar'){
    const groups={};list.forEach(i=>(groups[i.cat]=groups[i.cat]||[]).push(i));
    v.innerHTML='<div class="cabinet">'+Object.keys(groups).map(c=>`<section class="shelf"><h2>${esc(c)} (${groups[c].length})</h2><div class="row">${groups[c].map(bottle).join('')}</div></section>`).join('')+'</div>';
  }else{
    v.innerHTML='<div class="list">'+list.map(i=>`<div class="item" style="--c:${color(i.cat)}"><span class="dot"></span>
      <div><b>${esc(i.name)}</b>${i.brand?' · '+esc(i.brand):''}<small>${esc(i.cat)} · ${i.vol||'?'} מ״ל · ${i.abv||'?'}% · נשאר ${i.rem}%${i.note?' · '+esc(i.note):''}</small>${(i.rem<=20||i.qty==0)?'<span class="tag">עומד להיגמר</span>':''}</div>
      <div class="step"><button data-dec="${i.id}" aria-label="הפחתה">−</button><b>${i.qty}</b><button data-inc="${i.id}" aria-label="הוספה">+</button></div>
      <button data-edit="${i.id}">עריכה</button></div>`).join('')+'</div>';
  }
}
function bottle(i){
  const low=i.rem<=20||i.qty==0;
  return `<button class="bottle${low?' low':''}" data-edit="${i.id}" style="--c:${color(i.cat)}" title="${esc(i.name)} · נשאר ${i.rem}%" aria-label="${esc(i.name)}, נשאר ${i.rem} אחוז, כמות ${i.qty}">
    ${i.qty>1?`<span class="qty">×${i.qty}</span>`:''}<span class="cap"></span><span class="neck"></span>
    <span class="body"><span class="liq" style="height:${i.rem}%"></span><span class="lab">${esc(i.name)}</span></span></button>`;
}
function openForm(id){
  editId=id;const i=items.find(x=>x.id===id)||{name:'',cat:'וויסקי',brand:'',vol:700,abv:40,qty:1,rem:100,note:''};
  $('dTitle').textContent=id?'עריכת בקבוק':'בקבוק חדש';
  $('fName').value=i.name;$('fCat').value=i.cat;$('fBrand').value=i.brand;$('fVol').value=i.vol;$('fAbv').value=i.abv;
  $('fQty').value=i.qty;$('fRem').value=i.rem;$('remOut').textContent=i.rem;$('fNote').value=i.note;
  $('del').style.display=id?'':'none';$('dlg').showModal();$('fName').focus();
}
function saveForm(){
  const name=$('fName').value.trim();
  if(!name){toast('צריך להזין שם');$('fName').focus();return}
  const d={name,cat:$('fCat').value,brand:$('fBrand').value.trim(),vol:+$('fVol').value||0,abv:+$('fAbv').value||0,qty:Math.max(0,+$('fQty').value||0),rem:+$('fRem').value,note:$('fNote').value.trim()};
  if(editId){Object.assign(items.find(x=>x.id===editId),d)}else{items.push({id:'b'+Date.now().toString(36)+Math.random().toString(36).slice(2,5),...d})}
  save();$('dlg').close();render();toast('נשמר');
}
const catOpts=Object.keys(CATS).map(c=>`<option>${c}</option>`).join('');
$('fCat').innerHTML=catOpts;$('cat').innerHTML='<option value="">כל הקטגוריות</option>'+catOpts;
$('q').oninput=render;$('cat').onchange=render;
$('tBar').onclick=()=>{view='bar';$('tBar').setAttribute('aria-pressed',true);$('tList').setAttribute('aria-pressed',false);render()};
$('tList').onclick=()=>{view='list';$('tList').setAttribute('aria-pressed',true);$('tBar').setAttribute('aria-pressed',false);render()};
$('add').onclick=()=>openForm(null);
$('save').onclick=saveForm;$('cancel').onclick=()=>$('dlg').close();
$('fRem').oninput=e=>$('remOut').textContent=e.target.value;
$('del').onclick=()=>{if(confirm('למחוק את הבקבוק?')){items=items.filter(x=>x.id!==editId);save();$('dlg').close();render()}};
$('data').onclick=()=>{$('json').value=JSON.stringify(items,null,1);$('dlg2').showModal()};
$('close2').onclick=()=>$('dlg2').close();
$('copy').onclick=async()=>{try{await navigator.clipboard.writeText($('json').value);toast('הועתק')}catch(e){$('json').select();toast('סמן והעתק ידנית')}};
$('imp').onclick=()=>{
  try{const a=JSON.parse($('json').value);if(!Array.isArray(a))throw 0;
    items=a.filter(x=>x&&x.name).map(x=>({id:x.id||'b'+Math.random().toString(36).slice(2,9),name:String(x.name),cat:CATS[x.cat]?x.cat:'אחר',brand:x.brand||'',vol:+x.vol||0,abv:+x.abv||0,qty:+x.qty||0,rem:Math.min(100,Math.max(0,+x.rem||0)),note:x.note||''}));
    save();$('dlg2').close();render();toast('יובאו '+items.length+' פריטים');
  }catch(e){toast('הטקסט אינו גיבוי תקין')}
};
$('view').onclick=e=>{
  const t=e.target.closest('button');if(!t)return;
  if(t.id==='demo'){items=[['Jameson','וויסקי','Irish',700,40,1,80],['Absolut','וודקה','',700,40,2,100],['Bacardi Carta Blanca','רום','',700,37.5,1,45],['Tanqueray','ג’ין','',700,43.1,1,15],['Olmeca','טקילה','',700,38,1,60],['Aperol','ליקר','',700,11,1,90]].map((a,k)=>({id:'d'+k,name:a[0],cat:a[1],brand:a[2],vol:a[3],abv:a[4],qty:a[5],rem:a[6],note:''}));save();render();return}
  const g=k=>items.find(x=>x.id===t.dataset[k]);
  if(t.dataset.edit)openForm(t.dataset.edit);
  else if(t.dataset.inc){g('inc').qty++;save();render()}
  else if(t.dataset.dec){const i=g('dec');i.qty=Math.max(0,i.qty-1);save();render()}
};
load();render();
</script>
</body>
</html>
