<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0">
<title>Routine</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&family=Inter:wght@400;500;600&display=swap" rel="stylesheet">
<style>
  :root{
    --bg:#f6f6f4;
    --surface:#ffffff;
    --ink:#141414;
    --ink-soft:#8a8a86;
    --line:#e1e1dd;
    --line-soft:#ececea;
    --black:#0a0a0a;
    --white:#ffffff;
  }

  *{box-sizing:border-box;margin:0;padding:0;}

  html,body{
    height:100%;
    background:var(--bg);
    font-family:'Inter',system-ui,-apple-system,sans-serif;
    color:var(--ink);
    -webkit-font-smoothing:antialiased;
  }

  body{
    display:flex;
    justify-content:center;
    min-height:100vh;
  }

  .phone{
    width:100%;
    max-width:420px;
    min-height:100vh;
    background:var(--surface);
    display:flex;
    flex-direction:column;
    position:relative;
    overflow:hidden;
    border-left:1px solid var(--line);
    border-right:1px solid var(--line);
  }

  /* Header */
  .header{
    padding:28px 24px 20px;
    border-bottom:1px solid var(--line);
  }

  .header-top{
    display:flex;
    justify-content:space-between;
    align-items:flex-start;
  }

  .date{
    font-family:'Space Grotesk',sans-serif;
    font-size:22px;
    font-weight:600;
    letter-spacing:-0.02em;
  }

  .subdate{
    font-size:13px;
    color:var(--ink-soft);
    margin-top:2px;
  }

  .streak{
    text-align:right;
  }

  .streak-num{
    font-family:'Space Grotesk',sans-serif;
    font-size:22px;
    font-weight:700;
  }

  .streak-label{
    font-size:11px;
    color:var(--ink-soft);
    margin-top:2px;
  }

  .progress-row{
    margin-top:18px;
    display:flex;
    align-items:center;
    gap:10px;
  }

  .progress-track{
    flex:1;
    height:3px;
    background:var(--line-soft);
    border-radius:2px;
    overflow:hidden;
  }

  .progress-fill{
    height:100%;
    background:var(--black);
    width:0%;
    transition:width .35s ease;
  }

  .progress-text{
    font-size:12px;
    color:var(--ink-soft);
    white-space:nowrap;
    font-variant-numeric:tabular-nums;
  }

  /* List */
  .list-wrap{
    flex:1;
    overflow-y:auto;
    padding:8px 16px 100px;
  }

  .empty-state{
    padding:60px 24px;
    text-align:center;
  }

  .empty-state .glyph{
    font-family:'Space Grotesk',sans-serif;
    font-size:34px;
    font-weight:700;
    margin-bottom:10px;
  }

  .empty-state p{
    font-size:14px;
    color:var(--ink-soft);
    line-height:1.5;
  }

  .task{
    display:flex;
    align-items:center;
    gap:14px;
    padding:16px 8px;
    border-bottom:1px solid var(--line-soft);
    transition:opacity .3s ease, transform .3s ease, max-height .35s ease, padding .35s ease;
    max-height:80px;
    overflow:hidden;
  }

  .task.removing{
    opacity:0;
    transform:translateX(24px);
    max-height:0;
    padding-top:0;
    padding-bottom:0;
    border-color:transparent;
  }

  .check{
    width:24px;
    height:24px;
    min-width:24px;
    border-radius:50%;
    border:1.5px solid var(--ink);
    display:flex;
    align-items:center;
    justify-content:center;
    cursor:pointer;
    transition:background .2s ease, border-color .2s ease;
  }

  .check:active{
    transform:scale(0.92);
  }

  .check svg{
    width:13px;
    height:13px;
    opacity:0;
    transition:opacity .15s ease;
  }

  .task-body{
    flex:1;
    min-width:0;
  }

  .task-name{
    font-size:15px;
    font-weight:500;
    line-height:1.3;
  }

  .task-time{
    font-size:12px;
    color:var(--ink-soft);
    margin-top:2px;
    font-variant-numeric:tabular-nums;
  }

  .task-delete{
    width:28px;
    height:28px;
    display:flex;
    align-items:center;
    justify-content:center;
    color:var(--ink-soft);
    cursor:pointer;
    font-size:18px;
    opacity:0.5;
  }

  .task-delete:active{ opacity:1; }

  /* Add button + sheet */
  .add-btn{
    position:absolute;
    bottom:24px;
    right:24px;
    width:54px;
    height:54px;
    border-radius:50%;
    background:var(--black);
    color:var(--white);
    border:none;
    font-size:26px;
    font-weight:400;
    display:flex;
    align-items:center;
    justify-content:center;
    cursor:pointer;
    box-shadow:0 6px 16px rgba(0,0,0,0.18);
    line-height:1;
    padding-bottom:2px;
    transition:transform .15s ease;
  }

  .add-btn:active{ transform:scale(0.94); }

  .sheet-backdrop{
    position:absolute;
    inset:0;
    background:rgba(10,10,10,0.35);
    opacity:0;
    pointer-events:none;
    transition:opacity .25s ease;
    z-index:5;
  }

  .sheet-backdrop.open{
    opacity:1;
    pointer-events:auto;
  }

  .sheet{
    position:absolute;
    left:0;
    right:0;
    bottom:0;
    background:var(--surface);
    border-radius:20px 20px 0 0;
    padding:22px 24px 28px;
    transform:translateY(100%);
    transition:transform .3s ease;
    z-index:6;
    border-top:1px solid var(--line);
  }

  .sheet.open{ transform:translateY(0); }

  .sheet-title{
    font-family:'Space Grotesk',sans-serif;
    font-size:18px;
    font-weight:600;
    margin-bottom:18px;
  }

  .field{
    margin-bottom:16px;
  }

  .field label{
    display:block;
    font-size:12px;
    color:var(--ink-soft);
    margin-bottom:6px;
  }

  .field input{
    width:100%;
    border:1px solid var(--line);
    border-radius:10px;
    padding:12px 14px;
    font-size:15px;
    font-family:inherit;
    background:var(--bg);
    color:var(--ink);
  }

  .field input:focus{
    outline:none;
    border-color:var(--ink);
  }

  .sheet-actions{
    display:flex;
    gap:10px;
    margin-top:6px;
  }

  .btn{
    flex:1;
    padding:13px;
    border-radius:10px;
    border:none;
    font-size:14px;
    font-weight:600;
    font-family:inherit;
    cursor:pointer;
  }

  .btn-primary{
    background:var(--black);
    color:var(--white);
  }

  .btn-secondary{
    background:var(--bg);
    color:var(--ink);
    border:1px solid var(--line);
  }

  /* Reminder banner */
  .reminder-banner{
    position:absolute;
    top:16px;
    left:16px;
    right:16px;
    background:var(--black);
    color:var(--white);
    border-radius:12px;
    padding:14px 16px;
    display:flex;
    align-items:center;
    gap:12px;
    z-index:10;
    transform:translateY(-120%);
    transition:transform .3s ease;
    box-shadow:0 8px 20px rgba(0,0,0,0.25);
  }

  .reminder-banner.show{ transform:translateY(0); }

  .reminder-banner .rb-text{ flex:1; font-size:13.5px; }
  .reminder-banner .rb-text strong{ font-weight:600; }
  .reminder-banner .rb-close{ font-size:16px; opacity:0.7; cursor:pointer; }

  /* Celebration overlay */
  .celebrate-overlay{
    position:absolute;
    inset:0;
    display:flex;
    flex-direction:column;
    align-items:center;
    justify-content:center;
    background:rgba(255,255,255,0.97);
    opacity:0;
    pointer-events:none;
    transition:opacity .3s ease;
    z-index:20;
  }

  .celebrate-overlay.show{
    opacity:1;
    pointer-events:auto;
  }

  .celebrate-mark{
    width:76px;
    height:76px;
    border-radius:50%;
    background:var(--black);
    display:flex;
    align-items:center;
    justify-content:center;
    margin-bottom:20px;
    transform:scale(0);
    animation:pop .5s cubic-bezier(.34,1.56,.64,1) forwards;
  }

  @keyframes pop{
    to{ transform:scale(1); }
  }

  .celebrate-mark svg{ width:36px; height:36px; }

  .celebrate-title{
    font-family:'Space Grotesk',sans-serif;
    font-size:22px;
    font-weight:600;
    margin-bottom:6px;
    opacity:0;
    animation:rise .4s ease .15s forwards;
  }

  .celebrate-sub{
    font-size:13.5px;
    color:var(--ink-soft);
    opacity:0;
    animation:rise .4s ease .25s forwards;
  }

  @keyframes rise{
    from{ opacity:0; transform:translateY(8px); }
    to{ opacity:1; transform:translateY(0); }
  }

  .confetti{
    position:absolute;
    width:6px;
    height:12px;
    top:-20px;
    opacity:0.9;
  }

  .celebrate-close{
    margin-top:28px;
    padding:11px 26px;
    border-radius:10px;
    border:1px solid var(--line);
    background:var(--surface);
    font-size:13.5px;
    font-weight:600;
    cursor:pointer;
    opacity:0;
    animation:rise .4s ease .35s forwards;
  }

  ::-webkit-scrollbar{ width:0; }
