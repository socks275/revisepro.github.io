<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Quizlet Hub - Global Revision Sets</title>
  <style>
    :root {
      --bg: #0a092d;
      --card-bg: #2e3856;
      --card-hover: #38456c;
      --text: #ffffff;
      --subtext: #939bb4;
      --accent: #4255ff;
      --accent-hover: #2e3edb;
      --official: #23b26d;
      --public: #ffcd1f;
      --border: rgba(66, 85, 255, 0.2);
    }

    * { box-sizing: border-box; margin: 0; padding: 0; font-family: system-ui, -apple-system, sans-serif; }
    body { background-color: var(--bg); color: var(--text); padding-bottom: 50px; }

    #ad-container { background: #121420; text-align: center; padding: 1rem; border-bottom: 1px solid var(--border); min-height: 50px; }
    #ad-container img { max-width: 100%; max-height: 120px; border-radius: 8px; }
    #ad-container iframe { width: 100%; max-width: 560px; height: 200px; border: none; border-radius: 8px; }

    header {
      background-color: var(--card-bg);
      padding: 1rem 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      border-bottom: 2px solid var(--border);
    }
    .logo { font-size: 1.5rem; font-weight: bold; color: var(--accent); text-transform: uppercase; letter-spacing: 1px; cursor: pointer; }
    nav { display: flex; gap: 0.5rem; align-items: center; }
    nav button {
      background: transparent;
      border: none;
      color: var(--text);
      padding: 0.6rem 1rem;
      font-weight: 600;
      border-radius: 8px;
      cursor: pointer;
    }
    nav button.active, nav button:hover { background: var(--card-hover); }
    .btn-accent { background: var(--accent) !important; color: white !important; }
    .btn-accent:hover { background: var(--accent-hover) !important; }

    .user-badge { background: #1a1d24; padding: 0.4rem 0.8rem; border-radius: 20px; font-size: 0.85rem; color: #38d39f; }

    .container { max-width: 950px; margin: 2rem auto; padding: 0 1rem; }
    .view-section { display: none; }
    .view-section.active { display: block; }

    .search-bar {
      width: 100%;
      padding: 0.8rem 1rem;
      background: #121420;
      border: 1px solid var(--border);
      border-radius: 8px;
      color: var(--text);
      font-size: 1rem;
      margin-top: 1rem;
    }

    .sets-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
      gap: 1.5rem;
      margin-top: 1.5rem;
    }
    .set-card {
      background: var(--card-bg);
      border: 1px solid var(--border);
      border-radius: 12px;
      padding: 1.5rem;
      cursor: pointer;
      transition: transform 0.2s, background 0.2s;
    }
    .set-card:hover { transform: translateY(-4px); background: var(--card-hover); }
    .set-title { font-size: 1.2rem; font-weight: bold; margin-bottom: 0.5rem; }
    .set-meta { font-size: 0.85rem; color: var(--subtext); display: flex; justify-content: space-between; align-items: center; margin-top: 1rem; }

    .badge { padding: 0.25rem 0.6rem; border-radius: 20px; font-size: 0.75rem; font-weight: bold; }
    .badge-official { background: var(--official); color: #000; }
    .badge-public { background: var(--public); color: #000; }

    .perspective { perspective: 1000px; margin: 1.5rem 0; }
    .flashcard-inner {
      background-color: var(--card-bg);
      border-radius: 16px;
      height: 300px;
      width: 100%;
      text-align: center;
      transition: transform 0.6s;
      transform-style: preserve-3d;
      cursor: pointer;
      position: relative;
      box-shadow: 0 8px 24px rgba(0,0,0,0.3);
    }
    .flashcard-inner.flipped { transform: rotateY(180deg); }
    .card-front, .card-back {
      position: absolute;
      width: 100%; height: 100%;
      backface-visibility: hidden;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      padding: 2rem;
      border-radius: 16px;
    }
    .card-back { transform: rotateY(180deg); background-color: var(--card-hover); }

    .card-controls { display: flex; justify-content: space-between; align-items: center; margin-bottom: 2rem; }
    .btn { background: var(--accent); color: white; border: none; padding: 0.75rem 1.5rem; font-weight: bold; border-radius: 8px; cursor: pointer; }
    .btn:hover { background: var(--accent-hover); }

    .form-group { margin-bottom: 1.2rem; }
    label { display: block; margin-bottom: 0.4rem; font-size: 0.85rem; color: var(--subtext); }
    input, select, textarea {
      width: 100%; padding: 0.75rem; background: #121420; border: 1px solid var(--border);
      color: var(--text); border-radius: 8px; margin-top: 0.2rem;
    }
    .card-input-row { background: #121420; padding: 1rem; border-radius: 8px; margin-bottom: 1rem; border: 1px solid var(--border); }

    .modal {
      display: none; position: fixed; top: 0; left: 0; width: 100%; height: 100%;
      background: rgba(0,0,0,0.8); justify-content: center; align-items: center; z-index: 100;
    }
    .modal-content { background: var(--card-bg); padding: 2rem; border-radius: 12px; width: 100%; max-width: 400px; }

    .quiz-option {
      background: var(--card-bg); border: 2px solid var(--border); padding: 1rem;
      margin-bottom: 0.75rem; border-radius: 8px; cursor: pointer; font-weight: 600;
    }
    .quiz-option:hover { background: var(--card-hover); }
  </style>
</head>
<body>

  <div id="ad-container">
    <div id="ad-content">📢 Welcome to Quizlet Hub! Click "+ Add Set" to publish sets live across all devices.</div>
  </div>

  <header>
    <div class="logo" onclick="showSection('dashboard-view')">Quizlet Hub</div>
    <nav>
      <button onclick="showSection('dashboard-view')">Browse Sets</button>
      <button class="btn-accent" onclick="openCreateSetView()">+ Add Set</button>
      <span id="user-display" class="user-badge" style="display:none;"></span>
      <button id="auth-btn" onclick="openAuthModal()">Login / Register</button>
    </nav>
  </header>

  <div class="container">

    <!-- DASHBOARD -->
    <div id="dashboard-view" class="view-section active">
      <h2>Global Revision Sets</h2>
      <input type="text" id="search-input" class="search-bar" placeholder="🔍 Search sets by title or topic..." oninput="filterSets()">
      <div id="sets-container" class="sets-grid"></div>
    </div>

    <!-- CREATE SET -->
    <div id="create-set-view" class="view-section">
      <div style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 1.5rem;">
        <h2>Create New Flashcard Set</h2>
        <button class="btn" style="background: transparent; border: 1px solid var(--border);" onclick="showSection('dashboard-view')">Cancel</button>
      </div>

      <form onsubmit="handleSaveSet(event)">
        <div class="form-group">
          <label>Set Title:</label>
          <input type="text" id="set-title-input" placeholder="e.g. GCSE Physics - Waves" required>
        </div>
        <div class="form-group">
          <label>Description:</label>
          <input type="text" id="set-desc-input" placeholder="e.g. Core formulas and definitions">
        </div>

        <h3 style="margin: 1.5rem 0 1rem;">Flashcards</h3>
        <div id="cards-input-list"></div>

        <button type="button" class="btn" style="background: var(--card-hover); margin-bottom: 1.5rem;" onclick="addCardRow()">+ Add Card Pair</button>
        <br>
        <button type="submit" class="btn" style="width: 100%;">Publish to Cloud</button>
      </form>
    </div>

    <!-- STUDY VIEW -->
    <div id="study-view" class="view-section">
      <div style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 1rem;">
        <div>
          <button class="btn" style="background: transparent; border: 1px solid var(--border); padding: 0.4rem 0.8rem; font-size: 0.85rem;" onclick="showSection('dashboard-view')">← Back to All Sets</button>
          <h2 id="study-set-title" style="margin-top: 0.5rem;">Set Title</h2>
        </div>
        <div>
          <button class="btn" onclick="toggleStudyMode('cards')">Flashcards</button>
          <button class="btn" style="background: var(--card-hover);" onclick="toggleStudyMode('learn')">Learn Mode</button>
        </div>
      </div>

      <div id="mode-cards">
        <div class="perspective">
          <div class="flashcard-inner" id="card-element" onclick="flipCard()">
            <div class="card-front">
              <span id="card-badge" class="badge"></span>
              <h2 id="card-q">Question</h2>
              <p style="font-size:0.8rem; color:var(--subtext); position:absolute; bottom:15px;">Click card to flip</p>
            </div>
            <div class="card-back">
              <h2 id="card-a">Answer</h2>
            </div>
          </div>
        </div>

        <div class="card-controls">
          <button class="btn" onclick="prevCard()">← Prev</button>
          <span id="card-count" style="font-weight: bold; color: var(--subtext);">0 / 0</span>
          <button class="btn" onclick="nextCard()">Next →</button>
        </div>
      </div>

      <div id="mode-learn" style="display: none;">
        <div id="quiz-box" style="background: var(--card-bg); padding: 2rem; border-radius: 12px; margin-top: 1rem;">
          <h3 id="quiz-question" style="margin-bottom: 1.5rem;">Question</h3>
          <div id="quiz-options"></div>
        </div>
      </div>
    </div>

    <!-- ADMIN PANEL -->
    <div id="admin-panel" class="view-section" style="background: #1e1b4b; padding: 2rem; border-radius: 12px; border: 2px dashed var(--accent);">
      <h2>⚙️ Owner Admin Control Panel</h2>
      <p style="color: var(--subtext); margin-bottom: 1.5rem; font-size: 0.9rem;">Authenticated Owner Access Active.</p>

      <div>
        <h3>Update Global Website Advertisement</h3>
        <div class="form-group" style="margin-top: 1rem;">
          <label>Ad Type:</label>
          <select id="ad-type">
            <option value="text">Text / Announcement</option>
            <option value="image">Image Banner (Image URL)</option>
            <option value="video">Embedded Video (YouTube Embed HTML)</option>
          </select>
        </div>
        <div class="form-group">
          <label>Ad Content / Link:</label>
          <textarea id="ad-input" rows="3" placeholder="Enter text, image link, or video code..."></textarea>
        </div>
        <button class="btn" onclick="saveAdminAd()">Publish Advert</button>
      </div>
    </div>

  </div>

  <!-- AUTH MODAL -->
  <div id="auth-modal" class="modal">
    <div class="modal-content">
      <h2 style="margin-bottom: 1rem;">Account Login / Register</h2>
      
      <div class="form-group">
        <label>Username:</label>
        <input type="text" id="auth-username" placeholder="Enter username">
      </div>
      <div class="form-group">
        <label>Password:</label>
        <input type="password" id="auth-password" placeholder="Enter password">
      </div>
      <div class="form-group">
        <label>Admin Passcode (Optional):</label>
        <input type="password" id="auth-admin-code" placeholder="Enter passcode">
      </div>

      <button class="btn" style="width: 100%; margin-bottom: 0.5rem;" onclick="handleAuth()">Login / Register</button>
      <button class="btn" style="width: 100%; background: transparent; border: 1px solid var(--border);" onclick="closeAuthModal()">Cancel</button>
    </div>
  </div>

  <script>
    const CLOUD_API_URL = "https://api.jsonbin.io/v3/b/65d1bf2c1f5677401f31f9e2";
    const SECRET_PASS_HASH = "MTM1Nzk="; // Passcode "13579"

    let currentUser = null;
    let isAdmin = false;
    let globalData = { sets: [], ad: { type: "text", content: "Welcome to Quizlet Hub!" } };
    let activeSetIndex = null;
    let activeCardIndex = 0;

    async function loadCloudData() {
      try {
        const res = await fetch(CLOUD_API_URL + "/latest", {
          headers: { "X-Master-Key": "$2a$10$8C5X0G5dZ3e.uN/3N8pU/.QZzU04rA4U8Z0qE4T3rX4" }
        });
        if(res.ok) {
          const data = await res.json();
          if(data.record) globalData = data.record;
        }
      } catch(e) { console.log("Using local state"); }
      renderSetsGrid(globalData.sets);
      if(globalData.ad) renderAd(globalData.ad);
    }

    async function syncCloudData() {
      try {
        await fetch(CLOUD_API_URL, {
          method: "PUT",
          headers: {
            "Content-Type": "application/json",
            "X-Master-Key": "$2a$10$8C5X0G5dZ3e.uN/3N8pU/.QZzU04rA4U8Z0qE4T3rX4"
          },
          body: JSON.stringify(globalData)
        });
      } catch(e) {}
    }

    function showSection(id) {
      document.querySelectorAll('.view-section').forEach(s => s.classList.remove('active'));
      document.getElementById(id).classList.add('active');
    }

    function renderSetsGrid(setsToRender) {
      const container = document.getElementById('sets-container');
      container.innerHTML = '';

      if(!setsToRender || setsToRender.length === 0) {
        container.innerHTML = `<p style="grid-column: 1/-1; text-align:center; color: var(--subtext);">No sets found.</p>`;
        return;
      }

      setsToRender.forEach((set) => {
        const idx = globalData.sets.indexOf(set);
        const setCard = document.createElement('div');
        setCard.className = 'set-card';
        setCard.onclick = () => openStudySet(idx);
        
        setCard.innerHTML = `
          <div class="set-title">${escapeHtml(set.title)}</div>
          <div style="font-size: 0.85rem; color: var(--subtext);">${escapeHtml(set.desc || '')}</div>
          <div class="set-meta">
            <span>📚 ${set.cards ? set.cards.length : 0} terms</span>
            <span class="badge ${set.isOfficial ? 'badge-official' : 'badge-public'}">${set.isOfficial ? 'Official' : 'Public'}</span>
          </div>
        `;
        container.appendChild(setCard);
      });
    }

    function filterSets() {
      const query = document.getElementById('search-input').value.toLowerCase();
      const filtered = globalData.sets.filter(s => 
        s.title.toLowerCase().includes(query) || (s.desc && s.desc.toLowerCase().includes(query))
      );
      renderSetsGrid(filtered);
    }

    function openCreateSetView() {
      if(!currentUser) { alert("Please login first!"); return openAuthModal(); }
      document.getElementById('set-title-input').value = '';
      document.getElementById('set-desc-input').value = '';
      document.getElementById('cards-input-list').innerHTML = '';
      addCardRow(); addCardRow();
      showSection('create-set-view');
    }

    function addCardRow() {
      const list = document.getElementById('cards-input-list');
      const row = document.createElement('div');
      row.className = 'card-input-row';
      row.innerHTML = `
        <div class="form-group"><input type="text" class="card-q-input" placeholder="Question / Term" required></div>
        <div class="form-group" style="margin:0;"><input type="text" class="card-a-input" placeholder="Answer / Definition" required></div>
      `;
      list.appendChild(row);
    }

    async function handleSaveSet(e) {
      e.preventDefault();
      const title = document.getElementById('set-title-input').value.trim();
      const desc = document.getElementById('set-desc-input').value.trim();
      const q = document.querySelectorAll('.card-q-input');
      const a = document.querySelectorAll('.card-a-input');
      
      let cards = [];
      q.forEach((item, idx) => {
        if(item.value.trim() && a[idx].value.trim()) cards.push({ q: item.value.trim(), a: a[idx].value.trim() });
      });

      if(!globalData.sets) globalData.sets = [];
      globalData.sets.push({ id: Date.now().toString(), title, desc, author: currentUser, isOfficial: isAdmin, cards });
      renderSetsGrid(globalData.sets);
      await syncCloudData();
      showSection('dashboard-view');
    }

    function openStudySet(index) {
      activeSetIndex = index;
      activeCardIndex = 0;
      const set = globalData.sets[index];
      document.getElementById('study-set-title').textContent = set.title;
      showSection('study-view');
      toggleStudyMode('cards');
    }

    function renderCard() {
      const set = globalData.sets[activeSetIndex];
      const card = set.cards[activeCardIndex];
      document.getElementById('card-q').textContent = card.q;
      document.getElementById('card-a').textContent = card.a;
      document.getElementById('card-badge').textContent = set.isOfficial ? 'Official' : 'Public';
      document.getElementById('card-badge').className = 'badge ' + (set.isOfficial ? 'badge-official' : 'badge-public');
      document.getElementById('card-count').textContent = `${activeCardIndex + 1} / ${set.cards.length}`;
      document.getElementById('card-element').classList.remove('flipped');
    }

    function flipCard() { document.getElementById('card-element').classList.toggle('flipped'); }
    function nextCard() { activeCardIndex = (activeCardIndex + 1) % globalData.sets[activeSetIndex].cards.length; renderCard(); }
    function prevCard() { const s = globalData.sets[activeSetIndex].cards; activeCardIndex = (activeCardIndex - 1 + s.length) % s.length; renderCard(); }

    function toggleStudyMode(mode) {
      document.getElementById('mode-cards').style.display = mode === 'cards' ? 'block' : 'none';
      document.getElementById('mode-learn').style.display = mode === 'learn' ? 'block' : 'none';
      if(mode === 'cards') renderCard(); else startLearnQuiz();
    }

    function startLearnQuiz() {
      const set = globalData.sets[activeSetIndex];
      const current = set.cards[activeCardIndex];
      document.getElementById('quiz-question').textContent = `Definition of: "${current.q}"?`;
      const container = document.getElementById('quiz-options');
      container.innerHTML = '';

      let choices = [current.a];
      while(choices.length < Math.min(4, set.cards.length)) {
        let r = set.cards[Math.floor(Math.random() * set.cards.length)].a;
        if(!choices.includes(r)) choices.push(r);
      }
      choices.sort(() => Math.random() - 0.5);

      choices.forEach(choice => {
        const div = document.createElement('div');
        div.className = 'quiz-option';
        div.textContent = choice;
        div.onclick = () => {
          div.style.background = (choice === current.a) ? '#23b26d' : '#ff4757';
          if(choice === current.a) setTimeout(nextCard, 800);
        };
        container.appendChild(div);
      });
    }

    function openAuthModal() { document.getElementById('auth-modal').style.display = 'flex'; }
    function closeAuthModal() { document.getElementById('auth-modal').style.display = 'none'; }

    function handleAuth() {
      const user = document.getElementById('auth-username').value.trim();
      const code = document.getElementById('auth-admin-code').value.trim();
      if(!user) return alert("Enter a username.");

      currentUser = user;
      document.getElementById('user-display').textContent = `👤 ${user}`;
      document.getElementById('user-display').style.display = 'inline-block';

      if(code && btoa(code) === SECRET_PASS_HASH) {
        isAdmin = true;
        const nav = document.querySelector('nav');
        if(!document.getElementById('admin-nav-btn')) {
          const adminBtn = document.createElement('button');
          adminBtn.id = 'admin-nav-btn';
          adminBtn.style.color = '#ffcd1f';
          adminBtn.textContent = '⚡ Admin';
          adminBtn.onclick = () => showSection('admin-panel');
          nav.appendChild(adminBtn);
        }
      }
      closeAuthModal();
    }

    async function saveAdminAd() {
      globalData.ad = { type: document.getElementById('ad-type').value, content: document.getElementById('ad-input').value };
      renderAd(globalData.ad);
      await syncCloudData();
    }

    function renderAd(ad) {
      const container = document.getElementById('ad-content');
      if(!ad || !ad.content) return;
      if(ad.type === 'text') container.innerHTML = `📢 ${escapeHtml(ad.content)}`;
      else if(ad.type === 'image') container.innerHTML = `<img src="${escapeHtml(ad.content)}">`;
      else if(ad.type === 'video') container.innerHTML = ad.content.includes('<iframe') ? ad.content : `<iframe src="${escapeHtml(ad.content)}"></iframe>`;
    }

    function escapeHtml(str) { return str ? str.replace(/&/g, "&amp;").replace(/</g, "&lt;").replace(/>/g, "&gt;") : ''; }

    // Register Service Worker for PWA
    if ('serviceWorker' in navigator) {
      window.addEventListener('load', () => { navigator.serviceWorker.register('./sw.js').catch(()=>{}); });
    }

    loadCloudData();
  </script>
</body>
</html>
