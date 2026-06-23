<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0">
<title>BCF — Controle de Importação</title>
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@tabler/icons-webfont@2.47.0/tabler-icons.min.css">
<style>
* { box-sizing: border-box; margin: 0; padding: 0; }
:root {
  --bg:#f5f5f3; --surface:#fff; --surface2:#f1efe8;
  --text:#1a1a18; --text2:#5f5e5a; --text3:#888780;
  --border:rgba(0,0,0,0.12); --border2:rgba(0,0,0,0.22);
  --blue-bg:#e6f1fb; --blue-text:#0c447c;
  --green-bg:#eaf3de; --green-text:#3b6d11;
  --red-bg:#fcebeb; --red-text:#a32d2d;
  --amber-bg:#faeeda; --amber-text:#854f0b;
  --radius:12px; --radius-sm:8px;
}
body { font-family:-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif; background:var(--bg); color:var(--text); max-width:430px; margin:0 auto; min-height:100vh; font-size:14px; }

.app-header { background:var(--surface); border-bottom:.5px solid var(--border); padding:14px 16px 0; position:sticky; top:0; z-index:100; }
.app-title { font-size:17px; font-weight:600; }
.app-sub { font-size:11px; color:var(--text3); margin-top:2px; margin-bottom:10px; }
.tabs { display:flex; }
.tab { flex:1; padding:9px 2px; text-align:center; font-size:11px; font-weight:500; color:var(--text3); border-bottom:2px solid transparent; cursor:pointer; }
.tab.active { color:#185fa5; border-bottom-color:#185fa5; }

.section { display:none; padding:12px 16px 80px; }
.section.active { display:block; }

/* loading */
.loading { text-align:center; padding:50px 20px; }
.spinner { width:32px; height:32px; border:3px solid var(--border2); border-top-color:#185fa5; border-radius:50%; animation:spin .8s linear infinite; margin:0 auto 12px; }
@keyframes spin { to { transform:rotate(360deg); } }

/* config banner */
.config-banner { background:#042c53; color:#b5d4f4; border-radius:var(--radius); padding:14px 16px; margin-bottom:14px; }
.config-banner h2 { font-size:15px; font-weight:600; color:#e6f1fb; margin-bottom:6px; }
.config-banner p { font-size:12px; line-height:1.6; }
.config-banner input { width:100%; margin-top:10px; padding:9px 12px; border-radius:var(--radius-sm); border:none; font-size:13px; background:#0c447c; color:#e6f1fb; outline:none; }
.config-banner input::placeholder { color:#7aaed4; }
.config-banner button { margin-top:8px; width:100%; padding:9px; border-radius:var(--radius-sm); border:none; background:#185fa5; color:#fff; font-size:13px; font-weight:600; cursor:pointer; }

/* totals */
.totals-banner { background:#042c53; color:#b5d4f4; border-radius:var(--radius); padding:14px 16px; margin-bottom:14px; }
.totals-banner .tb-title { font-size:11px; opacity:.7; margin-bottom:4px; }
.totals-banner .tb-val { font-size:26px; font-weight:700; color:#e6f1fb; }
.totals-banner .tb-row { display:flex; gap:20px; margin-top:10px; }
.totals-banner .tbi-l { font-size:10px; opacity:.7; }
.totals-banner .tbi-v { font-size:14px; font-weight:600; color:#e6f1fb; }

.summary-grid { display:grid; grid-template-columns:repeat(2,1fr); gap:10px; margin-bottom:14px; }
.sum-card { background:var(--surface); border-radius:var(--radius); border:.5px solid var(--border); padding:14px; }
.sum-label { font-size:11px; color:var(--text3); margin-bottom:4px; }
.sum-val { font-size:19px; font-weight:600; }

.card { background:var(--surface); border-radius:var(--radius); border:.5px solid var(--border); margin-bottom:10px; overflow:hidden; }
.card-header { padding:12px 14px; display:flex; align-items:center; gap:10px; cursor:pointer; }
.card-header:active { background:var(--surface2); }
.supplier-initial { width:38px; height:38px; border-radius:50%; display:flex; align-items:center; justify-content:center; font-size:13px; font-weight:600; flex-shrink:0; }
.card-title { flex:1; }
.card-title h3 { font-size:14px; font-weight:600; }
.card-title p { font-size:12px; color:var(--text3); margin-top:1px; }
.card-chevron { color:var(--text3); font-size:16px; transition:transform .2s; }
.card.expanded .card-chevron { transform:rotate(180deg); }
.card-detail { display:none; padding:0 14px 14px; border-top:.5px solid var(--border); }
.card.expanded .card-detail { display:block; }

.stat-row { display:grid; grid-template-columns:repeat(3,1fr); gap:8px; margin-top:12px; }
.stat-box { background:var(--surface2); border-radius:var(--radius-sm); padding:8px 10px; }
.stat-box .stat-label { font-size:10px; color:var(--text3); margin-bottom:2px; }
.stat-box .stat-val { font-size:13px; font-weight:600; }

.badge { display:inline-flex; align-items:center; padding:3px 8px; border-radius:20px; font-size:11px; font-weight:500; }
.badge-green { background:var(--green-bg); color:var(--green-text); }
.badge-blue { background:var(--blue-bg); color:var(--blue-text); }
.badge-amber { background:var(--amber-bg); color:var(--amber-text); }
.badge-gray { background:#f1efe8; color:#444441; }

.inv-list { margin-top:8px; }
.inv-item { padding:9px 0; border-bottom:.5px solid var(--border); display:flex; justify-content:space-between; align-items:flex-start; }
.inv-item:last-child { border-bottom:none; }
.inv-ref { font-size:13px; font-weight:500; }
.inv-sub { font-size:11px; color:var(--text3); margin-top:2px; }
.inv-val { text-align:right; }
.inv-total { font-size:13px; font-weight:600; }
.inv-saldo { font-size:11px; margin-top:2px; }
.saldo-ok { color:var(--green-text); }
.saldo-due { color:var(--red-text); }

.pag-item { background:var(--surface); border-radius:var(--radius); border:.5px solid var(--border); padding:12px 14px; margin-bottom:8px; display:flex; justify-content:space-between; align-items:center; }
.pag-left h4 { font-size:13px; font-weight:600; }
.pag-left p { font-size:11px; color:var(--text3); margin-top:2px; }
.pag-right { text-align:right; }
.pag-val { font-size:14px; font-weight:600; color:var(--red-text); }
.pag-date { font-size:11px; color:var(--text3); margin-top:2px; }

.crono-item { background:var(--surface); border-radius:var(--radius); border:.5px solid var(--border); padding:12px 14px; margin-bottom:8px; }
.crono-head { display:flex; justify-content:space-between; align-items:flex-start; margin-bottom:8px; }
.crono-ref { font-size:13px; font-weight:600; }
.crono-sub { font-size:11px; color:var(--text3); margin-top:2px; }
.crono-vals { display:grid; grid-template-columns:1fr 1fr; gap:8px; }
.crono-box { background:var(--surface2); border-radius:6px; padding:8px 10px; }
.crono-box .cl { font-size:10px; color:var(--text3); }
.crono-box .cv { font-size:13px; font-weight:600; margin-top:2px; }
.crono-box .cd { font-size:10px; color:var(--text2); margin-top:1px; }

.emb-item { background:var(--surface); border-radius:var(--radius); border:.5px solid var(--border); padding:12px 14px; margin-bottom:8px; }
.emb-ref { font-size:13px; font-weight:600; }
.emb-sub { font-size:11px; color:var(--text3); margin-top:2px; margin-bottom:8px; }
.emb-dates { display:grid; grid-template-columns:repeat(3,1fr); gap:6px; }
.emb-dt { background:var(--surface2); border-radius:6px; padding:6px 8px; font-size:11px; }
.emb-dt .dl { color:var(--text3); font-size:10px; }
.emb-dt .dv { font-weight:600; margin-top:1px; }

.search-wrap { position:relative; padding:10px 0 12px; }
.search-icon { position:absolute; left:10px; top:50%; transform:translateY(-50%); color:var(--text3); font-size:16px; pointer-events:none; }
.search-input { width:100%; padding:9px 12px 9px 36px; border:.5px solid var(--border2); border-radius:var(--radius-sm); background:var(--surface2); color:var(--text); font-size:14px; outline:none; }
.result-item { background:var(--surface); border-radius:var(--radius); border:.5px solid var(--border); padding:12px 14px; margin-bottom:8px; }
.result-tag { font-size:10px; color:var(--text3); text-transform:uppercase; letter-spacing:.04em; margin-bottom:3px; }
.result-title { font-size:14px; font-weight:600; }
.result-sub { font-size:12px; color:var(--text2); margin-top:3px; }

.section-title { font-size:11px; font-weight:600; color:var(--text3); text-transform:uppercase; letter-spacing:.05em; margin:14px 0 8px; }

.sync-bar { display:flex; align-items:center; justify-content:space-between; background:var(--surface); border-radius:var(--radius-sm); padding:8px 12px; margin-bottom:12px; border:.5px solid var(--border); }
.sync-info { font-size:11px; color:var(--text3); }
.sync-btn { font-size:12px; color:#185fa5; font-weight:500; cursor:pointer; background:none; border:none; padding:0; }
.sync-btn:active { opacity:.6; }
</style>
</head>
<body>

<div class="app-header">
  <div class="app-title">BCF Controle de Importação</div>
  <div class="app-sub" id="app-sub">Extrapower</div>
  <div class="tabs">
    <div class="tab active" onclick="setTab('resumo')"><i class="ti ti-layout-dashboard"></i><br>Resumo</div>
    <div class="tab" onclick="setTab('fornecedores')"><i class="ti ti-building-factory"></i><br>Fornec.</div>
    <div class="tab" onclick="setTab('pagamentos')"><i class="ti ti-receipt"></i><br>Pagamentos</div>
    <div class="tab" onclick="setTab('cronograma')"><i class="ti ti-calendar-due"></i><br>Cronograma</div>
    <div class="tab" onclick="setTab('embarques')"><i class="ti ti-ship"></i><br>Embarques</div>
    <div class="tab" onclick="setTab('busca')"><i class="ti ti-search"></i><br>Buscar</div>
  </div>
</div>

<div id="sec-resumo" class="section active"><div class="loading"><div class="spinner"></div><p style="color:var(--text3);font-size:13px">Carregando dados...</p></div></div>
<div id="sec-fornecedores" class="section"><div class="loading"><div class="spinner"></div></div></div>
<div id="sec-pagamentos" class="section"><div class="loading"><div class="spinner"></div></div></div>
<div id="sec-cronograma" class="section"><div class="loading"><div class="spinner"></div></div></div>
<div id="sec-embarques" class="section"><div class="loading"><div class="spinner"></div></div></div>
<div id="sec-busca" class="section">
  <div class="search-wrap">
    <i class="ti ti-search search-icon"></i>
    <input class="search-input" type="text" placeholder="Fornecedor, invoice, BT..." id="search-input" oninput="doSearch(this.value)">
  </div>
  <div id="search-results"><p style="color:var(--text3);font-size:13px;text-align:center;padding:30px 0">Digite para buscar</p></div>
</div>

<script>
// ── CONFIG ───────────────────────────────────────────────────────────────────
// Cole aqui o ID da sua planilha Google Sheets após publicar
const SHEET_ID = '1w7uxPy2BSNpI5rM08JVSA2LtiDg8GREh5XRrbqrJUU4'; // mantido para referência

const COLORS = {
  SHI:{bg:'#e6f1fb',color:'#0c447c'},
  XMN:{bg:'#eaf3de',color:'#3b6d11'},
  MLG:{bg:'#faeeda',color:'#854f0b'},
  BCF:{bg:'#fbeaf0',color:'#993556'},
  MIK:{bg:'#eeedfe',color:'#3c3489'},
  HSN:{bg:'#f1efe8',color:'#444441'},
};

let DATA = { fornecedores:[], pedidos:[], pagamentos:[], cronograma:[], embarques:[] };
let lastSync = null;

// ── GOOGLE SHEETS CSV FETCH ───────────────────────────────────────────────────
function sheetURL(sheetName) {
  const encoded = encodeURIComponent(sheetName);
  return `https://docs.google.com/spreadsheets/d/e/2PACX-1vQZgTpL19-oDTyz7S292tMVg6HSdIWcAzU_RqIDBI-y2tMajYa7xn2x6LUKhBFfKmLgy9DjXUYFnZpl/pub?output=csv&sheet=${encoded}`;
}

function parseCSV(text) {
  const lines = text.trim().split('\n');
  if(lines.length < 2) return [];
  const headers = parseCSVLine(lines[0]);
  return lines.slice(1).map(line => {
    const vals = parseCSVLine(line);
    const obj = {};
    headers.forEach((h,i) => obj[h.trim()] = (vals[i]||'').trim());
    return obj;
  }).filter(r => Object.values(r).some(v => v));
}

function parseCSVLine(line) {
  const result = []; let cur = ''; let inQ = false;
  for(let i=0;i<line.length;i++){
    const ch=line[i];
    if(ch==='"'){if(inQ&&line[i+1]==='"'){cur+='"';i++;}else{inQ=!inQ;}}
    else if(ch===','&&!inQ){result.push(cur);cur='';}
    else{cur+=ch;}
  }
  result.push(cur);
  return result;
}

function parseNum(v) { if(!v||v==='-') return 0; return parseFloat(String(v).replace(/[^\d.-]/g,''))||0; }
function parseDate(v) { if(!v) return ''; return v.replace(/(\d+)\/(\d+)\/(\d+)/,'$3-$2-$1'); }

async function fetchSheet(name) {
  const r = await fetch(sheetURL(name));
  if(!r.ok) throw new Error(`Erro ao ler aba ${name}`);
  return parseCSV(await r.text());
}

async function loadAllData() {
  const [forn, ped, pag, cron, emb] = await Promise.all([
    fetchSheet('Fornecedores'),
    fetchSheet('Pedidos'),
    fetchSheet('Pagamentos'),
    fetchSheet('Cronograma'),
    fetchSheet('Embarques'),
  ]);

  DATA.fornecedores = forn.map(r => ({
    cod: r['Código']||r['Codigo']||'',
    nome: r['Fornecedor']||'',
    status: r['Status']||'',
    produto: r['Produto']||'',
    canal: r['Canal']||'',
  }));

  DATA.pedidos = ped.filter(r => r['Invoice / BT'] && r['Invoice / BT']!=='TOTAL').map(r => ({
    cod: r['Código']||r['Codigo']||'',
    nome: r['Fornecedor']||'',
    inv: r['Invoice / BT']||'',
    valorUSD: parseNum(r['Real USD']),
    valorRMB: parseNum(r['Real RMB']),
    pagoUSD: parseNum(r['Pago USD']),
    pagoRMB: parseNum(r['Pago RMB']),
    saldoUSD: parseNum(r['Saldo USD']),
    saldoRMB: parseNum(r['Saldo RMB']),
    status: r['Status']||'',
    obs: r['Observação']||r['Observacao']||'',
  }));

  DATA.pagamentos = pag.filter(r => r['Fornecedor'] && r['Valor'] && r['Valor']!=='TOTAL').map(r => ({
    cod: r['Código']||r['Codigo']||'',
    nome: r['Fornecedor']||'',
    inv: r['Invoice / BT']||'',
    tipo: r['Tipo']||'',
    moeda: r['Moeda']||'USD',
    valor: parseNum(r['Valor']),
    data: r['Data']||'',
    status: r['Status']||'',
    obs: r['Observação']||r['Observacao']||'',
  }));

  DATA.cronograma = cron.filter(r => r['Fornecedor']).map(r => ({
    cod: r['Código']||r['Codigo']||'',
    nome: r['Fornecedor']||'',
    inv: r['Invoice / Pedido']||'',
    moeda: r['Moeda']||'USD',
    saldo: parseNum(r['Saldo']),
    data30: r['Data 30%']||'',
    val30: parseNum(r['Valor 30%']),
    data70: r['Data 70%']||'',
    val70: parseNum(r['Valor 70%']),
    obs: r['Observação']||r['Observacao']||'',
  }));

  DATA.embarques = emb.filter(r => r['Fornecedor']).map(r => ({
    cod: r['Código']||r['Codigo']||'',
    nome: r['Fornecedor']||'',
    filial: r['Filial']||'',
    refMex: r['Ref. MEX']||'',
    inv: r['Pedido / Invoice']||'',
    exportador: r['Exportador']||'',
    descricao: r['Descrição']||r['Descricao']||'',
    prontidao: r['Prontidão']||r['Prontidao']||'',
    etd: r['ETD']||'',
    eta: r['ETA']||'',
    status: r['Status']||'',
  }));

  lastSync = new Date();
}

// ── FORMATTERS ────────────────────────────────────────────────────────────────
function fmt(v, moeda='USD') {
  if(!v||v===0) return moeda==='RMB'?'¥0':'$0';
  return (moeda==='RMB'?'¥':'$')+Math.round(v).toLocaleString('pt-BR');
}
function fmtDate(d) {
  if(!d) return '—';
  const m=d.match(/(\d{1,2})\/(\d{1,2})\/(\d{4})/);
  if(m) return `${m[1].padStart(2,'0')}/${m[2].padStart(2,'0')}/${m[3]}`;
  const m2=d.match(/(\d{4})-(\d{2})-(\d{2})/);
  if(m2) return `${m2[3]}/${m2[2]}/${m2[1]}`;
  return d;
}
function statusBadge(s) {
  const map={'Ativo':'badge-blue','Finalizado':'badge-green','Em produção':'badge-amber','Embarcado':'badge-blue','Cancelado':'badge-gray'};
  return `<span class="badge ${map[s]||'badge-gray'}">${s||'—'}</span>`;
}
function initials(nome) { return nome.split(' ').map(w=>w[0]).join('').substring(0,2).toUpperCase(); }
function syncBar() {
  const t = lastSync ? lastSync.toLocaleTimeString('pt-BR',{hour:'2-digit',minute:'2-digit'}) : '—';
  return `<div class="sync-bar"><span class="sync-info"><i class="ti ti-refresh" style="font-size:12px"></i> Sync: ${t}</span><button class="sync-btn" onclick="reload()">Atualizar ↗</button></div>`;
}

// ── RESUMO ────────────────────────────────────────────────────────────────────
function buildResumo() {
  const totPedUSD = DATA.pedidos.reduce((s,p)=>s+p.valorUSD,0);
  const totPagoUSD = DATA.pedidos.reduce((s,p)=>s+p.pagoUSD,0);
  const totPedRMB = DATA.pedidos.reduce((s,p)=>s+p.valorRMB,0);
  const totPagoRMB = DATA.pedidos.reduce((s,p)=>s+p.pagoRMB,0);
  const saldoUSD = DATA.pedidos.reduce((s,p)=>s+p.saldoUSD,0);
  const saldoRMB = DATA.pedidos.reduce((s,p)=>s+p.saldoRMB,0);
  const totalBRL = Math.round(saldoUSD*5.4 + saldoRMB*0.75);

  const fCards = DATA.fornecedores.map(f => {
    const c = COLORS[f.cod]||COLORS.HSN;
    const peds = DATA.pedidos.filter(p=>p.cod===f.cod);
    const sU = peds.reduce((s,p)=>s+p.saldoUSD,0);
    const sR = peds.reduce((s,p)=>s+p.saldoRMB,0);
    const brl = Math.round(sU*5.4+sR*0.75);
    const pagoU = peds.reduce((s,p)=>s+p.pagoUSD,0);
    const pedU = peds.reduce((s,p)=>s+p.valorUSD,0);
    const pagoR = peds.reduce((s,p)=>s+p.pagoRMB,0);
    const pedR = peds.reduce((s,p)=>s+p.valorRMB,0);
    return `
    <div class="card">
      <div class="card-header" onclick="toggleCard(this)">
        <div class="supplier-initial" style="background:${c.bg};color:${c.color}">${initials(f.nome)}</div>
        <div class="card-title">
          <h3>${f.nome}</h3>
          <p>${f.status} · R$ ${brl.toLocaleString('pt-BR')} a pagar</p>
        </div>
        <i class="ti ti-chevron-down card-chevron"></i>
      </div>
      <div class="card-detail">
        <div style="margin:8px 0">${statusBadge(f.status)}</div>
        <div class="stat-row">
          <div class="stat-box"><div class="stat-label">Pedido</div><div class="stat-val">${fmt(pedU)}</div></div>
          <div class="stat-box"><div class="stat-label">Pago</div><div class="stat-val" style="color:var(--green-text)">${fmt(pagoU)}</div></div>
          <div class="stat-box"><div class="stat-label">Saldo</div><div class="stat-val" style="color:${sU>0?'var(--red-text)':'var(--green-text)'}">${fmt(sU)}</div></div>
        </div>
        ${pedR>0?`<div class="stat-row" style="margin-top:6px">
          <div class="stat-box"><div class="stat-label">Pedido RMB</div><div class="stat-val">${fmt(pedR,'RMB')}</div></div>
          <div class="stat-box"><div class="stat-label">Pago RMB</div><div class="stat-val" style="color:var(--green-text)">${fmt(pagoR,'RMB')}</div></div>
          <div class="stat-box"><div class="stat-label">Saldo RMB</div><div class="stat-val" style="color:var(--red-text)">${fmt(sR,'RMB')}</div></div>
        </div>`:''}
      </div>
    </div>`;
  }).join('');

  document.getElementById('sec-resumo').innerHTML = `
    <div style="height:12px"></div>
    ${syncBar()}
    <div class="totals-banner">
      <div class="tb-title">Saldo total a pagar (BRL)</div>
      <div class="tb-val">R$ ${totalBRL.toLocaleString('pt-BR')}</div>
      <div style="font-size:11px;opacity:.6;margin-top:2px">USD 5,40 · RMB 0,75</div>
      <div class="tb-row">
        <div><div class="tbi-l">Saldo USD</div><div class="tbi-v">${fmt(saldoUSD)}</div></div>
        <div><div class="tbi-l">Saldo RMB</div><div class="tbi-v">${fmt(saldoRMB,'RMB')}</div></div>
      </div>
    </div>
    <div class="summary-grid">
      <div class="sum-card"><div class="sum-label">Total pedido USD</div><div class="sum-val">${fmt(totPedUSD)}</div></div>
      <div class="sum-card"><div class="sum-label">Total pago USD</div><div class="sum-val" style="color:var(--green-text)">${fmt(totPagoUSD)}</div></div>
      <div class="sum-card"><div class="sum-label">Total pedido RMB</div><div class="sum-val">${fmt(totPedRMB,'RMB')}</div></div>
      <div class="sum-card"><div class="sum-label">Total pago RMB</div><div class="sum-val" style="color:var(--green-text)">${fmt(totPagoRMB,'RMB')}</div></div>
    </div>
    <div class="section-title">Por fornecedor</div>
    ${fCards}`;
}

// ── FORNECEDORES ──────────────────────────────────────────────────────────────
function buildFornecedores() {
  const html = DATA.fornecedores.map(f => {
    const c = COLORS[f.cod]||COLORS.HSN;
    const peds = DATA.pedidos.filter(p=>p.cod===f.cod);
    const pags = DATA.pagamentos.filter(p=>p.cod===f.cod).slice(0,4);
    return `
    <div class="card">
      <div class="card-header" onclick="toggleCard(this)">
        <div class="supplier-initial" style="background:${c.bg};color:${c.color}">${initials(f.nome)}</div>
        <div class="card-title"><h3>${f.nome}</h3><p>${f.produto||'—'} · ${f.canal||'—'}</p></div>
        <i class="ti ti-chevron-down card-chevron"></i>
      </div>
      <div class="card-detail">
        <div style="margin:8px 0">${statusBadge(f.status)}</div>
        <div class="section-title" style="margin-top:4px">Pedidos</div>
        <div class="inv-list">
        ${peds.map(p=>`
          <div class="inv-item">
            <div><div class="inv-ref">${p.inv}</div><div class="inv-sub">${p.obs||p.status}</div></div>
            <div class="inv-val">
              <div class="inv-total">${p.valorUSD?fmt(p.valorUSD):fmt(p.valorRMB,'RMB')}</div>
              <div class="inv-saldo ${(p.saldoUSD||p.saldoRMB)>0?'saldo-due':'saldo-ok'}">saldo: ${p.saldoUSD?fmt(p.saldoUSD):fmt(p.saldoRMB,'RMB')}</div>
            </div>
          </div>`).join('')||'<p style="font-size:12px;color:var(--text3);padding:8px 0">Nenhum pedido</p>'}
        </div>
        <div class="section-title">Últimos pagamentos</div>
        ${pags.map(p=>`
          <div style="display:flex;justify-content:space-between;padding:6px 0;border-bottom:.5px solid var(--border);font-size:12px">
            <span style="color:var(--text2)">${p.inv}${p.tipo?' · '+p.tipo:''}</span>
            <span style="font-weight:600;color:var(--green-text)">${fmt(p.valor,p.moeda)}</span>
          </div>`).join('')||'<p style="font-size:12px;color:var(--text3);padding:6px 0">Nenhum pagamento</p>'}
      </div>
    </div>`;
  }).join('');
  document.getElementById('sec-fornecedores').innerHTML = `<div style="height:12px"></div>${syncBar()}${html}`;
}

// ── PAGAMENTOS ────────────────────────────────────────────────────────────────
function buildPagamentos() {
  const sorted = [...DATA.pagamentos].sort((a,b)=>b.data.localeCompare(a.data));
  const html = sorted.map(p=>`
    <div class="pag-item">
      <div class="pag-left"><h4>${p.nome||p.cod}</h4><p>${p.inv}${p.tipo?' · '+p.tipo:''}${p.obs?' · '+p.obs:''}</p></div>
      <div class="pag-right"><div class="pag-val">- ${fmt(p.valor,p.moeda)}</div><div class="pag-date">${fmtDate(p.data)}</div></div>
    </div>`).join('');
  document.getElementById('sec-pagamentos').innerHTML = `<div style="height:12px"></div>${syncBar()}<div class="section-title">Pagamentos realizados (${sorted.length})</div>${html}`;
}

// ── CRONOGRAMA ────────────────────────────────────────────────────────────────
function buildCronograma() {
  const html = DATA.cronograma.map(c=>`
    <div class="crono-item">
      <div class="crono-head">
        <div><div class="crono-ref">${c.nome} — ${c.inv}</div><div class="crono-sub">${c.obs||'Saldo: '+fmt(c.saldo,c.moeda)}</div></div>
        <span class="badge ${c.moeda==='RMB'?'badge-amber':'badge-blue'}">${c.moeda}</span>
      </div>
      <div class="crono-vals">
        <div class="crono-box"><div class="cl">30% — vence</div><div class="cv">${fmt(c.val30,c.moeda)}</div><div class="cd">${fmtDate(c.data30)}</div></div>
        <div class="crono-box"><div class="cl">70% — vence</div><div class="cv">${fmt(c.val70,c.moeda)}</div><div class="cd">${fmtDate(c.data70)}</div></div>
      </div>
    </div>`).join('');
  document.getElementById('sec-cronograma').innerHTML = `<div style="height:12px"></div>${syncBar()}<div class="section-title">Próximos vencimentos</div>${html}`;
}

// ── EMBARQUES ────────────────────────────────────────────────────────────────
function buildEmbarques() {
  const html = DATA.embarques.map(e=>{
    const c=COLORS[e.cod]||COLORS.HSN;
    const statColor={'Finalizado':'var(--green-text)','Embarcado':'var(--blue-text)','Cancelado':'var(--red-text)'};
    const sc = Object.entries(statColor).find(([k])=>e.status.includes(k));
    return `
    <div class="emb-item">
      <div style="display:flex;justify-content:space-between;align-items:flex-start;margin-bottom:6px">
        <div>
          <div class="emb-ref">${e.nome} · ${e.inv}</div>
          <div class="emb-sub">${e.filial||''}${e.refMex?' · '+e.refMex:''}</div>
        </div>
        <span style="font-size:11px;font-weight:600;color:${sc?sc[1]:'var(--text3)'}">${e.status}</span>
      </div>
      ${e.descricao?`<div style="font-size:11px;color:var(--text2);margin-bottom:8px;line-height:1.5">${e.descricao.substring(0,120)}${e.descricao.length>120?'...':''}</div>`:''}
      <div class="emb-dates">
        <div class="emb-dt"><div class="dl">Prontidão</div><div class="dv">${fmtDate(e.prontidao)||'—'}</div></div>
        <div class="emb-dt"><div class="dl">ETD</div><div class="dv">${fmtDate(e.etd)||'—'}</div></div>
        <div class="emb-dt"><div class="dl">ETA</div><div class="dv">${fmtDate(e.eta)||'—'}</div></div>
      </div>
    </div>`;
  }).join('');
  document.getElementById('sec-embarques').innerHTML = `<div style="height:12px"></div>${syncBar()}<div class="section-title">Embarques (${DATA.embarques.length})</div>${html}`;
}

// ── BUSCA ────────────────────────────────────────────────────────────────────
function doSearch(q) {
  const el = document.getElementById('search-results');
  q = q.trim().toLowerCase();
  if(!q){el.innerHTML='<p style="color:var(--text3);font-size:13px;text-align:center;padding:30px 0">Digite para buscar</p>';return;}
  const results=[];
  DATA.fornecedores.forEach(f=>{
    if(f.nome.toLowerCase().includes(q)||f.cod.toLowerCase().includes(q)||(f.produto||'').toLowerCase().includes(q)){
      const peds=DATA.pedidos.filter(p=>p.cod===f.cod);
      const sU=peds.reduce((s,p)=>s+p.saldoUSD,0);
      const sR=peds.reduce((s,p)=>s+p.saldoRMB,0);
      results.push(`<div class="result-item"><div class="result-tag">Fornecedor</div><div class="result-title">${f.nome} (${f.cod})</div><div class="result-sub">${statusBadge(f.status)} · Saldo R$ ${Math.round(sU*5.4+sR*0.75).toLocaleString('pt-BR')}</div></div>`);
    }
  });
  DATA.pedidos.forEach(p=>{
    if(p.inv.toLowerCase().includes(q)||(p.obs||'').toLowerCase().includes(q)){
      results.push(`<div class="result-item"><div class="result-tag">Pedido</div><div class="result-title">${p.inv}</div><div class="result-sub">${p.nome} · Total: ${p.valorUSD?fmt(p.valorUSD):fmt(p.valorRMB,'RMB')} · <span class="${(p.saldoUSD||p.saldoRMB)>0?'saldo-due':'saldo-ok'}">Saldo: ${p.saldoUSD?fmt(p.saldoUSD):fmt(p.saldoRMB,'RMB')}</span></div></div>`);
    }
  });
  DATA.pagamentos.forEach(p=>{
    if(p.inv.toLowerCase().includes(q)||p.nome.toLowerCase().includes(q)){
      results.push(`<div class="result-item"><div class="result-tag">Pagamento</div><div class="result-title">${fmt(p.valor,p.moeda)} · ${fmtDate(p.data)}</div><div class="result-sub">${p.nome} · ${p.inv}${p.tipo?' · '+p.tipo:''}</div></div>`);
    }
  });
  DATA.embarques.forEach(e=>{
    if(e.inv.toLowerCase().includes(q)||(e.refMex||'').toLowerCase().includes(q)||(e.descricao||'').toLowerCase().includes(q)){
      results.push(`<div class="result-item"><div class="result-tag">Embarque</div><div class="result-title">${e.inv}</div><div class="result-sub">${e.nome} · ${e.status} · ETA: ${fmtDate(e.eta)}</div></div>`);
    }
  });
  el.innerHTML=results.length?results.join(''):'<div style="text-align:center;padding:40px 20px;color:var(--text3)"><i class="ti ti-search-off" style="font-size:32px;opacity:.3"></i><p style="margin-top:8px">Nenhum resultado</p></div>';
}

// ── MAIN ──────────────────────────────────────────────────────────────────────
function toggleCard(h){h.parentElement.classList.toggle('expanded');}
function setTab(n){
  document.querySelectorAll('.section').forEach(s=>s.classList.remove('active'));
  document.querySelectorAll('.tab').forEach(t=>t.classList.remove('active'));
  document.getElementById('sec-'+n).classList.add('active');
  event.currentTarget.classList.add('active');
}

function showConfigBanner(msg) {
  document.getElementById('sec-resumo').innerHTML = `
    <div style="height:12px"></div>
    <div class="config-banner">
      <h2><i class="ti ti-settings"></i> Configurar planilha</h2>
      <p>${msg||'Cole o ID da sua planilha Google Sheets abaixo para conectar o app.'}</p>
      <input type="text" id="sheet-id-input" placeholder="Ex: 1BxiMVs0XRA5nFMdKvBdBZjgmUUqptlbs74OgVE2upms" value="${SHEET_ID!=='SEU_SHEET_ID_AQUI'?SHEET_ID:''}">
      <button onclick="saveSheetId()">Conectar e carregar dados</button>
    </div>
    <div style="padding:16px;background:var(--surface);border-radius:var(--radius);border:.5px solid var(--border);margin-top:4px">
      <p style="font-size:12px;font-weight:600;margin-bottom:8px">Como encontrar o ID:</p>
      <p style="font-size:12px;color:var(--text2);line-height:1.7">
        1. Abra sua planilha no Google Sheets<br>
        2. Veja a URL: <code style="font-size:11px;background:var(--surface2);padding:1px 4px;border-radius:4px">docs.google.com/spreadsheets/d/<b>ESTE_É_O_ID</b>/edit</code><br>
        3. Cole o ID acima e clique em Conectar
      </p>
    </div>`;
}

function saveSheetId() {
  const id = document.getElementById('sheet-id-input').value.trim();
  if(!id){alert('Cole o ID da planilha');return;}
  localStorage.setItem('bcf_sheet_id',id);
  location.reload();
}

async function reload() {
  try {
    await loadAllData();
    buildResumo(); buildFornecedores(); buildPagamentos(); buildCronograma(); buildEmbarques();
    const t = lastSync.toLocaleTimeString('pt-BR',{hour:'2-digit',minute:'2-digit'});
    document.getElementById('app-sub').textContent = `Extrapower · sync ${t}`;
  } catch(e) {
    showConfigBanner('Erro ao carregar: '+e.message);
  }
}

async function init() {
  if(SHEET_ID==='SEU_SHEET_ID_AQUI'){showConfigBanner();return;}
  try {
    await loadAllData();
    buildResumo(); buildFornecedores(); buildPagamentos(); buildCronograma(); buildEmbarques();
    const t = lastSync.toLocaleTimeString('pt-BR',{hour:'2-digit',minute:'2-digit'});
    document.getElementById('app-sub').textContent = `Extrapower · sync ${t}`;
  } catch(e){
    showConfigBanner('Não foi possível conectar à planilha. Verifique o ID e se ela está publicada publicamente.<br><br>Erro: '+e.message);
  }
}

init();
</script>
</body>
</html>
