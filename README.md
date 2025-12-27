# LINK-HUB-oS
Link hub os system 
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Link Hub | Business Operating System</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<!-- Fonts -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">

<!-- Chart.js -->
<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>

<style>
:root{
  --primary:#1E88E5;
  --bg:#F2F7FB;
  --card:#FFFFFF;
  --text:#0F172A;
  --muted:#64748B;
  --border:#DDE6F0;
}

*{box-sizing:border-box;margin:0;padding:0;font-family:'Inter',sans-serif;}
body{background:var(--bg);color:var(--text);}

.layout{display:flex}

/* SIDEBAR */
nav{
  width:300px;
  height:100vh;
  position:fixed;
  background:var(--card);
  padding:30px 20px;
  box-shadow:0 20px 50px rgba(0,0,0,.08);
  overflow-y:auto;
}

nav h2{color:var(--primary);margin-bottom:20px}

nav select{
  width:100%;
  padding:10px;
  border-radius:12px;
  border:1px solid var(--border);
  margin-bottom:20px;
}

nav a{
  display:block;
  text-decoration:none;
  color:var(--text);
  padding:12px 16px;
  border-radius:18px;
  font-size:14px;
  margin-bottom:8px;
}
nav a:hover{background:var(--bg)}

/* MAIN */
main{
  margin-left:320px;
  padding:50px;
  width:calc(100% - 320px);
}

section{margin-bottom:100px}

.card{
  background:var(--card);
  padding:36px;
  border-radius:28px;
  box-shadow:0 16px 44px rgba(0,0,0,.08);
  margin-bottom:30px;
}

h1{font-size:32px;margin-bottom:12px}
h2{font-size:22px;margin-bottom:10px}
p{font-size:14px;color:var(--muted);line-height:1.8}

/* KPI */
.kpi-grid{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
  gap:20px;
}
.kpi{
  background:var(--bg);
  padding:24px;
  border-radius:22px;
}
.kpi strong{font-size:22px;color:var(--primary)}
.kpi span{font-size:13px;color:var(--muted)}

/* TABLE */
table{width:100%;border-collapse:collapse}
th,td{padding:14px;border-bottom:1px solid var(--border);text-align:left}
th{font-size:13px;color:var(--muted)}
</style>
</head>

<body>
<div class="layout">

<!-- ================= SIDEBAR ================= -->
<nav>
  <h2>LINK HUB OS</h2>

  <select id="roleSelect">
    <option value="founder">Founder</option>
    <option value="program">Program Director</option>
    <option value="education">Education Lead</option>
    <option value="operations">Operations Lead</option>
    <option value="team">Team Member</option>
    <option value="learner">Learner</option>
  </select>

  <a href="#dashboard">Dashboard</a>
  <a href="#strategy">Strategy</a>
  <a href="#departments">Departments</a>
  <a href="#operations">Operations</a>
  <a href="#learning">Learning System</a>
  <a href="#roles">Roles & Team</a>
</nav>

<!-- ================= MAIN ================= -->
<main>

<!-- DASHBOARD -->
<section id="dashboard" data-role="founder program">
<h1>Executive Dashboard</h1>

<div class="card">
  <div class="kpi-grid">
    <div class="kpi"><strong>1,240</strong><br><span>Active Learners</span></div>
    <div class="kpi"><strong>312</strong><br><span>Businesses Supported</span></div>
    <div class="kpi"><strong>94%</strong><br><span>Completion Rate</span></div>
    <div class="kpi"><strong>R186k</strong><br><span>Monthly Revenue</span></div>
  </div>
</div>

<div class="card">
  <h2>Market Growth Projection</h2>
  <canvas id="marketChart"></canvas>
</div>
</section>

<!-- STRATEGY -->
<section id="strategy" data-role="founder program">
<h1>Vision & Strategy</h1>
<div class="card">
<p>
Link Hub operates as an AI-enabled education and business empowerment system.
Knowledge is standardized, culturally grounded, quality-controlled, and distributed at scale.
</p>
</div>
</section>

<!-- DEPARTMENTS -->
<section id="departments" data-role="founder program operations education">
<h1>Departments</h1>

<div class="card">
<table>
<tr><th>Department</th><th>Core Purpose</th></tr>
<tr><td>Education & Curriculum</td><td>CAPS delivery, assessments, learner outcomes</td></tr>
<tr><td>AI & Systems</td><td>Automation, platform intelligence, scalability</td></tr>
<tr><td>Operations</td><td>Execution flow, quality control, efficiency</td></tr>
<tr><td>Marketing & Growth</td><td>Brand, demand, audience growth</td></tr>
<tr><td>Community & Partnerships</td><td>Schools, NGOs, outreach, trust</td></tr>
<tr><td>Finance & Compliance</td><td>Cash flow, reporting, sustainability</td></tr>
</table>
</div>
</section>

<!-- OPERATIONS -->
<section id="operations" data-role="founder program operations">
<h1>Operational Workflow</h1>
<div class="card">
<ol style="line-height:2;color:var(--muted)">
  <li>Request Intake</li>
  <li>AI Draft Processing</li>
  <li>Human Review & Quality Control</li>
  <li>Final Delivery</li>
  <li>Feedback & Optimization</li>
</ol>
</div>
</section>

<!-- LEARNING -->
<section id="learning" data-role="founder program education team learner">
<h1>Internal & External Learning System</h1>

<div class="card">
<h2>Learning Tracks</h2>
<ul style="line-height:2;color:var(--muted)">
  <li>Onboarding (Culture, Tools, Discipline)</li>
  <li>Role-Specific Skill Development</li>
  <li>Performance-Based Advancement</li>
  <li>Certification & Career Transition</li>
</ul>
</div>
</section>

<!-- ROLES -->
<section id="roles" data-role="founder program">
<h1>Roles & Team Structure</h1>

<div class="card">
<table>
<tr><th>Role</th><th>Accountability</th></tr>
<tr><td>Founder / Managing Director</td><td>Vision, capital, partnerships</td></tr>
<tr><td>Program Director</td><td>KPIs, delivery, execution</td></tr>
<tr><td>Education Lead</td><td>Curriculum, learner outcomes</td></tr>
<tr><td>Operations Lead</td><td>Processes, efficiency</td></tr>
<tr><td>AI & Systems Lead</td><td>Automation, platform logic</td></tr>
<tr><td>Team Members</td><td>Execution & delivery</td></tr>
</table>
</div>
</section>

</main>
</div>

<!-- ================= SCRIPTS ================= -->
<script>
// ROLE BASED VIEW
const roleSelect = document.getElementById('roleSelect');
const sections = document.querySelectorAll('section');

function updateView(){
  const role = roleSelect.value;
  sections.forEach(sec=>{
    const allowed = sec.dataset.role;
    if(!allowed || allowed.includes(role)){
      sec.style.display = 'block';
    } else {
      sec.style.display = 'none';
    }
  });
}
roleSelect.addEventListener('change', updateView);
updateView();

// CHART
const ctx = document.getElementById('marketChart');
new Chart(ctx,{
  type:'line',
  data:{
    labels:['2024','2025','2026','2027','2028','2029','2030'],
    datasets:[{
      data:[22,26,30,35,40,45,48],
      borderWidth:3,
      tension:.4
    }]
  },
  options:{plugins:{legend:{display:false}}}
});
</script>

</body>
</html>
