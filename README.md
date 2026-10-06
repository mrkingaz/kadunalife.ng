# kadunalife.ng
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#0b2417">
<meta name="description" content="Kaduna Life — Your Kaduna. Your Story.">
<title>Kaduna Life — Your Kaduna. Your Story.</title>

<style>
:root{
  --green:#0b2417;
  --green2:#123b25;
  --green3:#1b5a34;
  --gold:#f4b942;
  --gold2:#ffd66b;
  --cream:#fff8e8;
  --paper:#fffdf7;
  --red:#c94b4b;
  --blue:#3777b8;
  --text:#172018;
  --muted:#69736b;
  --border:#e5e0d4;
  --shadow:0 14px 40px rgba(8,25,15,.12);
}

*{box-sizing:border-box}
html,body{margin:0;padding:0}
body{
  font-family:Inter,system-ui,-apple-system,BlinkMacSystemFont,"Segoe UI",sans-serif;
  background:#f3f0e7;
  color:var(--text);
  min-height:100vh;
}

button,input,select{font:inherit}
button{cursor:pointer}

.hidden{display:none!important}

.screen{
  min-height:100vh;
}

/* INTRO */
#intro{
  background:
    radial-gradient(circle at 20% 20%,rgba(244,185,66,.16),transparent 28%),
    radial-gradient(circle at 80% 80%,rgba(43,119,78,.2),transparent 32%),
    linear-gradient(135deg,#07170e,#123b25 60%,#1d5935);
  color:white;
  display:flex;
  align-items:center;
  justify-content:center;
  padding:30px 18px;
}

.intro-card{
  max-width:850px;
  width:100%;
  text-align:center;
}

.logo-mark{
  width:90px;
  height:90px;
  border-radius:28px;
  background:linear-gradient(135deg,var(--gold),#ffda79);
  color:var(--green);
  display:grid;
  place-items:center;
  font-size:44px;
  margin:0 auto 22px;
  box-shadow:0 20px 50px rgba(0,0,0,.25);
}

.intro-card h1{
  font-size:clamp(48px,10vw,92px);
  line-height:.9;
  margin:0;
  letter-spacing:-4px;
}

.intro-card h1 span{color:var(--gold)}

.tagline{
  font-size:clamp(18px,3vw,25px);
  opacity:.85;
  margin:22px 0 10px;
}

.intro-copy{
  max-width:620px;
  margin:0 auto 35px;
  color:#d9e6dc;
  line-height:1.7;
}

.primary{
  border:0;
  border-radius:15px;
  padding:15px 25px;
  background:var(--gold);
  color:#17200f;
  font-weight:800;
  box-shadow:0 10px 25px rgba(0,0,0,.18);
  transition:.2s;
}

.primary:hover{transform:translateY(-2px);background:var(--gold2)}

.secondary{
  border:1px solid var(--border);
  border-radius:12px;
  padding:11px 16px;
  background:white;
  color:var(--text);
  font-weight:700;
}

.danger{
  background:#fff0f0;
  color:#9f3030;
  border-color:#efcccc;
}

/* CREATION */
#creation{
  padding:30px 15px 60px;
}

.creation-wrap{
  max-width:950px;
  margin:auto;
}

.top-brand{
  color:var(--green);
  font-weight:900;
  letter-spacing:-.5px;
  margin-bottom:18px;
}

.creation-card{
  background:var(--paper);
  border:1px solid var(--border);
  border-radius:24px;
  padding:clamp(20px,4vw,40px);
  box-shadow:var(--shadow);
}

.creation-card h2{
  margin:0 0 8px;
  font-size:34px;
}

.sub{
  color:var(--muted);
  margin-top:0;
}

.form-grid{
  display:grid;
  grid-template-columns:repeat(2,1fr);
  gap:18px;
  margin-top:25px;
}

.field label{
  display:block;
  font-weight:800;
  font-size:14px;
  margin-bottom:7px;
}

.field input,.field select{
  width:100%;
  border:1px solid var(--border);
  border-radius:12px;
  padding:13px;
  background:white;
  outline:none;
}

.field input:focus,.field select:focus{
  border-color:var(--green3);
  box-shadow:0 0 0 3px rgba(27,90,52,.1);
}

.full{grid-column:1/-1}

.backgrounds{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:12px;
  margin-top:10px;
}

.bg-option{
  border:2px solid var(--border);
  background:white;
  border-radius:15px;
  padding:15px;
  text-align:left;
  transition:.2s;
}

.bg-option:hover{border-color:#9db6a4}
.bg-option.selected{
  border-color:var(--gold);
  background:#fff9e9;
  box-shadow:0 0 0 2px rgba(244,185,66,.2);
}

.bg-option strong{display:block;margin-bottom:4px}
.bg-option small{color:var(--muted);line-height:1.4}

.creation-actions{
  display:flex;
  justify-content:flex-end;
  margin-top:28px;
}

/* GAME */
#game{
  min-height:100vh;
}

.game-header{
  background:var(--green);
  color:white;
  position:sticky;
  top:0;
  z-index:50;
  box-shadow:0 4px 20px rgba(0,0,0,.16);
}

.header-inner{
  max-width:1250px;
  margin:auto;
  padding:13px 16px;
  display:flex;
  align-items:center;
  justify-content:space-between;
  gap:15px;
}

.brand{
  font-weight:900;
  white-space:nowrap;
}

.brand span{color:var(--gold)}

.header-stats{
  display:flex;
  gap:8px;
  flex-wrap:wrap;
  justify-content:flex-end;
}

.mini-stat{
  background:rgba(255,255,255,.09);
  border-radius:10px;
  padding:7px 10px;
  font-size:12px;
}