</style>
</head>
<body>

<div class="phone" id="phone">

  <div class="reminder-banner" id="reminderBanner">
    <div class="rb-text" id="reminderText"></div>
    <div class="rb-close" id="reminderClose">✕</div>
  </div>

  <div class="header">
    <div class="header-top">
      <div>
        <div class="date" id="dateLabel">—</div>
        <div class="subdate" id="subDateLabel">—</div>
      </div>
      <div class="streak">
        <div class="streak-num" id="streakNum">0</div>
        <div class="streak-label">day streak</div>
      </div>
    </div>
    <div class="progress-row">
      <div class="progress-track"><div class="progress-fill" id="progressFill"></div></div>
      <div class="progress-text" id="progressText">0 / 0</div>
    </div>
  </div>

  <div class="list-wrap" id="listWrap"></div>

  <button class="add-btn" id="addBtn">+</button>

  <div class="sheet-backdrop" id="sheetBackdrop"></div>
  <div class="sheet" id="sheet">
    <div class="sheet-title">New routine item</div>
    <div class="field">
      <label>What do you need to do</label>
      <input type="text" id="taskNameInput" placeholder="e.g. Morning run" maxlength="60">
    </div>
    <div class="field">
      <label>Remind me at</label>
      <input type="time" id="taskTimeInput">
    </div>
    <div class="sheet-actions">
      <button class="btn btn-secondary" id="cancelBtn">Cancel</button>
      <button class="btn btn-primary" id="saveBtn">Add to routine</button>
    </div>
  </div>

  <div class="celebrate-overlay" id="celebrateOverlay">
    <div class="celebrate-mark">
      <svg viewBox="0 0 24 24" fill="none" stroke="#fff" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round">
        <polyline points="20 6 9 17 4 12"></polyline>
      </svg>
    </div>
    <div class="celebrate-title">Routine complete</div>
    <div class="celebrate-sub" id="celebrateSub">Every task done. Streak extended.</div>
    <button class="celebrate-close" id="celebrateClose">Back to routine</button>
  </div>

