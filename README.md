<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<title>Coupe du Monde FIFA 2026</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
*{box-sizing:border-box}
body{
  margin:0;
  width:100vw;
  height:100vh;
  overflow:hidden;
  font-family:Arial Black,Arial,sans-serif;
  color:#fff;
  background:radial-gradient(circle at top,#062b68,#020814 55%,#000);
}
body:before{
  content:"";
  position:fixed;inset:0;
  background:
  radial-gradient(circle at 8% 10%,rgba(255,190,40,.35),transparent 12%),
  radial-gradient(circle at 90% 88%,rgba(0,120,255,.35),transparent 18%),
  linear-gradient(135deg,rgba(0,140,255,.14),transparent 45%);
  pointer-events:none;
}
.wrap{width:100vw;height:100vh;padding:24px 34px;position:relative}
.top{height:150px;display:grid;grid-template-columns:1fr 480px 150px;gap:25px;align-items:center}
.logo{font-size:82px;float:left;margin-right:25px}
h1{font-size:64px;margin:0;letter-spacing:3px;text-shadow:0 0 18px #000}
.gold{color:#ffd24a}
.sub{font-size:28px;color:#e5f2ff;margin-top:8px}
.clock{
  border:2px solid #096fe8;border-radius:24px;padding:18px;text-align:center;
  background:rgba(0,15,45,.85);box-shadow:0 0 25px #005dff88
}
#time{font-size:58px}
#date{font-size:26px;color:#ffd24a}
.trophy{font-size:80px;text-align:center}

.grid{
  display:grid;
  grid-template-columns:31% 24% 45%;
  grid-template-rows:520px 210px;
  gap:18px;
}
.card{
  background:rgba(0,12,34,.88);
  border:2px solid #0077ff;
  border-radius:22px;
  box-shadow:0 0 25px #006cff55;
  overflow:hidden;
}
.head{
  height:66px;padding:14px 24px;font-size:30px;
  background:linear-gradient(110deg,#d00000,#870000 70%,#001b55);
}
.blue{background:linear-gradient(110deg,#063fd1,#001949)}
.purple{background:linear-gradient(110deg,#9d00ff,#230064 65%,#001949)}
.match{height:151px;border-bottom:1px solid #ffffff22;padding:18px}
.line{display:grid;grid-template-columns:1fr 160px 1fr;align-items:center;text-align:center}
.flag{font-size:54px}
.name{font-size:18px;margin-top:8px}
.score{font-size:54px}
.live{background:#d50000;border-radius:20px;padding:6px 16px;display:inline-block;margin-top:7px;font-size:16px}

.fixture{height:108px;border-bottom:1px solid #ffffff22;display:grid;grid-template-columns:80px 1fr 45px 1fr;align-items:center;padding:12px 18px;font-size:18px}
.dateMatch{color:#27b7ff;font-size:18px}
.vs{color:#aaa;text-align:center}

.standing{padding:24px}
.groupTitle{text-align:center;color:#ffd24a;font-size:40px;margin:5px 0 18px}
table{width:100%;border-collapse:collapse;font-size:22px}
td,th{padding:12px;border-bottom:1px solid #ffffff22;text-align:center}
.team{text-align:left}
.pts{background:#8a16e8;border-radius:8px;padding:5px 13px;font-size:28px}
.tabs{text-align:center;margin-top:16px}
.tab{display:inline-block;border:1px solid #187cff;border-radius:8px;padding:8px 13px;margin:4px;background:#001b46;color:#ddd}
.active{background:#8a16e8;color:white;box-shadow:0 0 16px #d100ff}

.bottom1{grid-column:1/2}
.bottom2{grid-column:2/3}
.bottom3{grid-column:3/4}
.boxContent{text-align:center;padding:25px}
.big{font-size:28px;color:#ffd24a;margin-bottom:18px}
.info{font-size:26px}
.footer{position:absolute;bottom:8px;width:100%;left:0;text-align:center;color:#49b9ff;font-size:19px}
</style>
</head>
<body>
<div class="wrap">
  <div class="top">
    <div>
      <div class="logo">🏆</div>
      <h1>COUPE DU MONDE <span class="gold">FIFA 2026</span></h1>
      <div class="sub">⚽ SCORES EN DIRECT • PROCHAINS MATCHS • CLASSEMENTS</div>
    </div>
    <div class="clock">
      <div id="time">--:--</div>
      <div id="date">--</div>
    </div>
    <div class="trophy">🏆</div>
  </div>

  <div class="grid">
    <div class="card">
      <div class="head">⚡ MATCHS EN DIRECT</div>
      <div class="match"><div class="line"><div><div class="flag">🏴</div><div class="name">ANGLETERRE</div></div><div><div class="score">0 - 0</div><div class="live">EN DIRECT 45'</div></div><div><div class="flag">🇭🇷</div><div class="name">CROATIE</div></div></div></div>
      <div class="match"><div class="line"><div><div class="flag">🇲🇦</div><div class="name">MAROC</div></div><div><div class="score"><span style="color:#26ff52">2</span> - 1</div><div class="live">EN DIRECT 67'</div></div><div><div class="flag">🇺🇸</div><div class="name">ÉTATS-UNIS</div></div></div></div>
      <div class="match"><div class="line"><div><div class="flag">🇯🇵</div><div class="name">JAPON</div></div><div><div class="score"><span style="color:#26ff52">1</span> - 0</div><div class="live">EN DIRECT 32'</div></div><div><div class="flag">🇸🇳</div><div class="name">SÉNÉGAL</div></div></div></div>
    </div>

    <div class="card">
      <div class="head blue">📅 PROCHAINS MATCHS</div>
      <div class="fixture"><div class="dateMatch">18 JUIN<br>18:00</div><div>🇨🇭 SUISSE</div><div class="vs">VS</div><div>🇧🇦 BOSNIE</div></div>
      <div class="fixture"><div class="dateMatch">18 JUIN<br>21:00</div><div>🇨🇦 CANADA</div><div class="vs">VS</div><div>🇶🇦 QATAR</div></div>
      <div class="fixture"><div class="dateMatch">19 JUIN<br>00:00</div><div>🇲🇽 MEXIQUE</div><div class="vs">VS</div><div>🇰🇷 CORÉE</div></div>
      <div class="fixture"><div class="dateMatch">19 JUIN<br>03:00</div><div>🇧🇷 BRÉSIL</div><div class="vs">VS</div><div>🇦🇺 AUSTRALIE</div></div>
    </div>

    <div class="card">
      <div class="head purple">📊 CLASSEMENTS DES GROUPES <span style="float:right;font-size:16px;color:#39ff70">● DÉFILEMENT AUTO</span></div>
      <div class="standing">
        <div class="groupTitle" id="groupName">GROUPE A</div>
        <table>
          <thead><tr><th>#</th><th>Équipe</th><th>MJ</th><th>DIFF</th><th>PTS</th></tr></thead>
          <tbody id="table"></tbody>
        </table>
        <div class="tabs" id="tabs"></div>
      </div>
    </div>

    <div class="card bottom1"><div class="boxContent"><div class="big">🥇 MEILLEURS BUTEURS</div><div class="info">Mbappé 4 buts<br>Kane 3 buts<br>Martínez 3 buts</div></div></div>
    <div class="card bottom2"><div class="boxContent"><div class="big">PROCHAIN MATCH</div><div class="info">🇫🇷 FRANCE VS AUTRICHE 🇦🇹<br>22 JUIN - 21:00</div></div></div>
    <div class="card bottom3"><div class="boxContent"><div class="big">🏆 INFOS COUPE DU MONDE</div><div class="info">104 matchs • 48 équipes • 16 villes hôtes</div></div></div>
  </div>

  <div class="footer">🔄 ACTUALISATION AUTOMATIQUE — Toutes les 15 minutes</div>
</div>

<script>
function clock(){
 const n=new Date();
 time.textContent=n.toLocaleTimeString("fr-FR",{hour:"2-digit",minute:"2-digit"});
 date.textContent=n.toLocaleDateString("fr-FR",{weekday:"long",day:"numeric",month:"long",year:"numeric"}).toUpperCase();
}
setInterval(clock,1000);clock();

const groups=[
["GROUPE A",[["🇲🇽","MEXIQUE",1,"+2",3],["🇰🇷","CORÉE DU SUD",1,"+2",3],["🇿🇦","AFRIQUE DU SUD",1,"-1",0],["🇨🇿","TCHÉQUIE",1,"-3",0]]],
["GROUPE B",[["🇨🇦","CANADA",1,"0",1],["🇨🇭","SUISSE",1,"0",1],["🇧🇦","BOSNIE",1,"0",1],["🇶🇦","QATAR",1,"0",1]]],
["GROUPE C",[["🇧🇷","BRÉSIL",1,"0",1],["🇲🇦","MAROC",1,"0",1],["🏴","ÉCOSSE",1,"+1",3],["🇭🇹","HAÏTI",1,"-1",0]]],
["GROUPE D",[["🇺🇸","ÉTATS-UNIS",1,"+3",3],["🇦🇺","AUSTRALIE",1,"+2",3],["🇹🇷","TURQUIE",1,"-2",0],["🇵🇾","PARAGUAY",1,"-3",0]]]
];
let i=0;
function render(){
 const g=groups[i];
 groupName.textContent=g[0];
 table.innerHTML=g[1].map((t,n)=>`<tr><td>${n+1}</td><td class="team">${t[0]} ${t[1]}</td><td>${t[2]}</td><td>${t[3]}</td><td><span class="pts">${t[4]}</span></td></tr>`).join("");
 tabs.innerHTML=groups.map((x,n)=>`<span class="tab ${n==i?'active':''}">${x[0].replace('GROUPE ','')}</span>`).join("");
 i=(i+1)%groups.length;
}
render();setInterval(render,10000);
</script>
</body>
</html>