.mini-stat b{display:block;color:white}
.mini-stat span{color:#b9cbbd}

.game-layout{
  max-width:1250px;
  margin:auto;
  display:grid;
  grid-template-columns:235px minmax(0,1fr);
  gap:20px;
  padding:20px 15px 50px;
}

.sidebar{
  background:white;
  border:1px solid var(--border);
  border-radius:20px;
  padding:12px;
  height:max-content;
  position:sticky;
  top:78px;
}

.nav-btn{
  width:100%;
  border:0;
  background:transparent;
  padding:12px 13px;
  text-align:left;
  border-radius:11px;
  font-weight:750;
  color:#445047;
  margin-bottom:3px;
}

.nav-btn:hover{background:#f2f6f2}
.nav-btn.active{
  background:var(--green);
  color:white;
}

.sidebar-divider{
  height:1px;
  background:var(--border);
  margin:12px 4px;
}

.content{
  min-width:0;
}

.view{display:none}
.view.active{display:block}

.page-title{
  display:flex;
  justify-content:space-between;
  align-items:flex-start;
  gap:15px;
  margin-bottom:18px;
}

.page-title h2{
  margin:0;
  font-size:30px;
}

.page-title p{
  margin:5px 0 0;
  color:var(--muted);
}

/* CARDS */
.card{
  background:white;
  border:1px solid var(--border);
  border-radius:18px;
  padding:20px;
  box-shadow:0 5px 18px rgba(20,30,20,.04);
}

.card-grid{
  display:grid;
  grid-template-columns:repeat(2,minmax(0,1fr));
  gap:15px;
}

.three{
  grid-template-columns:repeat(3,minmax(0,1fr));
}

.card h3{
  margin:0 0 8px;
}

.card p{
  color:var(--muted);
  line-height:1.55;
}

.hero-card{
  background:
    linear-gradient(120deg,rgba(11,36,23,.96),rgba(25,86,51,.9)),
    radial-gradient(circle at 80% 20%,rgba(244,185,66,.4),transparent 30%);
  color:white;
  border:0;
}

.hero-card p{color:#d9e7dc}

.money{
  color:#2f8a4f;
  font-weight:900;
}

.big-money{
  font-size:34px;
  font-weight:950;
  color:var(--gold);
}

.progress{
  height:9px;
  background:#e9ece8;
  border-radius:999px;
  overflow:hidden;
  margin-top:8px;
}

.progress i{
  display:block;
  height:100%;
  background:var(--green3);
  border-radius:999px;
}

.stat-row{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:10px;
}

.stat-box{
  background:#f7f7f3;
  border-radius:12px;
  padding:12px;
}

.stat-box small{
  color:var(--muted);
  display:block;
}

.stat-box strong{
  font-size:20px;
}

/* ACTIONS */
.action-list{
  display:grid;
  gap:10px;
}

.action{
  border:1px solid var(--border);
  background:white;
  border-radius:13px;
  padding:14px;
  display:flex;
  align-items:center;
  justify-content:space-between;
  gap:12px;
}

.action:hover{border-color:#b8c8bc;background:#fbfdfb}

.action-info strong{display:block}
.action-info small{color:var(--muted);display:block;margin-top:3px}

.action button{
  flex-shrink:0;
}

/* LOCATION */
.location-grid{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:13px;
}

.location{
  min-height:150px;
  background:linear-gradient(145deg,#fff,#f7f4e9);
  border:1px solid var(--border);
  border-radius:16px;
  padding:17px;
  cursor:pointer;
  transition:.2s;
}

.location:hover{
  transform:translateY(-3px);
  box-shadow:var(--shadow);
}

.location .emoji{font-size:28px}
.location h3{margin:10px 0 5px}
.location p{font-size:13px;margin:0;color:var(--muted)}

/* JOBS */
.job{
  border:1px solid var(--border);
  border-radius:15px;
  padding:17px;
  background:white;
}

.job h3{margin-bottom:5px}
.job p{font-size:13px}
.job-meta{
  display:flex;
  gap:8px;
  flex-wrap:wrap;
  margin:12px 0;
}

.tag{
  background:#eef4ef;
  color:var(--green3);
  border-radius:999px;
  padding:5px 9px;
  font-size:11px;
  font-weight:800;
}

/* LOG */
.log{
  display:flex;
  flex-direction:column;
  gap:8px;
  max-height:430px;
  overflow:auto;
}

.log-entry{
  padding:11px 13px;
  border-left:3px solid var(--green3);
  background:#f8faf8;
  border-radius:0 10px 10px 0;
  font-size:13px;
}

.log-entry small{
  display:block;
  color:#8a928b;
  margin-top:3px;
}

/* PROFILE */
.avatar{
  width:82px;
  height:82px;
  border-radius:24px;
  display:grid;
  place-items:center;
  background:linear-gradient(135deg,var(--gold),#ffe08d);
  font-size:42px;
  margin-bottom:14px;
}

.relationship{
  display:flex;
  align-items:center;
  gap:12px;
  padding:12px;
  border:1px solid var(--border);
  border-radius:12px;
}

.rel-avatar{
  width:42px;
  height:42px;
  border-radius:50%;
  background:#eaf0eb;
  display:grid;
  place-items:center;
  font-size:21px;
}

.relationship-main{flex:1}
.relationship-main strong{display:block}
.relationship-main small{color:var(--muted)}

/* EVENT MODAL */
.modal{
  position:fixed;
  inset:0;
  background:rgba(5,16,9,.72);
  backdrop-filter:blur(5px);
  display:flex;
  align-items:center;
  justify-content:center;
  padding:18px;
  z-index:100;
}

.modal-card{
  background:white;
  width:min(600px,100%);
  border-radius:24px;
  padding:27px;
  box-shadow:0 30px 80px rgba(0,0,0,.3);
}

.event-icon{
  font-size:48px;
  margin-bottom:10px;
}

.event-options{
  display:grid;
  gap:10px;
  margin-top:20px;
}

.event-option{
  text-align:left;
  border:1px solid var(--border);
  background:#fafbf9;
  border-radius:13px;
  padding:14px;
}

.event-option:hover{
  background:#f0f6f1;
  border-color:#9ab3a0;
}

.toast{
  position:fixed;
  right:18px;
  bottom:18px;
  background:#102519;
  color:white;
  padding:13px 17px;
  border-radius:12px;
  z-index:200;
  box-shadow:0 12px 30px rgba(0,0,0,.2);
  transform:translateY(100px);
  opacity:0;
  transition:.25s;
  max-width:340px;
}

.toast.show{
  transform:translateY(0);
  opacity:1;
}

/* MOBILE */
.mobile-nav{
  display:none;
}

@media(max-width:900px){
  .game-layout{
    grid-template-columns:1fr;
    padding-bottom:80px;
  }

  .sidebar{display:none}

  .mobile-nav{
    display:flex;
    position:fixed;
    bottom:0;
    left:0;
    right:0;
    z-index:60;
    background:white;
    border-top:1px solid var(--border);
    padding:7px;
    gap:4px;
    overflow-x:auto;
  }

  .mobile-nav button{
    flex:1;
    min-width:72px;
    border:0;
    background:white;
    padding:7px 4px;
    border-radius:9px;
    font-size:10px;
    color:#566158;
  }

  .mobile-nav button.active{
    background:var(--green);
    color:white;
  }

  .location-grid,.three{grid-template-columns:repeat(2,1fr)}
}

@media(max-width:650px){
  .form-grid,.card-grid{grid-template-columns:1fr}
  .full{grid-column:auto}
  .backgrounds{grid-template-columns:1fr}
  .location-grid,.three{grid-template-columns:1fr}
  .header-inner{align-items:flex-start}
  .header-stats{max-width:55%}
  .mini-stat:nth-child(n+4){display:none}
  .stat-row{grid-template-columns:repeat(2,1fr)}
  .page-title{flex-direction:column}
}
</style>
</head>

<body>

<!-- INTRO -->
<section id="intro" class="screen">
  <div class="intro-card">
    <div class="logo-mark">🌿</div>
    <h1>KADUNA<br><span>LIFE</span></h1>
    <div class="tagline">Your Kaduna. Your Story.</div>
    <p class="intro-copy">
      Start with almost nothing. Find your hustle. Make friends.
      Fall in love. Build a business. Survive the unexpected.
      In Kaduna, every choice changes your story.
    </p>
    <button class="primary" onclick="showCreation()">Start Your Life →</button>
  </div>
</section>

<!-- CHARACTER CREATION -->
<section id="creation" class="screen hidden">
  <div class="creation-wrap">
    <div class="top-brand">🌿 KADUNA LIFE</div>

    <div class="creation-card">
      <h2>Create your life</h2>
      <p class="sub">Nobody starts at the top. Where you go from here is up to you.</p>

      <div class="form-grid">

        <div class="field">
          <label>Your name</label>
          <input id="playerName" maxlength="22" placeholder="e.g. Abdul, Grace, Musa...">
        </div>

        <div class="field">
          <label>Age</label>
          <select id="playerAge">
            <option value="18">18</option>
            <option value="19">19</option>
            <option value="20">20</option>
            <option value="21">21</option>
            <option value="22">22</option>
            <option value="23">23</option>
            <option value="24">24</option>
            <option value="25">25</option>
            <option value="26">26</option>
            <option value="27">27</option>
            <option value="28">28</option>
            <option value="29">29</option>
            <option value="30">30</option>
          </select>
        </div>

        <div class="field">
          <label>Gender</label>
          <select id="playerGender">
            <option value="male">Male</option>
            <option value="female">Female</option>
          </select>
        </div>

        <div class="field">
          <label>Starting neighbourhood</label>
          <select id="playerDistrict">
            <option value="Kawo">Kawo</option>
            <option value="Malali">Malali</option>
            <option value="Barnawa">Barnawa</option>
            <option value="Mando">Mando</option>
            <option value="Rigasa">Rigasa</option>
            <option value="Sabon Tasha">Sabon Tasha</option>
            <option value="Ungwan Rimi">Ungwan Rimi</option>
            <option value="Kaduna Central">Kaduna Central</option>
          </select>
        </div>

        <div class="field full">
          <label>Choose your background</label>

          <div class="backgrounds">
            <button class="bg-option selected" data-bg="hustler" onclick="chooseBackground(this,'hustler')">
              <strong>🔥 The Hustler</strong>
              <small>Little money, street sense and high energy. You know how to find an opportunity.</small>
            </button>

            <button class="bg-option" data-bg="student" onclick="chooseBackground(this,'student')">
              <strong>🎓 The Student</strong>
              <small>Smart and ambitious. Start with education and skills, but money is tight.</small>
            </button>

            <button class="bg-option" data-bg="connected" onclick="chooseBackground(this,'connected')">
              <strong>🤝 The Connected One</strong>
              <small>Your family knows people. You start with more money and better connections.</small>
            </button>
          </div>
        </div>

      </div>

      <div class="creation-actions">
        <button class="primary" onclick="startGame()">Enter Kaduna →</button>
      </div>
    </div>
  </div>
</section>

<!-- GAME -->
<section id="game" class="screen hidden">

  <header class="game-header">
    <div class="header-inner">
      <div class="brand">🌿 KADUNA <span>LIFE</span></div>

      <div class="header-stats">
        <div class="mini-stat">
          <span>Cash</span>
          <b id="headerMoney">₦0</b>
        </div>
        <div class="mini-stat">
          <span>Energy</span>
          <b id="headerEnergy">100</b>
        </div>
        <div class="mini-stat">
          <span>Level</span>
          <b id="headerLevel">1</b>
        </div>
        <div class="mini-stat">
          <span>Day</span>
          <b id="headerDay">1</b>
        </div>
      </div>
    </div>
  </header>

  <div class="game-layout">

    <aside class="sidebar">
      <button class="nav-btn active" data-view="home" onclick="navigate('home')">🏠 Home</button>
      <button class="nav-btn" data-view="work" onclick="navigate('work')">💼 Work</button>
      <button class="nav-btn" data-view="city" onclick="navigate('city')">📍 Kaduna</button>
      <button class="nav-btn" data-view="shop" onclick="navigate('shop')">🛒 Shop</button>
      <button class="nav-btn" data-view="people" onclick="navigate('people')">❤️ People</button>
      <button class="nav-btn" data-view="profile" onclick="navigate('profile')">👤 Profile</button>

      <div class="sidebar-divider"></div>

      <button class="nav-btn" onclick="saveGame()">💾 Save Game</button>
      <button class="nav-btn" onclick="loadGame()">↩️ Load Game</button>
      <button class="nav-btn" onclick="newGame()">🔄 New Life</button>
    </aside>

    <main class="content">

      <!-- HOME -->
      <section id="view-home" class="view active">

        <div class="page-title">
          <div>
            <h2 id="welcomeTitle">Good morning.</h2>
            <p id="homeSubtitle">Another day in Kaduna.</p>
          </div>
          <button class="secondary" onclick="nextDay()">🌙 Sleep / Next Day</button>
        </div>

        <div class="card hero-card">
          <div style="display:flex;justify-content:space-between;gap:15px;align-items:flex-start;flex-wrap:wrap">
            <div>
              <small id="homeDistrict">KADUNA</small>
              <h2 id="homeGreeting" style="margin:6px 0">Welcome home.</h2>
              <p id="homeQuote">Every day is another chance to change your story.</p>
            </div>

            <div>
              <small>Cash</small>
              <div class="big-money" id="homeMoney">₦0</div>
            </div>
          </div>
        </div>

        <div style="height:15px"></div>

        <div class="stat-row" id="needsStats"></div>

        <div style="height:15px"></div>

        <div class="card-grid">

          <div class="card">
            <h3>⚡ Today's actions</h3>
            <p>Spend your energy wisely. Most actions advance time and affect your needs.</p>

            <div class="action-list">
              <div class="action">
                <div class="action-info">
                  <strong>🍛 Eat local food</strong>
                  <small>+25 hunger · ₦1,500</small>
                </div>
                <button class="secondary" onclick="eat()">Eat</button>
              </div>

              <div class="action">
                <div class="action-info">
                  <strong>🛋️ Rest</strong>
                  <small>+20 energy</small>
                </div>
                <button class="secondary" onclick="rest()">Rest</button>
              </div>

              <div class="action">
                <div class="action-info">
                  <strong>🎮 Chill</strong>
                  <small>+12 happiness · -10 energy</small>
                </div>
                <button class="secondary" onclick="chill()">Chill</button>
              </div>
            </div>
          </div>

          <div class="card">
            <h3>📜 Life log</h3>
            <div id="lifeLog" class="log"></div>
          </div>

        </div>
      </section>

      <!-- WORK -->
      <section id="view-work" class="view">
        <div class="page-title">
          <div>
            <h2>Work & Hustle</h2>
            <p>Find your money. Build your career.</p>
          </div>
        </div>

        <div class="card hero-card" style="margin-bottom:15px">
          <small>CURRENT CAREER</small>
          <h2 id="currentJob" style="margin:6px 0">Unemployed</h2>
          <p id="currentJobText">Everybody starts somewhere.</p>
        </div>

        <div class="card-grid" id="jobsList"></div>
      </section>

      <!-- CITY -->
      <section id="view-city" class="view">
        <div class="page-title">
          <div>
            <h2>Explore Kaduna</h2>
            <p>Different places. Different people. Different opportunities.</p>
          </div>
        </div>

        <div class="location-grid" id="locationsList"></div>
      </section>

      <!-- SHOP -->
      <section id="view-shop" class="view">
        <div class="page-title">
          <div>
            <h2>Market</h2>
            <p>Spend money to improve your life.</p>
          </div>
        </div>

        <div class="card-grid" id="shopList"></div>
      </section>

      <!-- PEOPLE -->
      <section id="view-people" class="view">
        <div class="page-title">
          <div>
            <h2>Your People</h2>
            <p>Life is easier when you know the right people.</p>
          </div>
        </div>

        <div class="card-grid" id="peopleList"></div>
      </section>

      <!-- PROFILE -->
      <section id="view-profile" class="view">
        <div class="page-title">
          <div>
            <h2>Your Life</h2>
            <p>Your stats, progress and achievements.</p>
          </div>
        </div>

        <div class="card-grid">

          <div class="card">
            <div class="avatar" id="profileAvatar">🧑🏾</div>
            <h2 id="profileName">Player</h2>
            <p id="profileBackground">The Hustler</p>

            <div class="stat-row">
              <div class="stat-box">
                <small>Age</small>
                <strong id="profileAge">18</strong>
              </div>
              <div class="stat-box">
                <small>Level</small>
                <strong id="profileLevel">1</strong>
              </div>
              <div class="stat-box">
                <small>XP</small>
                <strong id="profileXP">0</strong>
              </div>
            </div>
          </div>

          <div class="card">
            <h3>⭐ Progress</h3>

            <p style="margin-bottom:4px">Level progress</p>
            <div class="progress"><i id="xpBar" style="width:0%"></i></div>
            <small id="xpText" style="color:var(--muted)">0 / 100 XP</small>

            <div style="height:20px"></div>

            <h3>🏆 Achievements</h3>
            <div id="achievements"></div>
          </div>

        </div>
      </section>

    </main>
  </div>

  <nav class="mobile-nav">
    <button class="active" data-view="home" onclick="navigate('home')">🏠<br>Home</button>
    <button data-view="work" onclick="navigate('work')">💼<br>Work</button>
    <button data-view="city" onclick="navigate('city')">📍<br>City</button>
    <button data-view="shop" onclick="navigate('shop')">🛒<br>Shop</button>
    <button data-view="people" onclick="navigate('people')">❤️<br>People</button>
    <button data-view="profile" onclick="navigate('profile')">👤<br>Me</button>
  </nav>
</section>

<!-- EVENT MODAL -->
<div id="eventModal" class="modal hidden">
  <div class="modal-card">
    <div class="event-icon" id="eventIcon">✨</div>
    <h2 id="eventTitle">Something happened</h2>
    <p id="eventText"></p>
    <div id="eventOptions" class="event-options"></div>
  </div>
</div>

<div id="toast" class="toast"></div>

<script>
/* =========================================================
   KADUNA LIFE V6
   Single-file game engine
========================================================= */

const SAVE_KEY = "kadunaLifeV6";

let selectedBackground = "hustler";

let player = {
  name:"",
  age:18,
  gender:"male",
  district:"Kawo",
  background:"hustler",

  money:5000,
  energy:80,
  hunger:75,
  health:85,
  happiness:65,
  reputation:10,

  level:1,
  xp:0,

  day:1,
  job:null,
  home:"Shared Room",
  homeLevel:0,

  skills:{
    business:1,
    tech:1,
    social:1,
    street:1,
    career:1
  },

  inventory:[],
  relationships:{
    amina:20,
    musa:15,
    daniel:10,
    zainab:5
  },

  achievements:[],
  visited:[],
  log:[]
};

const jobs = [
  {
    id:"delivery",
    title:"Dispatch Rider",
    icon:"🏍️",
    pay:8500,
    energy:28,
    skill:"street",
    desc:"Move around Kaduna delivering food and packages."
  },
  {
    id:"designer",
    title:"Freelance Designer",
    icon:"💻",
    pay:12000,
    energy:22,
    skill:"tech",
    desc:"Find clients online and design from your phone or laptop."
  },
  {
    id:"teacher",
    title:"Private Tutor",
    icon:"📚",
    pay:9500,
    energy:25,
    skill:"career",
    desc:"Teach students around the city."
  },
  {
    id:"trader",
    title:"Market Trader",
    icon:"🛍️",
    pay:10500,
    energy:30,
    skill:"business",
    desc:"Buy low, sell high and learn the Kaduna market."
  },
  {
    id:"creator",
    title:"Content Creator",
    icon:"📱",
    pay:6500,
    energy:20,
    skill:"social",
    desc:"Turn Kaduna stories into content."
  },
  {
    id:"office",
    title:"Office Assistant",
    icon:"🧾",
    pay:11500,
    energy:27,
    skill:"career",
    desc:"A steady job with room for promotion."
  }
];

const locations = [
  {
    id:"kawo",
    name:"Kawo",
    emoji:"🚌",
    text:"Busy roads, transport and endless movement.",
    action:"Transport hustle",
    reward:5000,
    energy:18,
    xp:10
  },
  {
    id:"central",
    name:"Kaduna Central",
    emoji:"🏙️",
    text:"The heart of the city. Shops, offices and opportunities.",
    action:"Network",
    reward:3500,
    energy:12,
    xp:14
  },
  {
    id:"malali",
    name:"Malali",
    emoji:"🌳",
    text:"A quieter side of Kaduna with room to breathe.",
    action:"Relax & network",
    reward:0,
    energy:5,
    xp:8
  },
  {
    id:"barnawa",
    name:"Barnawa",
    emoji:"🏘️",
    text:"Residential streets, businesses and local life.",
    action:"Find customers",
    reward:6500,
    energy:18,
    xp:12
  },
  {
    id:"mando",
    name:"Mando",
    emoji:"🎓",
    text:"Students, schools and young people chasing their future.",
    action:"Meet students",
    reward:3000,
    energy:15,
    xp:12
  },
  {
    id:"rigasa",
    name:"Rigasa",
    emoji:"🚉",
    text:"A huge community where opportunity can appear anywhere.",
    action:"Find a hustle",
    reward:7500,
    energy:25,
    xp:16
  },
  {
    id:"sabon",
    name:"Sabon Tasha",
    emoji:"🍲",
    text:"Food, commerce and plenty of neighbourhood stories.",
    action:"Sell something",
    reward:6000,
    energy:20,
    xp:13
  },
  {
    id:"ungwan",
    name:"Ungwan Rimi",
    emoji:"🏡",
    text:"Community, families and people who know people.",
    action:"Build connections",
    reward:2500,
    energy:10,
    xp:15
  }
];

const shopItems = [
  {
    id:"phone",
    name:"Better Smartphone",
    icon:"📱",
    price:45000,
    desc:"+2 social skill. Better opportunities online."
  },
  {
    id:"clothes",
    name:"Fresh Outfit",
    icon:"👕",
    price:18000,
    desc:"+5 happiness. +2 reputation."
  },
  {
    id:"laptop",
    name:"Used Laptop",
    icon:"💻",
    price:95000,
    desc:"+2 tech skill. Unlocks better freelance work."
  },
  {
    id:"bike",
    name:"Motorbike",
    icon:"🏍️",
    price:240000,
    desc:"Unlocks faster transport hustles."
  },
  {
    id:"generator",
    name:"Small Generator",
    icon:"⚡",
    price:85000,
    desc:"+5 happiness and better home comfort."
  },
  {
    id:"tv",
    name:"Smart TV",
    icon:"📺",
    price:120000,
    desc:"+8 happiness at home."
  }
];

const people = [
  {
    id:"amina",
    name:"Amina",
    emoji:"👩🏾",
    role:"University student",
    text:"Smart, ambitious and always knows what's happening around Kaduna."
  },
  {
    id:"musa",
    name:"Musa",
    emoji:"👨🏾",
    role:"Business-minded friend",
    text:"Always looking for the next business opportunity."
  },
  {
    id:"daniel",
    name:"Daniel",
    emoji:"🧑🏾",
    role:"Creative friend",
    text:"Knows music, events and the creative scene."
  },
  {
    id:"zainab",
    name:"Zainab",
    emoji:"👩🏾‍💼",
    role:"Young professional",
    text:"Focused, connected and difficult to impress."
  }
];

const randomEvents = [
  {
    icon:"📱",
    title:"Your post goes viral",
    text:"A short video you posted about life in Kaduna suddenly starts getting attention.",
    options:[
      {label:"Keep posting",money:7000,xp:18,happiness:8,reputation:5},
      {label:"Use the attention to promote a business",money:14000,xp:25,reputation:8},
      {label:"Ignore it",happiness:-2}
    ]
  },
  {
    icon:"🤝",
    title:"A friend needs help",
    text:"Someone you know has an urgent problem and asks you for money.",
    options:[
      {label:"Help with ₦5,000",money:-5000,reputation:8,happiness:5,relationship:5},
      {label:"Give advice instead",reputation:3,xp:8},
      {label:"Stay out of it",reputation:-3}
    ]
  },
  {
    icon:"💼",
    title:"Unexpected opportunity",
    text:"Someone offers you a small job. It could lead to something bigger.",
    options:[
      {label:"Take the opportunity",money:10000,xp:20,energy:-18},
      {label:"Negotiate first",money:15000,xp:25,reputation:3,energy:-22},
      {label:"Decline",energy:5}
    ]
  },
  {
    icon:"🚗",
    title:"Transport wahala",
    text:"Your plans are delayed because your transport arrangement falls apart.",
    options:[
      {label:"Pay for another ride",money:-2500,energy:-5},
      {label:"Wait it out",energy:-15,happiness:-5},
      {label:"Walk",energy:-22,health:-2,xp:5}
    ]
  },
  {
    icon:"🎉",
    title:"You're invited out",
    text:"Your friends are going out tonight. You need a little money to join.",
    options:[
      {label:"Go out",money:-6000,happiness:15,energy:-15,reputation:3},
      {label:"Join for a little while",money:-2500,happiness:8,energy:-8},
      {label:"Stay home",money:0}
    ]
  },
  {
    icon:"🏪",
    title:"Business opportunity",
    text:"A small local business needs someone to help them sell online.",
    options:[
      {label:"Take the deal",money:18000,xp:30,energy:-25},
      {label:"Ask for a better deal",money:26000,xp:35,energy:-30,reputation:4},
      {label:"Pass",xp:4}
    ]
  }
];

/* ---------- BASIC UI ---------- */

function showCreation(){
  document.getElementById("intro").classList.add("hidden");
  document.getElementById("creation").classList.remove("hidden");
}

function chooseBackground(el,bg){
  document.querySelectorAll(".bg-option").forEach(x=>x.classList.remove("selected"));
  el.classList.add("selected");
  selectedBackground=bg;
}

function startGame(){
  const name=document.getElementById("playerName").value.trim();

  if(!name){
    toast("Enter your name first.");
    return;
  }

  player.name=name;
  player.age=Number(document.getElementById("playerAge").value);
  player.gender=document.getElementById("playerGender").value;
  player.district=document.getElementById("playerDistrict").value;
  player.background=selectedBackground;

  applyBackground();

  player.log=[];
  addLog(`You arrived in ${player.district}. Your Kaduna story begins.`);

  document.getElementById("creation").classList.add("hidden");
  document.getElementById("game").classList.remove("hidden");

  renderAll();
  toast("Welcome to Kaduna Life, "+player.name+"!");
}

function applyBackground(){
  if(player.background==="hustler"){
    player.money=5000;
    player.energy=90;
    player.street=2;
    player.skills.street=2;
    player.skills.business=2;
    player.happiness=65;
  }

  if(player.background==="student"){
    player.money=3500;
    player.energy=90;
    player.skills.tech=2;
    player.skills.career=2;
    player.happiness=72;
  }

  if(player.background==="connected"){
    player.money=30000;
    player.energy=80;
    player.reputation=25;
    player.skills.social=3;
    player.skills.business=2;
    player.happiness=75;
  }
}

/* ---------- NAVIGATION ---------- */

function navigate(view){
  document.querySelectorAll(".view").forEach(v=>v.classList.remove("active"));
  document.getElementById("view-"+view).classList.add("active");

  document.querySelectorAll(".nav-btn,.mobile-nav button").forEach(b=>{
    b.classList.toggle("active",b.dataset.view===view);
  });

  if(view==="work") renderJobs();
  if(view==="city") renderLocations();
  if(view==="shop") renderShop();
  if(view==="people") renderPeople();
  if(view==="profile") renderProfile();

  window.scrollTo({top:0,behavior:"smooth"});
}

/* ---------- STATS ---------- */

function clamp(v,min=0,max=100){
  return Math.max(min,Math.min(max,v));
}

function money(n){
  return "₦"+Math.max(0,Math.round(n)).toLocaleString();
}

function change(stat,value){
  if(typeof player[stat]!=="number") return;
  player[stat]+=value;

  if(["energy","hunger","health","happiness","reputation"].includes(stat)){
    player[stat]=clamp(player[stat]);
  }

  if(stat==="money"){
    player.money=Math.max(0,player.money);
  }
}

function gainXP(amount){
  player.xp+=amount;

  let needed=100+(player.level-1)*50;

  while(player.xp>=needed){
    player.xp-=needed;
    player.level++;
    player.energy=clamp(player.energy+10);
    player.health=clamp(player.health+5);
    player.happiness=clamp(player.happiness+5);

    addLog(`🎉 You reached Level ${player.level}! Your abilities improved.`);
    toast(`Level ${player.level} reached!`);

    needed=100+(player.level-1)*50;
  }
}

function useEnergy(amount){
  if(player.energy<amount){
    toast("You're too tired. Rest first.");
    return false;
  }

  player.energy-=amount;
  player.energy=clamp(player.energy);
  return true;
}

/* ---------- HOME ACTIONS ---------- */

function eat(){
  if(player.money<1500){
    toast("You need ₦1,500 to eat.");
    return;
  }

  player.money-=1500;
  player.hunger=clamp(player.hunger+25);
  player.health=clamp(player.health+3);
  addLog("🍛 You ate a proper meal.");
  renderAll();
}

function rest(){
  player.energy=clamp(player.energy+20);
  player.hunger=clamp(player.hunger-5);
  addLog("🛋️ You rested and recovered some energy.");
  renderAll();
}

function chill(){
  if(!useEnergy(10)) return;

  player.happiness=clamp(player.happiness+12);
  player.hunger=clamp(player.hunger-5);
  addLog("🎮 You chilled for a while.");
  renderAll();
}

/* ---------- WORK ---------- */

function renderJobs(){
  const box=document.getElementById("jobsList");

  document.getElementById("currentJob").textContent =
    player.job ? player.job.title : "Unemployed";

  document.getElementById("currentJobText").textContent =
    player.job
      ? `You currently earn around ${money(player.job.pay)} per work day.`
      : "Find something that fits your story.";

  box.innerHTML=jobs.map(job=>{
    const skill=player.skills[job.skill]||1;
    const bonus=1+(skill-1)*.08;
    const earnings=Math.round(job.pay*bonus);

    return `
      <div class="job">
        <div style="font-size:30px">${job.icon}</div>
        <h3>${job.title}</h3>
        <p>${job.desc}</p>

        <div class="job-meta">
          <span class="tag">💰 ${money(earnings)}</span>
          <span class="tag">⚡ -${job.energy}</span>
          <span class="tag">⭐ ${job.skill} Lv.${skill}</span>
        </div>

        <button class="secondary" onclick="work('${job.id}')">
          ${player.job && player.job.id===job.id ? "Work today" : "Take job"}
        </button>
      </div>
    `;
  }).join("");
}

function work(id){
  const job=jobs.find(j=>j.id===id);
  if(!job) return;

  if(!useEnergy(job.energy)) return;

  player.job=job;

  const skill=player.skills[job.skill]||1;
  const earnings=Math.round(job.pay*(1+(skill-1)*.08));

  player.money+=earnings;
  player.hunger=clamp(player.hunger-10);
  player.happiness=clamp(player.happiness-2);
  player.reputation=clamp(player.reputation+1);

  player.skills[job.skill]=skill+0.15;

  gainXP(18);
  addLog(`💼 You worked as a ${job.title} and earned ${money(earnings)}.`);

  maybeEvent();
  renderAll();
}

/* ---------- CITY ---------- */

function renderLocations(){
  document.getElementById("locationsList").innerHTML=
    locations.map(loc=>`
      <div class="location" onclick="visitLocation('${loc.id}')">
        <div class="emoji">${loc.emoji}</div>
        <h3>${loc.name}</h3>
        <p>${loc.text}</p>
        <div style="margin-top:12px">
          <span class="tag">${loc.action}</span>
        </div>
      </div>
    `).join("");
}

function visitLocation(id){
  const loc=locations.find(x=>x.id===id);
  if(!loc) return;

  if(!useEnergy(loc.energy)) return;

  player.district=loc.name;

  if(!player.visited.includes(loc.id)){
    player.visited.push(loc.id);
    gainXP(10);
  }

  if(loc.reward){
    const variation=Math.floor(Math.random()*3000);
    const reward=loc.reward+variation;
    player.money+=reward;
    addLog(`📍 You visited ${loc.name} and made ${money(reward)}.`);
  }else{
    player.happiness=clamp(player.happiness+8);
    addLog(`📍 You spent time around ${loc.name}.`);
  }

  gainXP(loc.xp);
  maybeEvent(.15);
  renderAll();
  navigate("home");
}

/* ---------- SHOP ---------- */

function renderShop(){
  document.getElementById("shopList").innerHTML=
    shopItems.map(item=>{
      const owned=player.inventory.includes(item.id);

      return `
        <div class="card">
          <div style="font-size:35px">${item.icon}</div>
          <h3>${item.name}</h3>
          <p>${item.desc}</p>
          <div style="font-weight:900;margin:12px 0">${money(item.price)}</div>

          <button
            class="${owned?'secondary':'primary'}"
            ${owned?'disabled':''}
            onclick="buyItem('${item.id}')">
            ${owned?"Owned":"Buy"}
          </button>
        </div>
      `;
    }).join("");
}

function buyItem(id){
  const item=shopItems.find(x=>x.id===id);

  if(!item) return;

  if(player.inventory.includes(id)){
    toast("You already own this.");
    return;
  }

  if(player.money<item.price){
    toast("You can't afford this yet.");
    return;
  }

  player.money-=item.price;
  player.inventory.push(id);

  if(id==="phone"){
    player.skills.social+=2;
    player.reputation=clamp(player.reputation+3);
  }

  if(id==="clothes"){
    player.happiness=clamp(player.happiness+5);
    player.reputation=clamp(player.reputation+2);
  }

  if(id==="laptop"){
    player.skills.tech+=2;
  }

  if(id==="bike"){
    player.skills.street+=2;
  }

  if(id==="generator"){
    player.happiness=clamp(player.happiness+5);
  }

  if(id==="tv"){
    player.happiness=clamp(player.happiness+8);
  }

  addLog(`🛒 You bought ${item.name} for ${money(item.price)}.`);
  checkAchievements();
  renderAll();
}

/* ---------- PEOPLE ---------- */

function renderPeople(){
  document.getElementById("peopleList").innerHTML=
    people.map(person=>{
      const rel=player.relationships[person.id]||0;
      const percent=clamp(rel);

      return `
        <div class="card">
          <div class="relationship">
            <div class="rel-avatar">${person.emoji}</div>
            <div class="relationship-main">
              <strong>${person.name}</strong>
              <small>${person.role}</small>
            </div>
          </div>

          <p>${person.text}</p>

          <div class="progress">
            <i style="width:${percent}%"></i>
          </div>

          <small style="color:var(--muted)">Relationship: ${percent}/100</small>

          <div style="height:12px"></div>

          <button class="secondary" onclick="spendTime('${person.id}')">
            Spend time
          </button>
        </div>
      `;
    }).join("");
}

function spendTime(id){
  if(!useEnergy(12)) return;

  const person=people.find(x=>x.id===id);
  if(!person) return;

  const gain=5+Math.floor(Math.random()*6);

  player.relationships[id]=clamp((player.relationships[id]||0)+gain);
  player.happiness=clamp(player.happiness+7);

  gainXP(10);

  addLog(`❤️ You spent time with ${person.name}. Your relationship improved.`);

  if(player.relationships[id]>=50){
    player.reputation=clamp(player.reputation+2);
  }

  renderAll();
}

/* ---------- DAY / LIFE ---------- */

function nextDay(){
  player.day++;
  player.age += player.day%365===0 ? 1 : 0;

  player.energy=clamp(85);
  player.hunger=clamp(player.hunger-12);
  player.health=clamp(player.health-2);

  if(player.homeLevel===0){
    player.money=Math.max(0,player.money-2500);
    addLog("🏠 You paid ₦2,500 toward your shared room and basic expenses.");
  }

  if(player.homeLevel===1){
    player.money=Math.max(0,player.money-6500);
    addLog("🏠 You paid ₦6,500 in rent and bills.");
  }

  if(player.homeLevel===2){
    player.money=Math.max(0,player.money-15000);
    addLog("🏠 You paid ₦15,000 in rent and bills.");
  }

  if(player.homeLevel===3){
    player.money=Math.max(0,player.money-30000);
    addLog("🏠 You paid ₦30,000 in home expenses.");
  }

  if(player.hunger<20){
    player.health=clamp(player.health-8);
    addLog("⚠️ You're getting dangerously hungry.");
  }

  if(player.health<20){
    player.happiness=clamp(player.happiness-10);
  }

  addLog(`🌅 Day ${player.day}: A new day in Kaduna.`);

  gainXP(5);

  maybeEvent(.45);
  checkAchievements();
  renderAll();
}

/* ---------- RANDOM EVENTS ---------- */

function maybeEvent(chance=.3){
  if(Math.random()>chance) return;

  const event=randomEvents[Math.floor(Math.random()*randomEvents.length)];

  showEvent(event);
}

function showEvent(event){
  document.getElementById("eventIcon").textContent=event.icon;
  document.getElementById("eventTitle").textContent=event.title;
  document.getElementById("eventText").textContent=event.text;

  document.getElementById("eventOptions").innerHTML=
    event.options.map((option,i)=>`
      <button class="event-option" onclick="resolveEvent(${JSON.stringify(option).replace(/"/g,'&quot;')})">
        <strong>${option.label}</strong>
      </button>
    `).join("");

  document.getElementById("eventModal").classList.remove("hidden");
}

function resolveEvent(option){
  document.getElementById("eventModal").classList.add("hidden");

  for(const key of ["money","energy","hunger","health","happiness","reputation"]){
    if(option[key]) change(key,option[key]);
  }

  if(option.xp) gainXP(option.xp);

  if(option.relationship){
    const ids=Object.keys(player.relationships);
    const id=ids[Math.floor(Math.random()*ids.length)];
    player.relationships[id]=clamp(player.relationships[id]+option.relationship);
  }

  addLog(`✨ ${option.label}.`);
  checkAchievements();
  renderAll();
}

/* ---------- PROFILE / ACHIEVEMENTS ---------- */

function renderProfile(){
  const avatar=player.gender==="female"?"👩🏾":"👨🏾";

  document.getElementById("profileAvatar").textContent=avatar;
  document.getElementById("profileName").textContent=player.name;
  document.getElementById("profileBackground").textContent=
    backgroundName(player.background)+" · "+player.district;

  document.getElementById("profileAge").textContent=player.age;
  document.getElementById("profileLevel").textContent=player.level;
  document.getElementById("profileXP").textContent=Math.floor(player.xp);

  const needed=100+(player.level-1)*50;
  const pct=(player.xp/needed)*100;

  document.getElementById("xpBar").style.width=pct+"%";
  document.getElementById("xpText").textContent=
    `${Math.floor(player.xp)} / ${needed} XP`;

  renderAchievements();
}

function backgroundName(bg){
  return {
    hustler:"The Hustler",
    student:"The Student",
    connected:"The Connected One"
  }[bg]||"Unknown";
}

function renderAchievements(){
  const all=[
    ["firstDay","🌅 First Day","Survive your first day.",player.day>=2],
    ["firstJob","💼 First Hustle","Earn money from work.",!!player.job],
    ["tenK","💰 Ten Grand","Have ₦10,000.",player.money>=10000],
    ["fiftyK","💵 Fifty Grand","Have ₦50,000.",player.money>=50000],
    ["level5","⭐ Rising Star","Reach level 5.",player.level>=5],
    ["explorer","📍 Explorer","Visit 5 different areas.",player.visited.length>=5],
    ["social","❤️ People Person","Reach 50 relationship with someone.",Object.values(player.relationships).some(v=>v>=50)],
    ["million","👑 Big Player","Build ₦1,000,000.",player.money>=1000000]
  ];

  document.getElementById("achievements").innerHTML=
    all.map(a=>`
      <div style="
        padding:10px;
        border:1px solid ${a[3]?'#cbdccf':'var(--border)'};
        background:${a[3]?'#f0f7f1':'#fafafa'};
        border-radius:10px;
        margin-bottom:8px;
        opacity:${a[3]?1:.55};
      ">
        <strong>${a[1]}</strong>
        <small style="display:block;color:var(--muted)">${a[2]}</small>
      </div>
    `).join("");
}

function checkAchievements(){
  renderProfile();
}

/* ---------- LOG / RENDER ---------- */

function addLog(text){
  player.log.unshift({
    text,
    day:player.day,
    time:new Date().toLocaleTimeString([],{
      hour:"2-digit",
      minute:"2-digit"
    })
  });

  player.log=player.log.slice(0,50);
}

function renderLog(){
  const box=document.getElementById("lifeLog");

  if(!player.log.length){
    box.innerHTML=`<div class="log-entry">Your story hasn't started yet.</div>`;
    return;
  }

  box.innerHTML=player.log.map(x=>`
    <div class="log-entry">
      ${x.text}
      <small>Day ${x.day} · ${x.time}</small>
    </div>
  `).join("");
}

function renderNeeds(){
  const stats=[
    ["🍛","Hunger",player.hunger],
    ["⚡","Energy",player.energy],
    ["❤️","Health",player.health],
    ["😊","Happiness",player.happiness],
    ["⭐","Reputation",player.reputation],
    ["💰","Cash",null]
  ];

  document.getElementById("needsStats").innerHTML=
    stats.map(s=>{
      if(s[2]===null){
        return `
          <div class="stat-box">
            <small>${s[0]} ${s[1]}</small>
            <strong class="money">${money(player.money)}</strong>
          </div>
        `;
      }

      return `
        <div class="stat-box">
          <small>${s[0]} ${s[1]}</small>
          <strong>${Math.round(s[2])}</strong>
          <div class="progress">
            <i style="width:${s[2]}%;background:${s[2]<25?'#c94b4b':'var(--green3)'}"></i>
          </div>
        </div>
      `;
    }).join("");
}

function renderHome(){
  const hour=player.day%2===0?"Good morning":"Good evening";

  document.getElementById("welcomeTitle").textContent=
    `${hour}, ${player.name}.`;

  document.getElementById("homeSubtitle").textContent=
    `Day ${player.day} · ${player.district}`;

  document.getElementById("homeDistrict").textContent=
    player.district.toUpperCase();

  document.getElementById("homeGreeting").textContent=
    player.job
      ? `${player.job.title} · Keep moving.`
      : "Your story is just beginning.";

  document.getElementById("homeQuote").textContent=
    randomQuote();

  document.getElementById("homeMoney").textContent=money(player.money);
}

function randomQuote(){
  const quotes=[
    "Small moves become big stories.",
    "Kaduna is full of people chasing something.",
    "One good opportunity can change everything.",
    "Your network can become your net worth.",
    "No matter where you start, you can build something.",
    "Today might be the day everything changes."
  ];

  return quotes[Math.floor(Math.random()*quotes.length)];
}

function renderHeader(){
  document.getElementById("headerMoney").textContent=money(player.money);
  document.getElementById("headerEnergy").textContent=Math.round(player.energy);
  document.getElementById("headerLevel").textContent=player.level;
  document.getElementById("headerDay").textContent=player.day;
}

function renderAll(){
  renderHeader();
  renderHome();
  renderNeeds();
  renderLog();
  renderJobs();
  renderLocations();
  renderShop();
  renderPeople();
  renderProfile();
}

/* ---------- SAVE ---------- */

function saveGame(){
  try{
    localStorage.setItem(SAVE_KEY,JSON.stringify(player));
    toast("Game saved successfully.");
  }catch(e){
    toast("Could not save the game.");
  }
}

function loadGame(){
  try{
    const saved=localStorage.getItem(SAVE_KEY);

    if(!saved){
      toast("No saved game found.");
      return;
    }

    player=JSON.parse(saved);

    document.getElementById("intro").classList.add("hidden");
    document.getElementById("creation").classList.add("hidden");
    document.getElementById("game").classList.remove("hidden");

    renderAll();
    toast("Saved game loaded.");
  }catch(e){
    toast("Could not load the saved game.");
  }
}

function newGame(){
  if(!confirm("Start a completely new life? Your current local save will be replaced.")){
    return;
  }

  localStorage.removeItem(SAVE_KEY);
  location.reload();
}

/* ---------- TOAST ---------- */

let toastTimer;

function toast(message){
  const el=document.getElementById("toast");

  el.textContent=message;
  el.classList.add("show");

  clearTimeout(toastTimer);

  toastTimer=setTimeout(()=>{
    el.classList.remove("show");
  },2600);
}

/* ---------- STARTUP ---------- */

(function init(){
  const saved=localStorage.getItem(SAVE_KEY);

  if(saved){
    try{
      const data=JSON.parse(saved);

      if(data && data.name){
        const continueGame=confirm(
          `Continue your Kaduna Life as ${data.name}?`
        );

        if(continueGame){
          player=data;

          document.getElementById("intro").classList.add("hidden");
          document.getElementById("game").classList.remove("hidden");

          renderAll();
          return;
        }
      }
    }catch(e){}
  }
})();
</script>

</body>
</html>
