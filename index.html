<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1,viewport-fit=cover" />
<title>DGIST 퀴즈 이벤트 · Firebase 버전</title>
<meta name="theme-color" content="#0b1020">
<style>
  :root{
    --bg:#0b1020; --card:#141a32; --acc:#5cc8ff; --acc2:#9ef0a9; --text:#e8ecff; --muted:#9aa4d4;
    --warn:#ff7b7b;
  }
  *{box-sizing:border-box}
  html,body{height:100%}
  body{margin:0;background:linear-gradient(180deg,#0b1020,#0c1535 60%);color:var(--text);font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Apple SD Gothic Neo,Noto Sans KR,Helvetica,Arial,sans-serif}
  .wrap{max-width:940px;margin:0 auto;padding:20px}
  .card{background:var(--card);border:1px solid rgba(255,255,255,.08);border-radius:16px;box-shadow:0 6px 20px rgba(0,0,0,.35);padding:20px}
  h1{margin:0 0 10px;font-size:26px}
  h2{margin:8px 0 16px;font-size:20px;color:var(--acc)}
  p{color:var(--muted);line-height:1.6}
  .row{display:flex;gap:16px;flex-wrap:wrap}
  .col{flex:1;min-width:220px}
  input[type="text"],input[type="number"],input[type="password"],textarea,select{
    width:100%;padding:12px 14px;border-radius:12px;border:1px solid rgba(255,255,255,.12);
    background:#0d1330;color:var(--text);outline:none
  }
  textarea{min-height:180px;font-family:ui-monospace,Consolas,Menlo,monospace}
  .btn{display:inline-flex;align-items:center;justify-content:center;gap:8px;
    background:linear-gradient(180deg,#3aa9ff,#2989ff);border:none;color:#fff;border-radius:12px;
    padding:12px 18px;font-weight:700;cursor:pointer;transition:.2s;box-shadow:0 4px 12px rgba(0,132,255,.35)}
  .btn:hover{transform:translateY(-1px)}
  .btn.ghost{background:transparent;border:1px solid var(--acc);color:var(--acc);box-shadow:none}
  .btn.warn{background:linear-gradient(180deg,#ff7b7b,#ff4b4b)}
  .badge{display:inline-block;padding:3px 8px;border:1px solid rgba(255,255,255,.18);border-radius:999px;color:var(--muted);font-size:12px}
  .prog{height:12px;border-radius:999px;background:#0b1130;border:1px solid rgba(255,255,255,.08);overflow:hidden}
  .prog>div{height:100%;background:linear-gradient(90deg,#49d3ff,#3fffab)}
  .qopt{margin:8px 0;padding:10px 12px;border:1px solid rgba(255,255,255,.14);border-radius:12px;cursor:pointer;background:#0f1740}
  .qopt:hover{border-color:var(--acc)}
  .qopt.sel{border-color:var(--acc2);background:#0e1f36}
  .hidden{display:none}
  .topbar{display:flex;justify-content:space-between;align-items:center;gap:12px;margin-bottom:16px}
  .topbar .left{display:flex;align-items:center;gap:10px}
  .logo{width:36px;height:36px;border-radius:10px;background:linear-gradient(135deg,#49d3ff,#3fffab)}
  .small{font-size:12px;color:var(--muted)}
  .footer{margin-top:18px;text-align:center;color:var(--muted);font-size:12px}
  .list{border:1px solid rgba(255,255,255,.1);border-radius:12px;overflow:hidden}
  .list .rowi{display:flex;gap:10px;padding:10px 12px;border-top:1px solid rgba(255,255,255,.06)}
  .list .rowi:nth-child(odd){background:#0f1736}
  .pill{padding:3px 10px;border-radius:999px;background:#10204a;border:1px solid rgba(255,255,255,.12)}
  .center{text-align:center}
  .right{text-align:right}
  .avatar{width:28px;height:28px;border-radius:999px;background:#1f2a55;display:inline-flex;align-items:center;justify-content:center;font-size:12px}
  .stack{display:flex;align-items:center;gap:8px}
</style>
</head>
<body>
<div class="wrap">
  <div class="topbar">
    <div class="left">
      <div class="logo"></div>
      <div>
        <div style="font-weight:800">DGIST 퀴즈 이벤트 (Firebase)</div>
        <div class="small">이름+생년월일+전화 뒷자리로 중복 차단 (글로벌)</div>
      </div>
    </div>
    <div class="stack">
      <div id="userBox" class="small"></div>
      <button id="btnLogin" class="btn ghost">Google 로그인</button>
      <button id="btnLogout" class="btn ghost hidden">로그아웃</button>
      <button id="btnAdmin" class="btn ghost">관리자</button>
    </div>
  </div>

  <!-- 홈/참여 -->
  <section id="page-home" class="card">
    <h1>환영합니다 👋</h1>
    <p>아래 정보를 입력 후 시작하세요. 동일 조합(이름+생년월일+전화 뒷자리)은 <b>재참여 불가</b>합니다. 데이터는 Firestore에 저장되어 여러 기기에서 <b>동일하게</b> 조회됩니다.</p>
    <div class="row">
      <div class="col">
        <label class="small">이름</label>
        <input id="inpName" type="text" placeholder="예: 홍길동" autocomplete="off"/>
      </div>
      <div class="col">
        <label class="small">생년월일 (YYYYMMDD)</label>
        <input id="inpBirth" type="text" maxlength="8" placeholder="예: 20011231" inputmode="numeric" autocomplete="off"/>
      </div>
      <div class="col">
        <label class="small">전화번호 뒷자리 (4자리)</label>
        <input id="inpPhone4" type="text" maxlength="4" placeholder="예: 1234" inputmode="numeric" autocomplete="off"/>
      </div>
      <div class="col" style="align-self:end">
        <button id="btnStart" class="btn">퀴즈 시작</button>
      </div>
    </div>
    <div id="dupMsg" class="small" style="margin-top:8px;color:var(--warn)"></div>

    <div style="margin-top:22px">
      <div class="row">
        <div class="col">
          <div class="badge">진행 상황</div>
          <div class="prog" style="margin-top:8px"><div id="bar" style="width:0%"></div></div>
          <div class="small" id="visitInfo" style="margin-top:6px">0 / 1500</div>
        </div>
        <div class="col">
          <div class="badge">안내</div>
          <p style="margin-top:8px">개인정보는 <b>SHA-1 해시</b>로 키화되어 저장되며, 관리자 CSV에서는 마스킹되어 출력됩니다.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- 퀴즈 -->
  <section id="page-quiz" class="card hidden">
    <div class="small" id="quizHeader"></div>
    <h2 id="qh"></h2>
    <div id="qopts"></div>
    <div class="row" style="margin-top:14px">
      <div class="col">
        <button id="btnPrev" class="btn ghost">이전</button>
      </div>
      <div class="col right">
        <button id="btnNext" class="btn">다음</button>
      </div>
    </div>
  </section>

  <!-- 결과 -->
  <section id="page-done" class="card hidden center">
    <h2>제출 완료 🎉</h2>
    <p id="scoreLine"></p>
    <p class="small">참여해 주셔서 감사합니다!</p>
    <div style="margin-top:10px">
      <button id="btnHome" class="btn ghost">처음으로</button>
    </div>
  </section>

  <!-- 관리자 로그인 (PIN) -->
  <section id="page-admin-login" class="card hidden">
    <h2>관리자 페이지</h2>
    <p class="small">PIN을 입력하세요. 기본 PIN은 <b>0000</b> 입니다. (관리자에서 변경 가능) · 관리자 페이지는 <b>Google 로그인</b>이 필요합니다.</p>
    <div class="row">
      <div class="col">
        <label class="small">관리자 PIN</label>
        <input id="inpPin" type="password" placeholder="****" />
      </div>
      <div class="col" style="align-self:end">
        <button id="btnPinGo" class="btn">입장</button>
      </div>
    </div>
    <p id="pinMsg" class="small" style="color:var(--warn);margin-top:8px"></p>
  </section>

  <!-- 관리자 본문 -->
  <section id="page-admin" class="card hidden">
    <div class="row">
      <div class="col">
        <h2>대시보드</h2>
        <div class="list">
          <div class="rowi"><div style="width:180px">총 참여 수</div><div id="statTotal"></div></div>
          <div class="rowi"><div style="width:180px">평균 점수</div><div id="statAvg"></div></div>
          <div class="rowi"><div style="width:180px">목표(하한/상한)</div>
            <div><span id="low" class="pill"></span> ~ <span id="high" class="pill"></span></div></div>
          <div class="rowi"><div style="width:180px">진행바</div><div style="flex:1">
            <div class="prog"><div id="abar" style="width:0%"></div></div>
          </div></div>
        </div>
        <div class="row" style="margin-top:10px">
          <div class="col">
            <label class="small">하한(명)</label>
            <input id="inpLow" type="number" min="1" />
          </div>
          <div class="col">
            <label class="small">상한(명)</label>
            <input id="inpHigh" type="number" min="1" />
          </div>
          <div class="col" style="align-self:end">
            <button id="btnRangeSave" class="btn">목표 저장</button>
          </div>
        </div>
        <div style="margin-top:14px">
          <button id="btnCSV" class="btn ghost">참가자 CSV 다운로드</button>
          <button id="btnReset" class="btn warn">전체 데이터 초기화</button>
        </div>
      </div>
      <div class="col">
        <h2>설정</h2>
        <div class="row">
          <div class="col">
            <label class="small">관리자 PIN 변경</label>
            <input id="inpNewPin" type="password" placeholder="새 PIN" />
          </div>
          <div class="col" style="align-self:end">
            <button id="btnPinSet" class="btn">PIN 저장</button>
          </div>
        </div>
        <div class="row" style="margin-top:10px">
          <div class="col">
            <label class="small">출제 문항 수 (기본 5)</label>
            <input id="inpCount" type="number" min="1" max="20" />
          </div>
          <div class="col" style="align-self:end">
            <button id="btnCountSave" class="btn">문항 수 저장</button>
          </div>
        </div>
      </div>
    </div>

    <h2 style="margin-top:20px">문제은행</h2>
    <p class="small">아래 JSON을 수정/추가한 뒤 저장하세요. <b>id, question, choices[], answer</b> 필드가 필요합니다. (answer는 정답 인덱스)</p>
    <textarea id="taBank" spellcheck="false"></textarea>
    <div class="row" style="margin-top:8px">
      <div class="col">
        <button id="btnBankSave" class="btn">문제은행 저장</button>
        <button id="btnBankExport" class="btn ghost">JSON 내보내기</button>
      </div>
      <div class="col right">
        <button id="btnBankTemplate" class="btn ghost">샘플 10문제 로드</button>
      </div>
    </div>

    <h2 style="margin-top:20px">최근 제출</h2>
    <div id="submits" class="list"></div>

    <div class="footer">© DGIST Quiz · Firebase Firestore 저장 · Google 로그인</div>
  </section>
</div>

<!-- Firebase SDKs (compat for no-bundle use) -->
<script src="https://www.gstatic.com/firebasejs/10.12.3/firebase-app-compat.js"></script>
<script src="https://www.gstatic.com/firebasejs/10.12.3/firebase-auth-compat.js"></script>
<script src="https://www.gstatic.com/firebasejs/10.12.3/firebase-firestore-compat.js"></script>

<script>
/**
 * 1) 아래 firebaseConfig 값만 본인 프로젝트 값으로 교체하세요.
 *    Firebase 콘솔 > 프로젝트 설정 > 웹앱 구성에서 복사
 */
const firebaseConfig = {
  apiKey: "AIzaSyBlcq6BX9U8HRilZ0GQmYUoyGjfyWtRA5c",
  authDomain: "fix-2025--dgist-quiz.firebaseapp.com",
  projectId: "fix-2025--dgist-quiz",
  storageBucket: "fix-2025--dgist-quiz.appspot.com",
  messagingSenderId: "898254210099",
  appId: "1:898254210099:web:59abf5f674b44b1e878f46",
  measurementId: "G-LFRDQD9XEN"
};

/**
 * 2) 선택: 테스트 모드 Firestore 규칙 (2주 이벤트용)
 *   - 콘솔 > Firestore > 규칙에서 다음으로 설정 추천 (이벤트 종료 전용)
 * rules_version = '2';
 * service cloud.firestore {
 *   match /databases/{database}/documents {
 *     match /{document=**} { allow read, write: if true; }
 *   }
 * }
 */
</script>

<script>
(function(){
  // --- Firebase Init
  firebase.initializeApp(firebaseConfig);
  const auth = firebase.auth();
  const db = firebase.firestore();

  // --- Collections & Docs
  const COL_KEYS = 'keys';           // unique key hashes
  const COL_SUBS = 'submissions';    // quiz submissions
  const DOC_CFG  = db.collection('config').doc('config'); // count/low/high/pin

  // --- Default Data
  const defaultBank = [
    {id:'q1',question:'DGIST가 위치한 도시는?',choices:['대구','부산','대전','광주'],answer:0},
    {id:'q2',question:'DGIST의 설립 형태로 올바른 것은?',choices:['국립 과학기술특성화대학','사립 종합대학','전문대학','외국계 대학'],answer:0},
    {id:'q3',question:'다음 중 DGIST의 대표 연구 분야와 거리가 가장 먼 것은?',choices:['로봇·모빌리티','바이오·뇌과학','에너지·신소재','해양수산 개발'],answer:3},
    {id:'q4',question:'DGIST는 학부-대학원 통합 캠퍼스 운영을 한다(진위).',choices:['O','X'],answer:0},
    {id:'q5',question:'DGIST의 영문 약자는?',choices:['Daegu Gyeongbuk Institute of Science & Technology','Daejeon Global Institute of Science & Technology','Daegu Global Institute for Software & Tech','Dongguk Institute of Science & Tech'],answer:0},
    {id:'q6',question:'다음 중 DGIST 캠퍼스 소재지는?',choices:['달성군','수성구','북구','동구'],answer:0},
    {id:'q7',question:'DGIST와 관련 깊은 키워드는?',choices:['융합','연극','요리','패션'],answer:0},
    {id:'q8',question:'DGIST의 학생 참여 행사/프로그램 성격과 가장 가까운 것은?',choices:['창업·연구 중심 활동','군사 훈련 중심','금융 상품 판매','해외 이민 절차'],answer:0},
    {id:'q9',question:'다음 중 DGIST의 캠퍼스 문화로 알맞은 것은?',choices:['소규모 연구 중심 환경','대규모 상업시설 중심','관광지 중심','테마파크 중심'],answer:0},
    {id:'q10',question:'DGIST와 가장 관련이 높은 지역 권역은?',choices:['대구·경북','전라권','충청권','수도권만 해당'],answer:0},
  ];
  const defaultCfg = {count:5, low:1000, high:1500, pinHash:''};

  // --- DOM
  const $ = sel => document.querySelector(sel);
  const pages = {
    home: $('#page-home'),
    quiz: $('#page-quiz'),
    done: $('#page-done'),
    adminLogin: $('#page-admin-login'),
    admin: $('#page-admin'),
  };
  const inpName = $('#inpName');
  const inpBirth = $('#inpBirth');
  const inpPhone4 = $('#inpPhone4');
  const btnStart = $('#btnStart');
  const dupMsg = $('#dupMsg');
  const bar = $('#bar');
  const visitInfo = $('#visitInfo');
  const btnAdmin = $('#btnAdmin');
  const btnLogin = $('#btnLogin');
  const btnLogout = $('#btnLogout');
  const userBox = $('#userBox');

  // --- Quiz State
  let quiz = {name:'', birth:'', phone4:'', keyHash:'', picks:[], answers:{}, idx:0};
  let bankCache = null;
  let cfgCache = null;

  // --- Utils
  const nowStr = ()=> new Date().toLocaleString();
  const sha1 = async (str) => {
    const buf = new TextEncoder().encode(str);
    const hash = await crypto.subtle.digest('SHA-1', buf);
    return Array.from(new Uint8Array(hash)).map(b=>b.toString(16).padStart(2,'0')).join('');
  };
  async function ensureConfig(){
    const snap = await DOC_CFG.get();
    if(!snap.exists){
      await DOC_CFG.set(defaultCfg);
      return defaultCfg;
    }
    const cfg = snap.data();
    return {...defaultCfg, ...cfg};
  }
  async function getBank(){
    // 문제은행은 config/bank 문서로 저장, 없으면 default 사용
    const ref = db.collection('config').doc('bank');
    const snap = await ref.get();
    if(snap.exists && Array.isArray(snap.data().items)) return snap.data().items;
    return defaultBank;
  }
  function shuffle(a){
    const arr = a.slice();
    for(let i=arr.length-1;i>0;i--){
      const j = Math.floor(Math.random()*(i+1));
      [arr[i],arr[j]]=[arr[j],arr[i]];
    }
    return arr;
  }
  function show(id){
    Object.values(pages).forEach(el=>el.classList.add('hidden'));
    id.classList.remove('hidden');
  }
  function maskBirth(b){
    return b?.replace(/^(\d{4})(\d{2})(\d{2})$/, (_,y,m,d)=>`${y}**${d}`);
  }
  function maskPhone4(p){ return p?.replace(/^(\d{2})(\d{2})$/,'**$2'); }

  // --- Auth
  auth.onAuthStateChanged(user=>{
    if(user){
      const name = user.displayName || user.email;
      userBox.innerHTML = `<span class="avatar">👤</span> ${name}`;
      btnLogin.classList.add('hidden');
      btnLogout.classList.remove('hidden');
    }else{
      userBox.textContent = '';
      btnLogin.classList.remove('hidden');
      btnLogout.classList.add('hidden');
    }
  });
  btnLogin.onclick = async()=>{
    try{
      const provider = new firebase.auth.GoogleAuthProvider();
      await auth.signInWithPopup(provider);
      alert('로그인 되었습니다.');
    }catch(e){ alert('로그인 실패: '+e.message); }
  };
  btnLogout.onclick = async()=>{
    await auth.signOut();
    alert('로그아웃 되었습니다.');
  };

  // --- Home progress
  async function updateProgress(){
    cfgCache = await ensureConfig();
    visitInfo.textContent = `… / ${cfgCache.high}`;
    // count submissions quickly (approx by query size, for small volume ok)
    const snap = await db.collection(COL_SUBS).get();
    const total = snap.size;
    const pct = Math.min(100, Math.round((total / cfgCache.high) * 100));
    bar.style.width = pct + '%';
    visitInfo.textContent = `${total} / ${cfgCache.high}`;
  }

  // --- Start Quiz
  btnStart.addEventListener('click', async ()=>{
    const name = inpName.value.trim();
    const birth = inpBirth.value.trim();
    const phone4 = inpPhone4.value.trim();

    if(!name){ dupMsg.textContent = '이름을 입력해주세요.'; return; }
    if(!/^\d{8}$/.test(birth)){ dupMsg.textContent = '생년월일은 YYYYMMDD 8자리로 입력하세요.'; return; }
    const y = parseInt(birth.slice(0,4),10);
    const m = parseInt(birth.slice(4,6),10);
    const d = parseInt(birth.slice(6,8),10);
    if(y<1900 || y>2100 || m<1 || m>12 || d<1 || d>31){ dupMsg.textContent='생년월일 형식이 올바르지 않습니다.'; return; }
    if(!/^\d{4}$/.test(phone4)){ dupMsg.textContent = '전화번호 뒷자리는 숫자 4자리로 입력하세요.'; return; }

    const composite = `${name}|${birth}|${phone4}`;
    const keyHash = await sha1(composite);

    // 글로벌 중복 체크 (keys 컬렉션에 문서 id로 저장)
    const keyRef = db.collection(COL_KEYS).doc(keyHash);
    const keySnap = await keyRef.get();
    if(keySnap.exists){
      dupMsg.textContent = '이미 참여한 정보입니다. (이름+생년월일+전화 뒷자리 중복)';
      return;
    }

    // 문제 로드
    if(!bankCache) bankCache = await getBank();
    if(!cfgCache) cfgCache = await ensureConfig();
    const count = Math.min(cfgCache.count||5, bankCache.length);
    quiz = {name, birth, phone4, keyHash, picks: shuffle(bankCache).slice(0,count), answers:{}, idx:0};
    renderQ();
    show(pages.quiz);
  });

  function renderQ(){
    const i = quiz.idx;
    const total = quiz.picks.length;
    const q = quiz.picks[i];
    $('#quizHeader').textContent = `문항 ${i+1} / ${total}`;
    $('#qh').textContent = q.question;
    const box = $('#qopts');
    box.innerHTML = '';
    q.choices.forEach((c,idx)=>{
      const div = document.createElement('div');
      div.className = 'qopt' + (quiz.answers[q.id]===idx?' sel':'');
      div.textContent = c;
      div.onclick = ()=>{ quiz.answers[q.id]=idx; renderQ(); };
      box.appendChild(div);
    });
    $('#btnPrev').disabled = (i===0);
    $('#btnNext').textContent = (i===total-1)?'제출':'다음';
  }
  function nextQ(){
    if(quiz.idx < quiz.picks.length-1){ quiz.idx++; renderQ(); }
    else submitQuiz();
  }
  function prevQ(){
    if(quiz.idx>0){ quiz.idx--; renderQ(); }
  }
  $('#btnNext').onclick = nextQ;
  $('#btnPrev').onclick = prevQ;
  $('#btnHome').onclick = ()=>{ show(pages.home); };

  async function submitQuiz(){
    let score = 0;
    quiz.picks.forEach(q=>{ if(quiz.answers[q.id]===q.answer) score++; });

    // 저장 트랜잭션: keys/id 생성 -> submissions 추가
    const birthMask = maskBirth(quiz.birth);
    const phoneMask = maskPhone4(quiz.phone4);
    const at = Date.now();

    await db.runTransaction(async (tx)=>{
      const keyRef = db.collection(COL_KEYS).doc(quiz.keyHash);
      const keySnap = await tx.get(keyRef);
      if(keySnap.exists) throw new Error('이미 참여 기록이 있습니다.');
      tx.set(keyRef, {usedAt: at});
      const subRef = db.collection(COL_SUBS).doc();
      tx.set(subRef, {
        name: quiz.name,
        birthMask, phoneMask,
        keyHash: quiz.keyHash,
        score, total: quiz.picks.length,
        at, when: nowStr(),
        detail: quiz.picks.map(q=>({id:q.id,correct:q.answer,selected:quiz.answers[q.id] ?? null}))
      });
    });

    $('#scoreLine').textContent = `${quiz.name} 님의 점수: ${score} / ${quiz.picks.length}`;
    await updateProgress();
    show(pages.done);
  }

  // --- Admin
  btnAdmin.onclick = ()=>{
    if(!auth.currentUser){
      alert('관리자 페이지는 Google 로그인이 필요합니다.');
      return;
    }
    show(pages.adminLogin);
    $('#pinMsg').textContent = '';
    $('#inpPin').value = '';
  };

  async function adminEnter(){
    if(!auth.currentUser){ $('#pinMsg').textContent = '먼저 Google 로그인 하세요.'; return; }
    const p = $('#inpPin').value.trim();
    const hash = await sha1(p);
    cfgCache = await ensureConfig();
    let pinHash = cfgCache.pinHash;
    if(!pinHash){
      // 최초 설정: 기본 0000을 해시해 저장
      const defaultHash = await sha1('0000');
      await DOC_CFG.set({pinHash: defaultHash}, {merge:true});
      pinHash = defaultHash;
    }
    if(hash===pinHash){
      showAdminMain();
      window.location.hash = '#admin';
    }else{
      $('#pinMsg').textContent = 'PIN이 올바르지 않습니다.';
    }
  }
  $('#btnPinGo').onclick = adminEnter;

  async function showAdminMain(){
    show(pages.admin);
    // stats
    const subsSnap = await db.collection(COL_SUBS).get();
    const total = subsSnap.size;
    const avg = total? (subsSnap.docs.map(d=>d.data().score).reduce((a,b)=>a+b,0)/total).toFixed(2) : '0.00';
    $('#statTotal').textContent = total + ' 명';
    $('#statAvg').textContent = avg + ' 점';

    cfgCache = await ensureConfig();
    $('#low').textContent = cfgCache.low + '명';
    $('#high').textContent = cfgCache.high + '명';
    const pct = Math.min(100, Math.round((total / cfgCache.high) * 100));
    $('#abar').style.width = pct + '%';
    $('#inpLow').value = cfgCache.low;
    $('#inpHigh').value = cfgCache.high;
    $('#inpCount').value = cfgCache.count || 5;

    // bank JSON
    const bank = await getBank();
    $('#taBank').value = JSON.stringify(bank, null, 2);

    // recent
    renderSubmits();
  }

  async function renderSubmits(){
    const box = $('#submits');
    const snap = await db.collection(COL_SUBS).orderBy('at','desc').limit(20).get();
    box.innerHTML = snap.empty ? '<div class="rowi">제출 기록이 없습니다.</div>' : '';
    snap.forEach(doc=>{
      const s = doc.data();
      const row = document.createElement('div');
      row.className = 'rowi';
      row.innerHTML = `
        <div style="width:160px" class="pill">${s.when}</div>
        <div style="width:160px">${s.name}</div>
        <div style="width:120px">${s.birthMask ?? ''}</div>
        <div style="width:80px">${s.phoneMask ?? ''}</div>
        <div style="width:110px">${s.score} / ${s.total}</div>
        <div class="small" style="color:var(--muted)">key:${(s.keyHash||'').slice(0,8)}…</div>
      `;
      box.appendChild(row);
    });
  }

  // Range / Count Save
  $('#btnRangeSave').onclick = async ()=>{
    const low = parseInt($('#inpLow').value||'0',10);
    const high = parseInt($('#inpHigh').value||'0',10);
    if(!(low>0 && high>=low)){ alert('하한/상한 값을 확인해주세요.'); return; }
    await DOC_CFG.set({low, high}, {merge:true});
    await showAdminMain();
    alert('저장되었습니다.');
  };

  $('#btnCountSave').onclick = async ()=>{
    let c = parseInt($('#inpCount').value||'5',10);
    const bank = JSON.parse($('#taBank').value || '[]');
    if(c<1) c=1;
    if(c>bank.length) c=bank.length;
    await DOC_CFG.set({count: c}, {merge:true});
    alert('출제 문항 수 저장 완료');
  };

  $('#btnPinSet').onclick = async ()=>{
    const np = $('#inpNewPin').value.trim();
    if(!np){ alert('새 PIN을 입력하세요.'); return; }
    const hash = await sha1(np);
    await DOC_CFG.set({pinHash: hash}, {merge:true});
    $('#inpNewPin').value = '';
    alert('PIN이 변경되었습니다.');
  };

  // Bank Save/Export/Template
  $('#btnBankSave').onclick = async ()=>{
    try{
      const parsed = JSON.parse($('#taBank').value);
      if(!Array.isArray(parsed)) throw 0;
      parsed.forEach(q=>{
        if(!q.id||!q.question||!Array.isArray(q.choices)||typeof q.answer!=='number') throw 0;
      });
      await db.collection('config').doc('bank').set({items: parsed});
      // count 보정
      const cfgSnap = await DOC_CFG.get();
      const cfg = cfgSnap.exists ? cfgSnap.data() : defaultCfg;
      if((cfg.count||5) > parsed.length){
        await DOC_CFG.set({count: parsed.length}, {merge:true});
      }
      alert('문제은행 저장 완료');
    }catch(e){
      alert('JSON 형식이 올바르지 않습니다. id, question, choices[], answer(번호)를 확인하세요.');
    }
  };

  $('#btnBankExport').onclick = async ()=>{
    const bank = await getBank();
    const a = document.createElement('a');
    a.href = URL.createObjectURL(new Blob([JSON.stringify(bank,null,2)],{type:'application/json'}));
    a.download = 'dgist_quiz_bank.json';
    a.click();
    URL.revokeObjectURL(a.href);
  };

  $('#btnBankTemplate').onclick = ()=>{
    $('#taBank').value = JSON.stringify(defaultBank, null, 2);
  };

  // CSV Download
  $('#btnCSV').onclick = async ()=>{
    const snap = await db.collection(COL_SUBS).orderBy('at','asc').get();
    const rows = [['when','name','birth_mask','phone_mask','key_hash','score','total']];
    snap.forEach(d=>{
      const s = d.data();
      rows.push([s.when,s.name,s.birthMask||'',s.phoneMask||'',s.keyHash||'',s.score,s.total]);
    });
    const csv = rows.map(r=>r.map(v=>`"${String(v).replaceAll('"','""')}"`).join(',')).join('\n');
    const a = document.createElement('a');
    a.href = URL.createObjectURL(new Blob([csv],{type:'text/csv;charset=utf-8'}));
    a.download = `dgist_quiz_submissions_${new Date().toISOString().slice(0,10)}.csv`;
    a.click();
    URL.revokeObjectURL(a.href);
  };

  // Reset (Delete All)
  $('#btnReset').onclick = async ()=>{
    if(!confirm('정말 전체 데이터를 초기화할까요? 참가 기록과 중복키가 모두 삭제됩니다.')) return;
    // delete submissions
    const subSnap = await db.collection(COL_SUBS).get();
    const batchSize = subSnap.size;
    for(const doc of subSnap.docs){
      await db.collection(COL_SUBS).doc(doc.id).delete();
    }
    // delete keys
    const keySnap = await db.collection(COL_KEYS).get();
    for(const doc of keySnap.docs){
      await db.collection(COL_KEYS).doc(doc.id).delete();
    }
    await updateProgress();
    await renderSubmits();
    alert('초기화 완료');
    await showAdminMain();
  };

  // Direct hash for admin
  if(location.hash==='#admin'){ btnAdmin.click(); }

  // Init
  updateProgress();
})();
</script>
</body>
</html>
