<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>Jackal Den — DEN OF FIRE ARMS</title>
<link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700&family=Roboto&display=swap" rel="stylesheet">
<style>
    :root{--bg:#0b0b0b;--card:#0f1113;--accent:#f5a623;--accent-2:#f24e1e;--muted:#9aa3ad;--glass:rgba(255,255,255,0.03)}
    *{box-sizing:border-box} body{margin:0;font-family:Roboto,Arial,sans-serif;background:
    radial-gradient(900px 600px at 10% 10%, rgba(242,78,30,0.06), transparent 6%),
    linear-gradient(180deg,#040405,#0b0b0b);color:#fff}
    header.site{display:flex;align-items:center;justify-content:space-between;padding:14px 20px;border-bottom:1px solid rgba(255,255,255,0.03);position:sticky;top:0;background:linear-gradient(90deg, rgba(0,0,0,0.65), rgba(0,0,0,0.12));z-index:50}
    .brand{display:flex;gap:12px;align-items:center}.logo{width:64px;height:64px;border-radius:12px;background:linear-gradient(135deg,var(--accent),var(--accent-2));display:flex;align-items:center;justify-content:center;font-family:Orbitron;font-weight:700;color:#0b0b0b;box-shadow:0 6px 18px rgba(242,78,30,0.12), inset 0 -6px 18px rgba(0,0,0,0.12)}
    h1{margin:0;font-size:1.05rem;font-family:Orbitron} nav.top{display:flex;gap:10px;align-items:center}
    nav.top a{color:var(--muted);text-decoration:none;padding:8px 12px;border-radius:8px;font-size:0.95rem} nav.top a.active,nav.top a:hover{background:var(--glass);color:#fff}
    .contact{font-size:0.86rem;color:var(--muted)} main{padding:22px}
    .hero{display:flex;gap:18px;align-items:flex-start;margin-bottom:18px}
    .left{flex:1;max-width:760px;background:linear-gradient(180deg, rgba(255,255,255,0.01), transparent);padding:18px;border-radius:12px;border:1px solid rgba(255,255,255,0.02)}
    .tag{display:inline-block;padding:6px 10px;border-radius:999px;background:rgba(242,78,30,0.08);color:var(--accent-2);font-weight:700;margin-bottom:8px}
    .sub{color:var(--muted);font-size:0.95rem} .actions{margin-top:12px;display:flex;gap:10px}
    .btn{background:var(--accent);color:#0b0b0b;border:none;padding:10px 14px;border-radius:8px;cursor:pointer;font-weight:700}
    .btn.ghost{background:transparent;color:var(--muted);border:1px solid rgba(255,255,255,0.03)}
    .layout{display:grid;grid-template-columns:300px 1fr;gap:20px;align-items:start;margin-top:18px}
    .sidebar{background:linear-gradient(180deg, rgba(255,255,255,0.01), transparent);padding:14px;border-radius:12px;border:1px solid rgba(255,255,255,0.03)}
    .section-title{font-size:0.95rem;color:var(--muted);margin-bottom:8px}
    .content-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(260px,1fr));gap:16px}
    .card{background:var(--card);padding:12px;border-radius:10px;border:1px solid rgba(255,255,255,0.02)}
    .card img.gun{width:100%;height:160px;object-fit:cover;border-radius:8px}
    .card img.pellet{width:92px;height:60px;object-fit:cover;border-radius:6px;border:1px solid rgba(255,255,255,0.04);margin-top:8px}
    .card h3{margin:10px 0 6px 0;font-size:1rem} .input,select{width:100%;padding:8px;margin-top:8px;border-radius:8px;border:1px solid rgba(255,255,255,0.06);background:transparent;color:#fff}
    .small{font-size:0.86rem;color:var(--muted)} .filters{display:flex;gap:8px;margin-bottom:12px;flex-wrap:wrap}
    .pill{background:rgba(255,255,255,0.02);padding:6px 10px;border-radius:999px;color:var(--muted);cursor:pointer}
    .pill.active{background:var(--accent-2);color:#0b0b0b} footer{margin-top:18px;text-align:center;color:var(--muted);padding:16px 0}
    @media(max-width:980px){.layout{grid-template-columns:1fr}.hero{flex-direction:column}}
</style>
</head>
<body>
    <header class="site">
        <div class="brand">
            <div class="logo">JCKL</div>
            <div>
                <h1>Jackal Den — DEN OF FIRE ARMS</h1>
                <div class="contact">Owner: <strong style="color:var(--accent)">CHAUDARY HAMZA</strong> · <span class="small">jackal edition</span></div>
            </div>
        </div>

        <nav class="top" aria-label="Main menu">
            <a href="#" data-target="home" class="active">Home</a>
            <a href="#" data-target="guns">Guns</a>
            <a href="#" data-target="bullets">Bullets</a>
            <a href="#" data-target="orders">Orders</a>
            <a href="#" id="loginBtn">Login</a>
        </nav>

        <div class="contact">📧 25-se-081@student.hitecuni.edu.pk</div>
    </header>

    <main>
        <section class="hero">
            <div class="left">
                <div class="tag">JACKAL EDITION</div>
                <h2 style="margin:6px 0;font-family:Orbitron">Predator-grade Airguns — stealth | precision | power</h2>
                <p class="sub">A Jackal-themed storefront demo. Images are public placeholders (picsum.photos). Replace URLs with your own photos when ready.</p>
                <div class="actions">
                    <button class="btn" id="showGuns">Browse The Den</button>
                    <button class="btn ghost" id="showOrders">Orders</button>
                </div>
            </div>

            <div style="width:340px">
                <div class="card">
                    <h3 style="margin:0 0 8px 0">Quick Editor</h3>
                    <div class="small">Edit demo price/delivery; saved locally</div>
                    <input id="editSku" class="input" placeholder="SKU (gun-001)" />
                    <input id="editPrice" class="input" placeholder="Price (e.g., 1200 USD)" />
                    <select id="editDelivery" class="input"><option>Standard</option><option>Express</option><option>Pickup</option></select>
                    <div style="display:flex;gap:8px;margin-top:8px">
                        <button class="btn" id="saveBtn">Save</button>
                        <button class="btn ghost" id="resetBtn">Reset Local</button>
                    </div>
                </div>
            </div>
        </section>

        <div class="layout">
            <aside class="sidebar">
                <div class="section-title">Filters</div>
                <div class="filters" id="topFilters">
                    <div class="pill active" data-filter="all">All</div>
                    <div class="pill" data-filter="hunting">Hunting</div>
                    <div class="pill" data-filter="target">Target</div>
                    <div class="pill" data-filter="tactical">Tactical</div>
                    <div class="pill" data-filter="plinking">Plinking</div>
                </div>

                <div style="margin-top:14px">
                    <div class="section-title">Range</div>
                    <div class="filters" id="rangeFilters">
                        <div class="pill active" data-range="all">Show All</div>
                        <div class="pill" data-range="0-20">0–20m</div>
                        <div class="pill" data-range="20-50">20–50m</div>
                        <div class="pill" data-range="50-100">50–100m</div>
                        <div class="pill" data-range="100+">100m+</div>
                    </div>
                </div>

                <div style="margin-top:14px">
                    <div class="section-title">Contact</div>
                    <div class="small">Owner: CHAURADY HAMZA</div>
                    <div class="small">Phone: +92 332 5534567</div>
                </div>
            </aside>

            <section class="main-content">
                <div id="panel-home" class="panel">
                    <h2 style="margin-top:0">Featured</h2>
                    <div class="content-grid" id="gunsGrid"></div>
                </div>

                <div id="panel-guns" class="panel" style="display:none">
                    <h2>Jackal Den — Guns (60)</h2>
                    <div style="margin:12px 0;display:flex;gap:8px;align-items:center;flex-wrap:wrap">
                        <input id="searchBox" class="input" placeholder="Search by name or SKU" />
                        <select id="sortSelect" class="input" style="max-width:180px"><option value="default">Sort: Featured</option><option value="price-asc">Price ↑</option><option value="price-desc">Price ↓</option></select>
                    </div>
                    <div id="gunsList" class="content-grid"></div>
                </div>

                <div id="panel-bullets" class="panel" style="display:none">
                    <h2>Bullets</h2>
                    <div class="card small">Common pellet sizes: .177 (4.5), .22 (5.5), .25 (6.35), .30 (7.62)</div>
                </div>

                <div id="panel-orders" class="panel" style="display:none">
                    <h2>Orders</h2>
                    <div class="card">
                        <table id="ordersTable" style="width:100%;border-collapse:collapse"><thead><tr><th>Order ID</th><th>SKU</th><th>Model</th><th>Price</th><th>Delivery</th></tr></thead><tbody></tbody></table>
                    </div>
                </div>
            </section>
        </div>

        <footer>&copy; <span id="year"></span> Jackal Den — DEN OF FIRE ARMS</footer>
    </main>

<script>
document.getElementById('year').textContent = new Date().getFullYear();

// Use picsum.photos placeholder images for immediate display.
// You can replace any url below with your own CDN or repo URL later.
const gunsData = [];
for(let i=1;i<=60;i++){
    const id = String(i).padStart(3,'0');
    // unique picsum seed per image so they differ
    const gunUrl = `https://picsum.photos/seed/jackal-gun-${id}/900/600`;
    const pelletTypes = ['https://picsum.photos/seed/pellet-177/300/200','https://picsum.photos/seed/pellet-22/300/200','https://picsum.photos/seed/pellet-25/300/200','https://picsum.photos/seed/pellet-30/300/200','https://picsum.photos/seed/pellet-bb/300/200'];
    const pellet = pelletTypes[i % pelletTypes.length];
    gunsData.push({
        sku: 'gun-'+id,
        name: 'Jackal Series '+id,
        category: (i%4===0)?'tactical': (i%4===1)?'hunting': (i%4===2)?'target':'plinking',
        range: (i%4===0)?'50-100': (i%4===1)?'100-200': (i%4===2)?'20-50':'0-20',
        price: (300 + i*15) + ' USD',
        delivery: (i%3===0)?'Express':'Standard',
        img: gunUrl,
        pellet_size: (i%5===1)?'4.5 mm (.177)': (i%5===2)?'5.5 mm (.22)': (i%5===3)?'6.35 mm (.25)': (i%5===4)?'7.62 mm (.30)':'4.5 mm BB',
        pellet_image: pellet
    });
}

const localEdits = JSON.parse(localStorage.getItem('jackal_local_edits') || '{}');
const demoOrders = JSON.parse(localStorage.getItem('jackal_orders') || '[]');

function applyLocalEdits(item){ return localEdits[item.sku] ? {...item, ...localEdits[item.sku]} : item; }

function makeCard(item){
    const it = applyLocalEdits(item);
    const div = document.createElement('div'); div.className = 'card';
    div.innerHTML = `
        <img class="gun" src="${it.img}" alt="${it.name}" loading="lazy" onerror="this.style.opacity=0.5">
        <h3>${it.name}</h3>
        <div class="small">SKU: ${it.sku} · ${it.range}</div>
        <div style="display:flex;gap:10px;align-items:center;margin-top:8px">
            <img class="pellet" src="${it.pellet_image}" alt="${it.pellet_size}" loading="lazy" onerror="this.style.opacity=0.5">
            <div style="flex:1">
                <div class="small">Pellet: <strong>${it.pellet_size}</strong></div>
                <input class="input priceInput" data-sku="${it.sku}" value="${it.price}">
                <select class="input deliverySelect" data-sku="${it.sku}">
                    <option ${it.delivery==='Standard'?'selected':''}>Standard</option>
                    <option ${it.delivery==='Express'?'selected':''}>Express</option>
                    <option ${it.delivery==='Pickup'?'selected':''}>Pickup</option>
                </select>
            </div>
        </div>
        <div style="display:flex;gap:8px;margin-top:10px">
            <button class="btn saveLocal" data-sku="${it.sku}">Save</button>
            <button class="btn ghost viewBtn" data-sku="${it.sku}">View</button>
            <button class="btn ghost orderBtn" data-sku="${it.sku}">Order</button>
        </div>
    `;
    return div;
}

function renderGrid(list){ const grid = document.getElementById('gunsGrid'); grid.innerHTML=''; list.forEach(i=>grid.appendChild(makeCard(i))); attachCardHandlers(); }
function renderList(list){ const listEl = document.getElementById('gunsList'); listEl.innerHTML=''; list.forEach(i=>listEl.appendChild(makeCard(i))); attachCardHandlers(); }

renderGrid(gunsData.slice(0,12));
renderList(gunsData);

function attachCardHandlers(){
    document.querySelectorAll('.saveLocal').forEach(btn=>{
        btn.onclick = () => {
            const sku = btn.dataset.sku;
            const price = document.querySelector('.priceInput[data-sku="'+sku+'"]').value;
            const delivery = document.querySelector('.deliverySelect[data-sku="'+sku+'"]').value;
            localEdits[sku] = {price, delivery};
            localStorage.setItem('jackal_local_edits', JSON.stringify(localEdits));
            alert('Saved locally for '+sku);
        };
    });
    document.querySelectorAll('.viewBtn').forEach(b=>{
        b.onclick = () => {
            const sku = b.dataset.sku; const item = gunsData.find(x=>x.sku===sku); const edit = localEdits[sku] || {};
            alert(item.name + '\nSKU: '+item.sku+'\nPrice: '+(edit.price||item.price)+'\nDelivery: '+(edit.delivery||item.delivery));
        };
    });
    document.querySelectorAll('.orderBtn').forEach(b=>{
        b.onclick = () => {
            const sku = b.dataset.sku; const item = gunsData.find(x=>x.sku===sku); const edit = localEdits[sku] || {};
            const price = edit.price||item.price; const delivery = edit.delivery||item.delivery;
            const orderId = 'JORD-'+Math.random().toString(36).slice(2,8).toUpperCase();
            const order = {id:orderId, sku:item.sku, model:item.name, price, delivery};
            demoOrders.push(order); localStorage.setItem('jackal_orders', JSON.stringify(demoOrders)); renderOrders(); alert('Order placed: '+orderId);
        };
    });
}

function showPanel(name){
    document.querySelectorAll('nav.top a').forEach(a=>a.classList.remove('active'));
    document.querySelectorAll('nav.top a[data-target="'+name+'"]').forEach(a=>a.classList.add('active'));
    document.querySelectorAll('.panel').forEach(p=>p.style.display='none');
    const panel = document.getElementById('panel-'+name);
    if(panel) panel.style.display='block'; else document.getElementById('panel-home').style.display='block';
}
document.querySelectorAll('nav.top a').forEach(a=>a.addEventListener('click', e=>{ e.preventDefault(); showPanel(a.dataset.target); }));
document.getElementById('showGuns').onclick = ()=> showPanel('guns'); document.getElementById('showOrders').onclick = ()=> showPanel('orders');

document.getElementById('searchBox').addEventListener('input', e=>{
    const q = e.target.value.toLowerCase();
    renderList(gunsData.filter(g=> g.name.toLowerCase().includes(q) || g.sku.toLowerCase().includes(q)));
});
document.getElementById('sortSelect').addEventListener('change', e=>{
    let arr = [...gunsData];
    if(e.target.value==='price-asc') arr.sort((a,b)=> parseInt(a.price) - parseInt(b.price));
    if(e.target.value==='price-desc') arr.sort((a,b)=> parseInt(b.price) - parseInt(a.price));
    renderList(arr);
});

document.getElementById('saveBtn').addEventListener('click', ()=>{
    const sku = document.getElementById('editSku').value.trim(); const price = document.getElementById('editPrice').value.trim(); const delivery = document.getElementById('editDelivery').value;
    if(!sku) return alert('Enter SKU'); localEdits[sku] = {price, delivery}; localStorage.setItem('jackal_local_edits', JSON.stringify(localEdits)); alert('Saved '+sku);
    renderGrid(gunsData.slice(0,12)); renderList(gunsData);
});
document.getElementById('resetBtn').addEventListener('click', ()=>{ if(confirm('Clear local edits?')){ localStorage.removeItem('jackal_local_edits'); location.reload(); } });

function renderOrders(){ const tb = document.querySelector('#ordersTable tbody'); tb.innerHTML=''; const orders = demoOrders.length ? demoOrders : [{id:'JORD-01',sku:'gun-001',model:'Jackal Series 001',price:'315 USD',delivery:'Standard'}]; orders.forEach(o=>{ const tr=document.createElement('tr'); tr.innerHTML=`<td>${o.id}</td><td>${o.sku}</td><td>${o.model}</td><td>${o.price}</td><td>${o.delivery}</td>`; tb.appendChild(tr); }); }
renderOrders();
</script>
</body>
</html>



