<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JonilsonVPN | Downloads</title>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { font-family: 'Plus Jakarta Sans', sans-serif; background: #0a0c15; color: #fff; overflow-x: hidden; }
        .gradient-bg { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -2; background: radial-gradient(circle at 20% 30%, #0f172a, #030614); }
        .container { max-width: 1400px; margin: 0 auto; padding: 2rem; position: relative; z-index: 2; }
        .hero { text-align: center; margin-bottom: 3rem; }
        .logo-wrapper { display: inline-flex; align-items: center; gap: 16px; background: rgba(15,25,45,0.6); backdrop-filter: blur(12px); padding: 1rem 2.5rem; border-radius: 100px; border: 1px solid rgba(56,189,248,0.4); margin-bottom: 1.5rem; }
        .logo-icon { font-size: 2.5rem; color: #38bdf8; }
        .logo-wrapper h1 { font-size: 2.2rem; font-weight: 800; background: linear-gradient(135deg, #fff, #38bdf8, #a855f7); -webkit-background-clip: text; background-clip: text; color: transparent; }
        .badge { display: inline-block; background: rgba(56,189,248,0.15); padding: 0.5rem 1.2rem; border-radius: 40px; font-size: 0.85rem; border: 1px solid rgba(56,189,248,0.3); }
        .info-banner { background: linear-gradient(135deg, rgba(56,189,248,0.15), rgba(168,85,247,0.15)); border: 1px solid rgba(56,189,248,0.4); border-radius: 24px; padding: 1.5rem; margin: 1.5rem 0; text-align: center; }
        .info-banner h2 { font-size: 1.3rem; margin-bottom: 0.8rem; color: #38bdf8; }
        .info-banner .highlight { display: flex; gap: 1rem; flex-wrap: wrap; justify-content: center; margin-top: 1rem; }
        .info-banner .highlight span { background: rgba(0,0,0,0.4); padding: 0.4rem 1rem; border-radius: 40px; font-size: 0.85rem; }
        .stats { display: flex; justify-content: center; gap: 2rem; margin: 2rem 0; flex-wrap: wrap; }
        .stat-item { background: rgba(255,255,255,0.03); padding: 0.6rem 1.5rem; border-radius: 60px; }
        .stat-number { font-weight: 800; font-size: 1.3rem; color: #38bdf8; }
        .downloads-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(340px, 1fr)); gap: 2rem; margin: 3rem 0; }
        .card { background: rgba(18,25,45,0.65); backdrop-filter: blur(16px); border-radius: 32px; border: 1px solid rgba(56,189,248,0.2); overflow: hidden; transition: all 0.4s ease; }
        .card:hover { transform: translateY(-8px); border-color: rgba(56,189,248,0.5); }
        .card-header { padding: 1.8rem 1.8rem 1rem; display: flex; align-items: center; gap: 15px; }
        .card-icon { width: 55px; height: 55px; background: linear-gradient(135deg, rgba(56,189,248,0.2), rgba(168,85,247,0.2)); border-radius: 20px; display: flex; align-items: center; justify-content: center; font-size: 1.8rem; color: #38bdf8; }
        .card-header h3 { font-size: 1.4rem; font-weight: 700; }
        .card-body { padding: 0 1.8rem 1.5rem; }
        .file-meta { display: flex; gap: 15px; margin-bottom: 1rem; font-size: 0.75rem; color: #94a3b8; }
        .file-meta span { background: rgba(0,0,0,0.3); padding: 4px 12px; border-radius: 20px; }
        .description { color: #cbd5e1; line-height: 1.5; font-size: 0.9rem; margin-bottom: 1.5rem; }
        .btn-download { display: inline-flex; align-items: center; justify-content: center; gap: 12px; width: 100%; padding: 14px 0; background: linear-gradient(90deg, #1e293b, #0f172a); border: 1.5px solid rgba(56,189,248,0.5); border-radius: 60px; color: white; font-weight: 700; text-decoration: none; transition: all 0.3s; }
        .btn-download:hover { background: linear-gradient(90deg, #38bdf8, #a855f7); }
        .whatsapp-float { position: fixed; bottom: 30px; right: 30px; z-index: 1000; }
        .whatsapp-float a { display: flex; align-items: center; justify-content: center; width: 70px; height: 70px; background: linear-gradient(135deg, #25d366, #128C7E); border-radius: 50%; text-decoration: none; animation: pulse 2s infinite; }
        .whatsapp-float i { font-size: 2.5rem; color: white; }
        @keyframes pulse { 0% { box-shadow: 0 0 0 0 rgba(37,211,102,0.4); } 70% { box-shadow: 0 0 0 15px rgba(37,211,102,0); } 100% { box-shadow: 0 0 0 0 rgba(37,211,102,0); } }
        .whatsapp-header { display: inline-flex; align-items: center; gap: 8px; background: linear-gradient(135deg, #25d366, #128C7E); padding: 0.6rem 1.2rem; border-radius: 60px; margin-top: 1rem; text-decoration: none; color: white; font-weight: 600; }
        .admin-section { margin-top: 4rem; background: rgba(0,0,0,0.5); backdrop-filter: blur(20px); border-radius: 40px; border: 1px solid rgba(168,85,247,0.3); overflow: hidden; }
        .admin-header { display: flex; justify-content: space-between; align-items: center; padding: 1.2rem 2rem; background: rgba(168,85,247,0.1); cursor: pointer; }
        .admin-header h3 { color: #c084fc; }
        .admin-panel { max-height: 0; overflow: hidden; transition: max-height 0.5s; padding: 0 2rem; }
        .admin-panel.open { max-height: 800px; padding: 2rem; }
        .form-row { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 1rem; }
        .form-group { margin-bottom: 1rem; }
        input, textarea { width: 100%; padding: 12px 18px; background: #0f172a; border: 1px solid #334155; border-radius: 24px; color: white; font-family: inherit; }
        .btn-admin { background: linear-gradient(90deg, #7c3aed, #a855f7); border: none; padding: 12px 28px; border-radius: 40px; color: white; font-weight: 600; cursor: pointer; margin-right: 12px; margin-top: 8px; }
        .btn-admin-danger { background: linear-gradient(90deg, #dc2626, #ef4444); }
        .links-preview { margin-top: 1.5rem; background: #0a0f1a; border-radius: 24px; padding: 1rem; }
        .preview-item { display: flex; justify-content: space-between; align-items: center; padding: 0.8rem; border-bottom: 1px solid #1e293b; }
        .delete-item { background: none; border: none; color: #f87171; font-size: 1.2rem; cursor: pointer; }
        .empty-state { text-align: center; padding: 3rem; background: rgba(0,0,0,0.3); border-radius: 32px; }
        .footer { text-align: center; margin-top: 4rem; padding: 2rem; font-size: 0.8rem; color: #64748b; }
        @media (max-width: 768px) { .container { padding: 1rem; } .logo-wrapper h1 { font-size: 1.5rem; } .whatsapp-float a { width: 55px; height: 55px; } .whatsapp-float i { font-size: 2rem; } }
    </style>
</head>
<body>
<div class="gradient-bg"></div>
<div class="container">
    <div class="hero">
        <div class="logo-wrapper"><i class="fas fa-shield-haltered logo-icon"></i><h1>JonilsonVPN</h1></div>
        <div class="badge"><i class="fas fa-link"></i> Apps Modificados | VPN | Downloads Seguros</div>
        <div class="info-banner">
            <h2>📱 Sobre este site</h2>
            <p>Site criado para baixar <strong>aplicativos modificados</strong>, <strong>arquivos de VPN</strong> e <strong>clientes VPN</strong> com segurança.</p>
            <div class="highlight"><span><i class="fas fa-mobile-alt"></i> Apps Modificados</span><span><i class="fas fa-shield-vpn"></i> Arquivos VPN</span><span><i class="fas fa-globe"></i> Clientes VPN</span></div>
        </div>
        <div><a href="https://wa.me/244923505559?text=Ol%C3%A1%20Jonilson" target="_blank" class="whatsapp-header"><i class="fab fa-whatsapp"></i> Suporte WhatsApp</a></div>
        <div class="stats"><div class="stat-item"><span class="stat-number" id="fileCount">0</span> Arquivos</div><div class="stat-item"><i class="fas fa-shield-alt"></i> Seguro</div><div class="stat-item"><i class="fas fa-headset"></i> Suporte</div></div>
    </div>
    <div id="downloadsGrid" class="downloads-grid"></div>
    <div class="admin-section">
        <div class="admin-header" id="adminToggle"><h3><i class="fas fa-crown"></i> 🔐 Painel Admin</h3><i class="fas fa-chevron-down" id="adminIcon"></i></div>
        <div class="admin-panel" id="adminPanel">
            <div class="form-row">
                <div class="form-group"><label>Título</label><input type="text" id="fileTitle" placeholder="Ex: VPN Pro Mod"></div>
                <div class="form-group"><label>Ícone</label><input type="text" id="fileIcon" value="fa-shield-vpn"></div>
            </div>
            <div class="form-group"><label>Descrição</label><textarea id="fileDesc" rows="2" placeholder="Descrição..."></textarea></div>
            <div class="form-row">
                <div class="form-group"><label>Link MediaFire</label><input type="text" id="mediafireLink" placeholder="https://www.mediafire.com/file/..."></div>
                <div class="form-group"><label>Tamanho</label><input type="text" id="fileSize" placeholder="Ex: 25 MB"></div>
            </div>
            <div><button class="btn-admin" id="addFileBtn">+ Adicionar</button><button class="btn-admin btn-admin-danger" id="clearAllBtn">🗑️ Remover Todos</button></div>
            <div class="links-preview"><h4>📋 Links Ativos</h4><div id="linksPreviewList"></div></div>
        </div>
    </div>
    <div class="footer">JonilsonVPN © 2025 - Apps Modificados e VPN</div>
</div>
<div class="whatsapp-float"><a href="https://wa.me/244923505559?text=Ol%C3%A1%20Jonilson" target="_blank"><i class="fab fa-whatsapp"></i></a></div>
<script>
    const STORAGE_KEY='jonilsonvpn_links';
    let downloads=[];
    function loadData(){const s=localStorage.getItem(STORAGE_KEY);downloads=s?JSON.parse(s):[];renderUI();updateStats();}
    function saveData(){localStorage.setItem(STORAGE_KEY,JSON.stringify(downloads));renderUI();updateStats();}
    function updateStats(){document.getElementById('fileCount').innerText=downloads.length;}
    function escapeHtml(s){if(!s)return'';return s.replace(/[&<>]/g,function(m){if(m==='&')return'&amp;';if(m==='<')return'&lt;';if(m==='>')return'&gt;';return m;});}
    function renderUI(){
        const g=document.getElementById('downloadsGrid');
        if(!downloads.length){g.innerHTML='<div class="empty-state"><i class="fas fa-folder-open fa-4x" style="color:#38bdf8;"></i><h3>Nenhum link</h3><p>Use o painel admin para adicionar links.</p></div>';}
        else{g.innerHTML=downloads.map(f=>`<div class="card"><div class="card-header"><div class="card-icon"><i class="fas ${f.icon||'fa-download'}"></i></div><h3>${escapeHtml(f.title)}</h3></div><div class="card-body"><div class="file-meta"><span><i class="fas fa-weight-hanging"></i> ${escapeHtml(f.fileSize||'Tamanho não informado')}</span><span><i class="fas fa-cloud"></i> MediaFire</span></div><div class="description">${escapeHtml(f.description||'Arquivo disponível')}</div><a href="${f.mediafireUrl.replace(/&/g,'&amp;').replace(/"/g,'&quot;')}" target="_blank" class="btn-download"><i class="fas fa-external-link-alt"></i> ABRIR LINK</a></div></div>`).join('');}
        const p=document.getElementById('linksPreviewList');
        if(p){if(!downloads.length){p.innerHTML='<div style="padding:1rem;color:#64748b;">Nenhum link cadastrado.</div>';}
        else{p.innerHTML=downloads.map(f=>`<div class="preview-item"><div><strong>${escapeHtml(f.title)}</strong><br><small>${escapeHtml(f.mediafireUrl?.substring(0,50)||'')}</small></div><button class="delete-item" data-id="${f.id}"><i class="fas fa-trash-alt"></i></button></div>`).join('');
        document.querySelectorAll('.delete-item').forEach(b=>{b.addEventListener('click',()=>{const id=b.getAttribute('data-id');if(confirm('Remover?')){downloads=downloads.filter(f=>f.id!==id);saveData();}});});}}
    }
    function addNewFile(){
        const t=document.getElementById('fileTitle').value.trim();
        let i=document.getElementById('fileIcon').value.trim();
        const d=document.getElementById('fileDesc').value.trim();
        const u=document.getElementById('mediafireLink').value.trim();
        const s=document.getElementById('fileSize').value.trim();
        if(!t){alert('Digite um título.');return;}
        if(!u){alert('Cole o link do MediaFire.');return;}
        if(!i)i='fa-shield-vpn';
        if(!i.startsWith('fa-'))i='fa-'+i;
        downloads.unshift({id:Date.now().toString(),title:t,icon:i,description:d||'Arquivo disponível',mediafireUrl:u,fileSize:s||'Tamanho não informado'});
        saveData();
        document.getElementById('fileTitle').value='';document.getElementById('fileIcon').value='fa-shield-vpn';document.getElementById('fileDesc').value='';document.getElementById('mediafireLink').value='';document.getElementById('fileSize').value='';
        alert(`✅ "${t}" adicionado!`);
    }
    function clearAll(){if(downloads.length===0){alert('Nenhum link');return;}if(confirm('Remover TODOS os links?')){downloads=[];saveData();alert('Todos removidos.');}}
    document.getElementById('adminToggle')?.addEventListener('click',()=>{document.getElementById('adminPanel').classList.toggle('open');const ic=document.getElementById('adminIcon');ic.classList.toggle('fa-chevron-down');ic.classList.toggle('fa-chevron-up');});
    document.getElementById('addFileBtn')?.addEventListener('click',addNewFile);
    document.getElementById('clearAllBtn')?.addEventListener('click',clearAll);
    loadData();
</script>
</body>
</html>