</div>

<script>
(function(){
  const STORAGE_KEY = 'routine-app-data';
  let data = null;
  let reminderTimer = null;
  let dismissedReminders = {};

  const DEFAULT_TASKS = [
    { id: 't1', name: 'Drink a glass of water', time: '07:00' },
    { id: 't2', name: 'Stretch for 10 minutes', time: '07:15' },
    { id: 't3', name: 'Review today\'s priorities', time: '09:00' }
  ];

  function todayStr(){
    const d = new Date();
    return d.getFullYear() + '-' + String(d.getMonth()+1).padStart(2,'0') + '-' + String(d.getDate()).padStart(2,'0');
  }

  function fmtDate(){
    const d = new Date();
    const opts = { weekday:'long', month:'long', day:'numeric' };
    return d.toLocaleDateString('en-US', opts);
  }

  async function loadData(){
    try{
      const res = await window.storage.get(STORAGE_KEY, false);
      if(res && res.value){
        data = JSON.parse(res.value);
      }
    }catch(e){
      data = null;
    }
    if(!data){
      data = {
        tasks: DEFAULT_TASKS,
        completedToday: [],
        currentDate: todayStr(),
        streak: 0,
        lastFullDate: null
      };
    }
    handleDayRollover();
    await saveData();
  }

  async function saveData(){
    try{
      await window.storage.set(STORAGE_KEY, JSON.stringify(data), false);
    }catch(e){
      console.error('Save failed', e);
    }
  }

  function handleDayRollover(){
    const today = todayStr();
    if(data.currentDate !== today){
      // check if yesterday's routine was fully completed
      const wasFull = data.tasks.length > 0 && data.completedToday.length >= data.tasks.length;
      if(wasFull){
        data.streak = data.streak + 1;
        data.lastFullDate = data.currentDate;
      } else {
        data.streak = 0;
      }
      data.completedToday = [];
      data.currentDate = today;
      dismissedReminders = {};
    }
  }

  function render(){
    document.getElementById('dateLabel').textContent = 'Today';
    document.getElementById('subDateLabel').textContent = fmtDate();
    document.getElementById('streakNum').textContent = data.streak;

    const remaining = data.tasks.filter(t => !data.completedToday.includes(t.id));
    const total = data.tasks.length;
    const doneCount = total - remaining.length;

    document.getElementById('progressText').textContent = doneCount + ' / ' + total;
    document.getElementById('progressFill').style.width = total > 0 ? Math.round((doneCount/total)*100) + '%' : '0%';

    const wrap = document.getElementById('listWrap');
    wrap.innerHTML = '';

    if(total === 0){
      wrap.innerHTML = '<div class="empty-state"><div class="glyph">+</div><p>No routine items yet.<br>Tap the button below to add your first one.</p></div>';
      return;
    }

    if(remaining.length === 0){
      wrap.innerHTML = '<div class="empty-state"><div class="glyph">✓</div><p>Everything is done for today.<br>Come back tomorrow.</p></div>';
      return;
    }

    remaining
      .slice()
      .sort((a,b) => (a.time || '').localeCompare(b.time || ''))
      .forEach(task => {
        const row = document.createElement('div');
        row.className = 'task';
        row.dataset.id = task.id;
        row.innerHTML =
          '<div class="check" data-id="' + task.id + '">' +
            '<svg viewBox="0 0 24 24" fill="none" stroke="#fff" stroke-width="3" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"></polyline></svg>' +
          '</div>' +
          '<div class="task-body">' +
            '<div class="task-name">' + escapeHtml(task.name) + '</div>' +
            '<div class="task-time">' + (task.time ? formatTime(task.time) : 'No reminder set') + '</div>' +
          '</div>' +
          '<div class="task-delete" data-id="' + task.id + '">×</div>';
        wrap.appendChild(row);
      });
  }

  function escapeHtml(str){
    const div = document.createElement('div');
    div.textContent = str;
    return div.innerHTML;
  }

  function formatTime(t){
    const [h,m] = t.split(':').map(Number);
    const period = h >= 12 ? 'PM' : 'AM';
    let hour = h % 12;
    if(hour === 0) hour = 12;
    return hour + ':' + String(m).padStart(2,'0') + ' ' + period;
  }

  async function completeTask(id){
    const row = document.querySelector('.task[data-id="' + id + '"]');
    if(row){
      row.classList.add('removing');
    }
    if(!data.completedToday.includes(id)){
      data.completedToday.push(id);
    }
    await saveData();

    setTimeout(async () => {
      render();
      if(data.tasks.length > 0 && data.completedToday.length >= data.tasks.length){
        celebrate();
      }
    }, 320);
  }

  async function deleteTask(id){
    data.tasks = data.tasks.filter(t => t.id !== id);
    data.completedToday = data.completedToday.filter(cid => cid !== id);
    await saveData();
    render();
  }

  function celebrate(){
    const overlay = document.getElementById('celebrateOverlay');
    document.getElementById('celebrateSub').textContent =
      'Every task done. Streak now ' + (data.streak) + ' days when tomorrow rolls over.';
    spawnConfetti();
    overlay.classList.add('show');
  }

  function spawnConfetti(){
    const overlay = document.getElementById('celebrateOverlay');
    const shades = ['#0a0a0a', '#4a4a4a', '#8a8a86', '#c9c9c5', '#ffffff'];
    for(let i=0;i<26;i++){
      const piece = document.createElement('div');
      piece.className = 'confetti';
      const left = Math.random()*100;
      const delay = Math.random()*0.4;
      const dur = 1.4 + Math.random()*1.1;
      const color = shades[Math.floor(Math.random()*shades.length)];
      const rot = Math.random()*360;
      piece.style.left = left + '%';
      piece.style.background = color;
      piece.style.border = color === '#ffffff' ? '1px solid #ddd' : 'none';
      piece.style.transform = 'rotate(' + rot + 'deg)';
      piece.style.animation = 'confettiFall ' + dur + 's ease-in ' + delay + 's forwards';
      overlay.appendChild(piece);
      setTimeout(() => piece.remove(), (dur+delay)*1000 + 200);
    }
  }

  const styleTag = document.createElement('style');
  styleTag.textContent = '@keyframes confettiFall{to{ top:105%; opacity:0.15; }}';
  document.head.appendChild(styleTag);

  function checkReminders(){
    const now = new Date();
    const hh = String(now.getHours()).padStart(2,'0');
    const mm = String(now.getMinutes()).padStart(2,'0');
    const current = hh + ':' + mm;

    data.tasks.forEach(task => {
      if(!task.time) return;
      if(data.completedToday.includes(task.id)) return;
      const key = task.id + '_' + current;
      if(task.time === current && !dismissedReminders[key]){
        dismissedReminders[key] = true;
        showReminder(task);
      }
    });
  }

  function showReminder(task){
    const banner = document.getElementById('reminderBanner');
    document.getElementById('reminderText').innerHTML = '<strong>' + escapeHtml(task.name) + '</strong> — scheduled now';
    banner.classList.add('show');
    if('Notification' in window && Notification.permission === 'granted'){
      try{ new Notification(task.name, { body: 'Time for your routine item' }); }catch(e){}
    }
    setTimeout(() => banner.classList.remove('show'), 6000);
  }

  function genId(){
    return 't_' + Date.now() + '_' + Math.floor(Math.random()*1000);
  }

  // Event wiring
  document.getElementById('listWrap').addEventListener('click', (e) => {
    const check = e.target.closest('.check');
    if(check){ completeTask(check.dataset.id); return; }
    const del = e.target.closest('.task-delete');
    if(del){ deleteTask(del.dataset.id); return; }
  });

  const sheet = document.getElementById('sheet');
  const backdrop = document.getElementById('sheetBackdrop');

  function openSheet(){
    document.getElementById('taskNameInput').value = '';
    document.getElementById('taskTimeInput').value = '';
    sheet.classList.add('open');
    backdrop.classList.add('open');
    if('Notification' in window && Notification.permission === 'default'){
      Notification.requestPermission();
    }
  }
  function closeSheet(){
    sheet.classList.remove('open');
    backdrop.classList.remove('open');
  }

  document.getElementById('addBtn').addEventListener('click', openSheet);
  document.getElementById('cancelBtn').addEventListener('click', closeSheet);
  document.getElementById('sheetBackdrop').addEventListener('click', closeSheet);

  document.getElementById('saveBtn').addEventListener('click', async () => {
    const name = document.getElementById('taskNameInput').value.trim();
    const time = document.getElementById('taskTimeInput').value;
    if(!name) return;
    data.tasks.push({ id: genId(), name: name, time: time || null });
    await saveData();
    closeSheet();
    render();
  });

  document.getElementById('reminderClose').addEventListener('click', () => {
    document.getElementById('reminderBanner').classList.remove('show');
  });

  document.getElementById('celebrateClose').addEventListener('click', () => {
    document.getElementById('celebrateOverlay').classList.remove('show');
  });

  // Midnight rollover check while app stays open
  setInterval(() => {
    const before = data.currentDate;
    handleDayRollover();
    if(before !== data.currentDate){
      saveData().then(render);
    }
    checkReminders();
  }, 30000);

  // Init
  (async function init(){
    await loadData();
    render();
    checkReminders();
  })();

})();
</script>

</body>
</html>
