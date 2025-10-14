<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>EderConvert — Ultimate PDF & File Converter</title>
  <meta name="description" content="EderConvert: Convert Images, CSV, Text & Documents to PDF instantly. Merge, encrypt & download. Fast, secure, mobile-first." />
  <meta name="keywords" content="PDF converter, image to PDF, CSV to PDF, merge PDF, encrypt PDF, free PDF converter, EderConvert" />
  <link rel="canonical" href="https://www.ederconvert.com/" />

  <!-- Open Graph -->
  <meta property="og:title" content="EderConvert — Ultimate PDF & File Converter" />
  <meta property="og:description" content="Convert Images, CSV, Text & Documents to PDF instantly. Optional password, merge PDFs, client-side & server-ready." />
  <meta property="og:type" content="website" />
  <meta property="og:url" content="https://www.ederconvert.com/" />
  <meta property="og:image" content="https://www.ederconvert.com/og-image.png" />

  <!-- Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700;800&display=swap" rel="stylesheet">

  <style>
    :root{
      --bg:#f6f8fb; --card:#ffffff; --muted:#6b7280; --accent1:#4b6ef5; --accent2:#8b5cf6;
      --glass: rgba(255,255,255,0.6);
    }
    *{box-sizing:border-box}
    html,body{height:100%;margin:0;font-family:'Poppins',system-ui,Segoe UI,Roboto,Helvetica,Arial; background:var(--bg); color:#0f172a}

    /* Container */
    .wrap{max-width:1200px;margin:28px auto;padding:20px}

    /* Header */
    header{display:flex;align-items:center;justify-content:space-between;padding:18px;border-radius:12px;background:linear-gradient(90deg,var(--card),#fbfdff);box-shadow:0 6px 24px rgba(11,22,53,0.06)}
    .brand{display:flex;align-items:center;gap:12px}
    .logo-mark{width:44px;height:44px;border-radius:10px;background:linear-gradient(135deg,var(--accent1),var(--accent2));display:flex;align-items:center;justify-content:center;color:#fff;font-weight:800}
    .brand h1{margin:0;font-size:18px}
    .nav-actions{display:flex;gap:12px;align-items:center}
    .btn-outline{padding:8px 12px;border-radius:10px;border:1px solid rgba(11,22,53,0.06);background:transparent;cursor:pointer}
    .btn-primary{background:linear-gradient(90deg,var(--accent1),var(--accent2));color:#fff;padding:10px 14px;border-radius:12px;border:none;cursor:pointer;box-shadow:0 8px 30px rgba(75,110,245,0.18)}

    /* Hero */
    .hero{display:grid;grid-template-columns:1fr 420px;gap:28px;align-items:center;margin-top:22px}
    .hero-card{background:linear-gradient(180deg, rgba(255,255,255,0.85), rgba(255,255,255,0.95));padding:28px;border-radius:16px;box-shadow:0 10px 30px rgba(11,22,53,0.06)}
    .hero h2{margin:0 0 12px;font-size:30px}
    .hero p{color:var(--muted);margin:0 0 18px}
    .upload-area{display:flex;flex-direction:column;gap:10px;align-items:center}
    .file-input{width:100%;padding:12px;border-radius:10px;border:1px dashed #e6eefb;background:transparent;text-align:center}
    .small-muted{color:var(--muted);font-size:13px}

    /* Options */
    .options{margin-top:26px;display:grid;grid-template-columns:repeat(3,1fr);gap:16px}
    .card{background:var(--card);padding:18px;border-radius:12px;box-shadow:0 8px 30px rgba(12,16,29,0.04);cursor:pointer;transition:transform .18s ease, box-shadow .18s ease}
    .card:hover{transform:translateY(-8px);box-shadow:0 18px 40px rgba(12,16,29,0.08)}
    .card h4{margin:0 0 6px}
    .card small{color:var(--muted)}

    /* Right hero graphic */
    .hero-visual{background:linear-gradient(180deg, #ffffff, #fbfdff);padding:18px;border-radius:12px;display:flex;flex-direction:column;align-items:center;gap:12px}
    .doc-preview{width:100%;height:320px;border-radius:10px;background:linear-gradient(180deg,#f8fbff,#ffffff);display:flex;align-items:center;justify-content:center;box-shadow:inset 0 1px 0 rgba(255,255,255,0.6);}

    /* Merge section */
    .merge{margin-top:26px;padding:18px;border-radius:12px;background:linear-gradient(180deg,rgba(255,255,255,0.9),#fff);box-shadow:0 8px 20px rgba(11,22,53,0.04)}

    /* Modal */
    #workflowModal{position:fixed;inset:0;display:none;align-items:center;justify-content:center;background:linear-gradient(rgba(8,12,20,0.45),rgba(8,12,20,0.45));backdrop-filter: blur(4px);z-index:999}
    #workflowModal .modal{width:720px;max-width:94%;background:linear-gradient(180deg,#fff,#fbfdff);padding:20px;border-radius:14px;box-shadow:0 30px 60px rgba(3,8,23,0.5)}
    .modal-head{display:flex;align-items:center;justify-content:space-between;gap:8px}
    .modal-body{margin-top:12px}
    .input-file{display:block;width:100%;padding:12px;border-radius:10px;border:1px solid #eef2ff;background:#f8fbff}
    .modal-footer{display:flex;gap:10px;justify-content:flex-end;margin-top:14px}

    /* Footer */
    footer{margin-top:28px;text-align:center;color:var(--muted);font-size:13px}

    /* Responsive */
    @media (max-width:900px){
      .hero{grid-template-columns:1fr}
      .options{grid-template-columns:repeat(2,1fr)}
    }
    @media (max-width:520px){
      .options{grid-template-columns:1fr}
      .brand h1{font-size:16px}
      header{padding:12px}
    }
  </style>

  <!-- AdSense script (App ID) -->
  <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-app-pub-4191528661876815~8639241290" crossorigin="anonymous"></script>

  <!-- Libraries -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js" defer></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/pdf-lib/1.17.1/pdf-lib.min.js" defer></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/PapaParse/5.4.1/papaparse.min.js" defer></script>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="brand">
        <div class="logo-mark">E</div>
        <div>
          <h1>EderConvert</h1>
          <div style="font-size:12px;color:var(--muted)">Fast • Secure • Mobile-first</div>
        </div>
      </div>
      <div class="nav-actions">
        <button class="btn-outline" onclick="openFAQ()">How it works</button>
        <button class="btn-primary" onclick="document.getElementById('options').scrollIntoView({behavior:'smooth'})">Start</button>
      </div>
    </header>

    <!-- Top Ad -->
    <div style="margin:18px 0;text-align:center">
      <ins class="adsbygoogle" style="display:block" data-ad-client="ca-app-pub-4191528661876815" data-ad-slot="6400801206" data-ad-format="auto" data-full-width-responsive="true"></ins>
    </div>

    <section class="hero">
      <div class="hero-card">
        <h2>Convert files to high-quality PDFs — instantly</h2>
        <p>Images, CSV, Text &amp; documents. Optional password protection, merge PDFs and download — all in your browser.</p>

        <div class="upload-area">
          <input id="fileInput" class="file-input" type="file" accept="image/*,.csv,.txt,.doc,.docx,.xls,.xlsx,.ppt,.pptx,.pdf" multiple aria-label="Upload files to convert">
          <div style="display:flex;gap:10px;width:100%;justify-content:center;margin-top:6px">
            <button class="btn-primary" onclick="document.getElementById('options').scrollIntoView({behavior:'smooth'})">Choose Conversion</button>
            <button class="btn-outline" onclick="openWorkflow('merge')">Merge PDFs</button>
          </div>
          <div class="small-muted" style="margin-top:8px">Supported: JPG, PNG, CSV, TXT, DOCX, XLSX, PPTX, PDF</div>
        </div>

        <div class="options" id="options">
          <div class="card" onclick="openWorkflow('image')">
            <h4>📷 Image → PDF</h4>
            <small>Combine multiple images into a single printable PDF</small>
          </div>
          <div class="card" onclick="openWorkflow('csv')">
            <h4>📊 CSV → PDF</h4>
            <small>Convert tabular CSV into a clean PDF table</small>
          </div>
          <div class="card" onclick="openWorkflow('text')">
            <h4>📝 Text → PDF</h4>
            <small>Paste or upload plain text and get a formatted PDF</small>
          </div>
          <div class="card" onclick="openWorkflow('word')">
            <h4>📄 Word → PDF</h4>
            <small>Server-ready: Upload for backend conversion (future)</small>
          </div>
          <div class="card" onclick="openWorkflow('excel')">
            <h4>📈 Excel → PDF</h4>
            <small>Server-ready: Convert spreadsheets to PDFs</small>
          </div>
          <div class="card" onclick="openWorkflow('ppt')">
            <h4>🎞 PPT → PDF</h4>
            <small>Server-ready: Convert slide decks to PDFs</small>
          </div>
        </div>
      </div>

      <aside class="hero-visual">
        <div class="doc-preview" aria-hidden="true">
          <!-- Simple SVG illustration -->
          <svg width="260" height="220" viewBox="0 0 260 220" fill="none" xmlns="http://www.w3.org/2000/svg">
            <rect x="12" y="20" width="150" height="190" rx="10" fill="white" stroke="#e6eefb" />
            <rect x="96" y="8" width="152" height="172" rx="10" fill="url(#g)" transform="rotate(6 96 8)" />
            <line x1="26" y1="44" x2="136" y2="44" stroke="#e6eefb" stroke-width="6" stroke-linecap="round" />
            <circle cx="60" cy="90" r="18" fill="#4b6ef5" />
            <rect x="30" y="130" width="90" height="12" rx="6" fill="#eef6ff" />
            <defs>
              <linearGradient id="g" x1="0" x2="1">
                <stop offset="0" stop-color="#8b5cf6" />
                <stop offset="1" stop-color="#4b6ef5" />
              </linearGradient>
            </defs>
          </svg>
        </div>
        <div style="text-align:center;color:var(--muted);font-size:13px">Fast, secure and private — files processed locally where possible</div>
      </aside>
    </section>

    <section class="merge" aria-label="Merge PDFs section">
      <h3 style="margin:0 0 8px">Merge PDFs (Client-side)</h3>
      <div style="display:flex;gap:10px;align-items:center;flex-wrap:wrap">
        <input id="mergeFiles" type="file" accept=".pdf" multiple style="flex:1;min-width:220px;padding:10px;border-radius:8px;border:1px solid #eef2ff" />
        <button class="btn-primary" onclick="mergePDFs()">Merge Selected PDFs</button>
      </div>
      <small class="small-muted">Select PDF files and click Merge. For large files use server-side merge (future).</small>
    </section>

    <!-- Bottom Ad -->
    <div style="margin:18px 0;text-align:center">
      <ins class="adsbygoogle" style="display:block" data-ad-client="ca-app-pub-4191528661876815" data-ad-slot="7765961562" data-ad-format="auto" data-full-width-responsive="true"></ins>
    </div>

    <footer>
      © 2025 EderConvert — Built for speed & simplicity
    </footer>
  </div>

  <!-- Modal -->
  <div id="workflowModal" role="dialog" aria-modal="true">
    <div class="modal">
      <div class="modal-head">
        <div>
          <h3 id="modalTitle" style="margin:0">Convert</h3>
          <div id="modalSub" style="font-size:13px;color:var(--muted)">Choose files and options</div>
        </div>
        <button onclick="closeModal()" aria-label="Close modal" style="background:none;border:none;font-size:20px;cursor:pointer">✕</button>
      </div>
      <div class="modal-body">
        <input id="modalFiles" class="input-file" type="file" />
        <div style="display:flex;gap:8px;margin-top:10px;align-items:center">
          <label style="font-size:13px;color:var(--muted)">Password (optional):</label>
          <input id="pdfPassword" type="password" placeholder="Enter password to protect PDF" style="flex:1;padding:10px;border-radius:8px;border:1px solid #eef2ff" />
        </div>
        <div style="margin-top:10px;display:flex;gap:8px;align-items:center">
          <label style="font-size:13px;color:var(--muted)"><input id="addWatermark" type="checkbox"> Add watermark</label>
          <input id="watermarkText" placeholder="Watermark text (optional)" style="flex:1;padding:8px;border-radius:8px;border:1px solid #eef2ff" />
        </div>
      </div>
      <div class="modal-footer">
        <button class="btn-outline" onclick="closeModal()">Cancel</button>
        <button class="btn-primary" id="modalAction">Convert & Download</button>
      </div>
    </div>
  </div>

  <script>
  // Wait until libraries have loaded
  window.addEventListener('DOMContentLoaded', ()=>{
    // push ads
    try{(adsbygoogle=window.adsbygoogle||[]).push({});}catch(e){}

    // expose functions
    window.openWorkflow = function(type){
      const modal = document.getElementById('workflowModal');
      modal.style.display='flex';
      const title = document.getElementById('modalTitle');
      const modalFiles = document.getElementById('modalFiles');
      title.textContent = (type||'Convert').toUpperCase() + ' to PDF';
      // configure input accept
      modalFiles.value = null;
      if(type==='image') modalFiles.accept='image/*';
      else if(type==='csv') modalFiles.accept='.csv';
      else if(type==='text') modalFiles.accept='.txt';
      else modalFiles.accept='.doc,.docx,.xls,.xlsx,.ppt,.pptx,.pdf';
      modalFiles.multiple = (type==='image');
      // set flow handler
      document.getElementById('modalAction').onclick = async function(){ await handleConvert(type); };
    };

    window.closeModal = function(){ document.getElementById('workflowModal').style.display='none'; };

    async function handleConvert(type){
      const input = document.getElementById('modalFiles');
      if(!input.files.length){ alert('Please select a file'); return; }
      const password = document.getElementById('pdfPassword').value.trim();
      const addWater = document.getElementById('addWatermark').checked;
      const watermarkText = document.getElementById('watermarkText').value || '';

      // jsPDF available
      const { jsPDF } = window.jspdf;
      const pdf = new jsPDF();

      try{
        if(type==='image'){
          for(let i=0;i<input.files.length;i++){
            const f = input.files[i];
            const data = await readFileAsDataURL(f);
            const img = await loadImage(data);
            const pw = pdf.internal.pageSize.getWidth();
            const ph = pdf.internal.pageSize.getHeight();
            const ratio = Math.min(pw/img.width, ph/img.height);
            const w = img.width*ratio; const h = img.height*ratio;
            if(i>0) pdf.addPage();
            pdf.addImage(data, 'JPEG', (pw-w)/2, (ph-h)/2, w, h);
            if(addWater && watermarkText){ addTextWatermark(pdf, watermarkText); }
          }
        } else if(type==='text'){
          const txt = await input.files[0].text();
          const lines = pdf.splitTextToSize(txt, 180);
          pdf.text(lines, 15, 20);
          if(addWater && watermarkText) addTextWatermark(pdf, watermarkText);
        } else if(type==='csv'){
          const txt = await input.files[0].text();
          const data = Papa.parse(txt).data;
          let y=20; const colPad=12;
          data.forEach((row,idx)=>{
            pdf.text(row.join(' | '), 15, y);
            y+=10; if(y>280){ pdf.addPage(); y=20; }
          });
          if(addWater && watermarkText) addTextWatermark(pdf, watermarkText);
        } else if(type==='merge'){
          // merge PDF files selected
          const mergedDoc = await PDFLib.PDFDocument.create();
          for(let f of input.files){
            const buf = await f.arrayBuffer();
            const doc = await PDFLib.PDFDocument.load(buf);
            const pages = await mergedDoc.copyPages(doc, doc.getPageIndices());
            pages.forEach(p=>mergedDoc.addPage(p));
          }
          const mergedBytes = await mergedDoc.save();
          downloadBlob(mergedBytes, 'merged.pdf');
          closeModal(); return;
        } else {
          // server-side placeholder for office files
          alert('Office file conversion requires a server. This is a placeholder — upload to server for full conversion.');
          closeModal(); return;
        }

        // If password set -> encrypt using pdf-lib
        if(password){
          const arr = pdf.output('arraybuffer');
          const pdfDoc = await PDFLib.PDFDocument.load(arr);
          pdfDoc.encrypt({ userPassword: password, ownerPassword: password, permissions: { printing:'lowResolution' } });
          const enc = await pdfDoc.save();
          downloadBlob(enc, (input.files[0].name||'converted') + '.pdf');
        } else {
          const name = (input.files[0].name || 'converted').replace(/\.[^/.]+$/, '') + '.pdf';
          pdf.save(name);
        }

        closeModal();
      }catch(err){ console.error(err); alert('Conversion failed: '+(err.message||err)); }
    }

    // helper: add simple watermark
    function addTextWatermark(pdf, text){
      const pw = pdf.internal.pageSize.getWidth(), ph = pdf.internal.pageSize.getHeight();
      pdf.setTextColor(150);
      pdf.setFontSize(20);
      pdf.text(text, pw/2, ph - 20, { align: 'center' });
      pdf.setTextColor(0);
    }

    function readFileAsDataURL(file){ return new Promise((res,rej)=>{ const r=new FileReader(); r.onload=e=>res(e.target.result); r.onerror=rej; r.readAsDataURL(file); }); }
    function loadImage(src){ return new Promise((res,rej)=>{ const i=new Image(); i.onload=()=>res(i); i.onerror=rej; i.src=src; }); }
    function downloadBlob(bytes, filename){ const blob = new Blob([bytes], {type:'application/pdf'}); const url = URL.createObjectURL(blob); const a=document.createElement('a'); a.href=url; a.download=filename; document.body.appendChild(a); a.click(); a.remove(); URL.revokeObjectURL(url); }

    // merge PDFs (separate UI)
    window.mergePDFs = async function(){
      const input = document.getElementById('mergeFiles'); if(!input.files.length){ alert('Select PDFs to merge'); return; }
      const mergedDoc = await PDFLib.PDFDocument.create();
      for(let f of input.files){ const buf = await f.arrayBuffer(); const doc = await PDFLib.PDFDocument.load(buf); const pages = await mergedDoc.copyPages(doc, doc.getPageIndices()); pages.forEach(p=>mergedDoc.addPage(p)); }
      const mergedBytes = await mergedDoc.save(); downloadBlob(mergedBytes, 'merged.pdf'); alert('Merged — download started');
    };

    // Quick FAQ open
    window.openFAQ = function(){ alert('Select a conversion type, choose files, add optional password or watermark, then Convert & Download. Office files require a server.'); };

    // Auto attach main file input to jump to options
    const mainFile = document.getElementById('fileInput');
    if(mainFile){ mainFile.addEventListener('change', ()=>document.getElementById('options').scrollIntoView({behavior:'smooth'})); }

  });
  </script>

  <!-- AdSense init -->
  <script>(adsbygoogle = window.adsbygoogle || []).push({});</script>
</body>
</html>
