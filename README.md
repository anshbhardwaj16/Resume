<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Ansh Bhardwaj — Platform &amp; Data Engineer</title>
<meta name="description" content="Ansh Bhardwaj — Platform, Data &amp; GenAI Automation Engineer. 2.5+ years building large-scale Airflow orchestration, CI/CD, and Agentic AI systems." />
<link rel="preconnect" href="https://fonts.googleapis.com" />
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;600;700&family=IBM+Plex+Sans:wght@400;500;600&family=IBM+Plex+Mono:wght@400;500&display=swap" rel="stylesheet" />
<style>
  :root{
    --ink:#16233A;
    --navy:#1F3A5F;
    --navy-600:#2C4E77;
    --paper:#F4F7FA;
    --card:#FFFFFF;
    --line:#E3E9F0;
    --muted:#5C6B80;
    --body:#2A3648;
    --accent:#0E7C86;
    --tag-bg:#EEF3F8;
    --tag-text:#334965;
    --sans:"IBM Plex Sans",-apple-system,BlinkMacSystemFont,"Segoe UI",sans-serif;
    --disp:"Space Grotesk",var(--sans);
    --mono:"IBM Plex Mono",ui-monospace,"SFMono-Regular",Menlo,monospace;
  }

  *{box-sizing:border-box;}
  html{-webkit-text-size-adjust:100%;}
  body{
    margin:0;
    background:
      radial-gradient(1200px 400px at 85% -120px, #EAF1F7 0%, rgba(234,241,247,0) 70%),
      var(--paper);
    color:var(--body);
    font-family:var(--sans);
    font-size:15px;
    line-height:1.6;
    -webkit-font-smoothing:antialiased;
    text-rendering:optimizeLegibility;
  }

  .sheet{
    max-width:1040px;
    margin:40px auto;
    background:var(--card);
    border:1px solid var(--line);
    border-radius:14px;
    box-shadow:0 1px 2px rgba(22,35,58,.04), 0 18px 50px -30px rgba(22,35,58,.35);
    overflow:hidden;
  }

  /* ---------- header ---------- */
  .head{
    position:relative;
    padding:44px 48px 30px;
    border-bottom:1px solid var(--line);
    overflow:hidden;
  }
  .dag{
    position:absolute;
    top:0; right:0; height:100%; width:46%;
    color:var(--navy);
    opacity:.11;
    pointer-events:none;
  }
  .name{
    font-family:var(--disp);
    font-weight:700;
    font-size:clamp(30px,5.2vw,46px);
    letter-spacing:.01em;
    line-height:1.02;
    color:var(--navy);
    margin:0;
    position:relative;
  }
  .role{
    font-family:var(--mono);
    font-size:13px;
    letter-spacing:.06em;
    color:var(--muted);
    margin:12px 0 0;
    position:relative;
  }
  .role b{color:var(--accent);font-weight:500;}
  .contact{
    position:relative;
    margin-top:22px;
    display:flex;
    flex-wrap:wrap;
    gap:9px 20px;
    font-family:var(--mono);
    font-size:12.5px;
  }
  .contact a, .contact span{
    display:inline-flex;
    align-items:center;
    gap:7px;
    color:var(--ink);
    text-decoration:none;
    border-bottom:1px solid transparent;
    transition:color .15s ease, border-color .15s ease;
  }
  .contact a:hover{color:var(--accent);border-bottom-color:var(--accent);}
  .contact svg{width:14px;height:14px;flex:0 0 auto;color:var(--navy-600);}
  .contact a:hover svg{color:var(--accent);}

  /* ---------- body grid ---------- */
  .grid{
    display:grid;
    grid-template-columns:1.85fr .95fr;
    gap:0;
  }
  .main{padding:30px 40px 42px 48px;}
  .rail{
    padding:30px 44px 42px 34px;
    background:linear-gradient(180deg,#FBFCFE 0%,#F7FAFD 100%);
    border-left:1px solid var(--line);
  }

  /* ---------- section titles ---------- */
  .sec{margin:0 0 22px;}
  .sec:last-child{margin-bottom:0;}
  .sec-title{
    display:flex;
    align-items:center;
    gap:11px;
    margin:0 0 14px;
    font-family:var(--disp);
    font-weight:600;
    font-size:12.5px;
    letter-spacing:.16em;
    text-transform:uppercase;
    color:var(--navy);
    white-space:nowrap;
  }
  .node{
    width:9px;height:9px;flex:0 0 auto;border-radius:50%;
    background:var(--navy);
    box-shadow:0 0 0 3px rgba(31,58,95,.14);
  }
  .edge{height:1px;flex:1 1 auto;background:var(--line);}

  /* ---------- summary ---------- */
  .summary{margin:0;color:var(--body);}

  /* ---------- experience / projects ---------- */
  .item{margin:0 0 20px;}
  .item:last-child{margin-bottom:0;}
  .item-head{display:flex;flex-wrap:wrap;align-items:baseline;justify-content:space-between;gap:4px 16px;}
  .org{font-family:var(--disp);font-weight:600;font-size:16px;color:var(--ink);margin:0;letter-spacing:.005em;}
  .org .at{color:var(--navy-600);font-weight:500;}
  .when{font-family:var(--mono);font-size:11.5px;color:var(--muted);white-space:nowrap;}
  .sub{font-size:13px;color:var(--muted);margin:1px 0 10px;}
  .proj-name{font-family:var(--disp);font-weight:600;font-size:15.5px;color:var(--navy);margin:0 0 8px;}

  .stack{display:flex;flex-wrap:wrap;gap:6px;margin:0 0 11px;}
  .tag{
    font-family:var(--mono);
    font-size:11px;
    line-height:1;
    padding:5px 8px;
    color:var(--tag-text);
    background:var(--tag-bg);
    border:1px solid #E0E8F1;
    border-radius:6px;
    white-space:nowrap;
  }

  ul.pts{list-style:none;margin:0;padding:0;}
  ul.pts li{position:relative;padding:0 0 7px 20px;color:var(--body);}
  ul.pts li:last-child{padding-bottom:0;}
  ul.pts li::before{
    content:"";
    position:absolute;left:2px;top:.62em;
    width:6px;height:6px;border-radius:50%;
    background:var(--accent);
    opacity:.85;
  }
  b.mark{color:var(--ink);font-weight:600;}

  .proj + .proj{margin-top:20px;padding-top:20px;border-top:1px dashed var(--line);}

  /* ---------- rail blocks ---------- */
  .skill{margin:0 0 14px;}
  .skill:last-child{margin-bottom:0;}
  .skill-k{
    font-family:var(--mono);
    font-size:10.5px;
    letter-spacing:.1em;
    text-transform:uppercase;
    color:var(--navy-600);
    margin:0 0 3px;
  }
  .skill-v{font-size:13.5px;color:var(--body);line-height:1.5;}

  ul.stack-list{list-style:none;margin:0;padding:0;}
  ul.stack-list li{position:relative;padding:0 0 8px 18px;font-size:13.5px;line-height:1.45;color:var(--body);}
  ul.stack-list li:last-child{padding-bottom:0;}
  ul.stack-list li::before{
    content:"";position:absolute;left:0;top:.5em;
    width:7px;height:7px;border-radius:2px;
    border:1.5px solid var(--navy);
  }
  .cert-i{color:var(--muted);font-family:var(--mono);font-size:11px;display:block;}

  .edu{margin:0 0 12px;}
  .edu:last-child{margin-bottom:0;}
  .edu-d{font-family:var(--disp);font-weight:600;font-size:13.5px;color:var(--ink);}
  .edu-s{font-size:12.5px;color:var(--muted);}
  .edu-y{font-family:var(--mono);font-size:11px;color:var(--accent);}

  .langs{font-size:13.5px;color:var(--body);}
  .langs b{color:var(--ink);font-weight:600;}

  .foot{
    padding:16px 48px;
    border-top:1px solid var(--line);
    font-family:var(--mono);
    font-size:11px;
    color:var(--muted);
    display:flex;justify-content:space-between;flex-wrap:wrap;gap:8px;
  }
  .foot a{color:var(--navy-600);text-decoration:none;}
  .foot a:hover{color:var(--accent);}

  /* ---------- entrance motion ---------- */
  @keyframes fadeUp{from{opacity:0;transform:translateY(10px);}to{opacity:1;transform:none;}}
  .anim{opacity:0;animation:fadeUp .55s cubic-bezier(.22,.61,.36,1) forwards;}
  .head{animation:fadeUp .5s ease forwards;}
  .d1{animation-delay:.05s}.d2{animation-delay:.12s}.d3{animation-delay:.19s}
  .d4{animation-delay:.26s}.d5{animation-delay:.33s}.d6{animation-delay:.4s}
  .d7{animation-delay:.47s}.d8{animation-delay:.54s}

  a:focus-visible, .contact a:focus-visible{outline:2px solid var(--accent);outline-offset:3px;border-radius:3px;}

  @media (max-width:760px){
    .sheet{margin:0;border-radius:0;border-left:0;border-right:0;}
    .head{padding:34px 22px 24px;}
    .dag{display:none;}
    .grid{grid-template-columns:1fr;}
    .main{padding:26px 22px 8px;}
    .rail{border-left:0;border-top:1px solid var(--line);padding:26px 22px 34px;}
    .foot{padding:16px 22px;}
    .item-head{gap:2px;}
  }

  @media (prefers-reduced-motion:reduce){
    .anim,.head{animation:none;opacity:1;transform:none;}
  }

  /* ---------- print ---------- */
  @media print{
    @page{margin:14mm;}
    body{background:#fff;font-size:10.5pt;}
    .sheet{max-width:none;margin:0;border:0;border-radius:0;box-shadow:none;}
    .head{padding:0 0 12px;border-bottom:1px solid #ccc;}
    .dag{display:none;}
    .grid{grid-template-columns:1.9fr 1fr;}
    .main{padding:16px 20px 0 0;}
    .rail{background:none;border-left:1px solid #ddd;padding:16px 0 0 20px;}
    .anim,.head{animation:none;opacity:1;}
    .tag{background:#fff;}
    a{color:var(--ink);text-decoration:none;}
    .item,.proj,.sec,.edu,.skill{break-inside:avoid;}
    .foot{border-top:1px solid #ddd;}
  }
</style>
</head>
<body>
  <main class="sheet">

    <header class="head">
      <svg class="dag" viewBox="0 0 420 300" fill="none" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
        <g stroke="currentColor" stroke-width="1.5" opacity="0.9">
          <path d="M40 60 C110 60 120 40 190 40" />
          <path d="M40 60 C110 60 120 150 190 150" />
          <path d="M40 210 C110 210 120 150 190 150" />
          <path d="M40 210 C110 210 120 250 190 250" />
          <path d="M190 40 C260 40 270 95 340 95" />
          <path d="M190 150 C260 150 270 95 340 95" />
          <path d="M190 150 C260 150 270 205 340 205" />
          <path d="M190 250 C260 250 270 205 340 205" />
          <path d="M340 95 C380 95 388 150 405 150" />
          <path d="M340 205 C380 205 388 150 405 150" />
        </g>
        <g fill="currentColor">
          <circle cx="40" cy="60" r="7"/><circle cx="40" cy="210" r="7"/>
          <circle cx="190" cy="40" r="7"/><circle cx="190" cy="150" r="8"/><circle cx="190" cy="250" r="7"/>
          <circle cx="340" cy="95" r="7"/><circle cx="340" cy="205" r="7"/>
          <circle cx="405" cy="150" r="7"/>
        </g>
      </svg>

      <h1 class="name">Ansh Bhardwaj</h1>
      <p class="role">Platform Engineer <b>·</b> Data Engineer <b>·</b> GenAI Automation Engineer</p>

      <nav class="contact" aria-label="Contact">
        <span>
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M20 10c0 6-8 12-8 12s-8-6-8-12a8 8 0 0116 0z"/><circle cx="12" cy="10" r="3"/></svg>
          Meerut, India
        </span>
        <a href="mailto:anshbhardwaj16@gmail.com">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="3" y="5" width="18" height="14" rx="2"/><path d="m3 7 9 6 9-6"/></svg>
          anshbhardwaj16@gmail.com
        </a>
        <a href="tel:+918445256683">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M22 16.9v3a2 2 0 0 1-2.2 2 19.8 19.8 0 0 1-8.6-3.1 19.5 19.5 0 0 1-6-6 19.8 19.8 0 0 1-3.1-8.7A2 2 0 0 1 4.1 2h3a2 2 0 0 1 2 1.7c.1.9.3 1.8.6 2.6a2 2 0 0 1-.5 2.1L8 9.6a16 16 0 0 0 6 6l1.2-1.2a2 2 0 0 1 2.1-.5c.8.3 1.7.5 2.6.6a2 2 0 0 1 1.7 2z"/></svg>
          +91 84452 56683
        </a>
        <a href="https://www.linkedin.com/in/anshbhardwaj16" target="_blank" rel="noopener">
          <svg viewBox="0 0 24 24" fill="currentColor"><path d="M4.98 3.5A2.5 2.5 0 1 1 0 3.5a2.5 2.5 0 0 1 4.98 0zM.5 8h4v13h-4V8zM8 8h3.8v1.8h.05c.53-1 1.83-2.05 3.76-2.05C19.6 7.75 21 10 21 13.3V21h-4v-6.9c0-1.64-.03-3.75-2.28-3.75-2.29 0-2.64 1.79-2.64 3.63V21H8V8z"/></svg>
          linkedin.com/in/anshbhardwaj16
        </a>
        <a href="https://github.com/anshbhardwaj16" target="_blank" rel="noopener">
          <svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 .5A11.5 11.5 0 0 0 .5 12a11.5 11.5 0 0 0 7.86 10.92c.57.1.78-.25.78-.55v-2c-3.2.7-3.88-1.37-3.88-1.37-.53-1.34-1.28-1.7-1.28-1.7-1.05-.72.08-.7.08-.7 1.16.08 1.77 1.2 1.77 1.2 1.03 1.76 2.7 1.25 3.36.96.1-.75.4-1.26.73-1.55-2.56-.29-5.26-1.28-5.26-5.7 0-1.26.45-2.29 1.2-3.1-.12-.29-.52-1.46.11-3.05 0 0 .97-.31 3.18 1.18a11 11 0 0 1 5.8 0c2.2-1.5 3.17-1.18 3.17-1.18.63 1.59.23 2.76.12 3.05.74.81 1.19 1.84 1.19 3.1 0 4.43-2.7 5.4-5.28 5.69.42.36.79 1.08.79 2.18v3.23c0 .31.2.66.79.55A11.5 11.5 0 0 0 23.5 12 11.5 11.5 0 0 0 12 .5z"/></svg>
          github.com/anshbhardwaj16
        </a>
      </nav>
    </header>

    <div class="grid">
      <!-- MAIN COLUMN -->
      <section class="main">
        <section class="sec anim d1">
          <h2 class="sec-title"><span class="node"></span>Summary<span class="edge"></span></h2>
          <p class="summary">Platform &amp; Data Engineer with <b class="mark">2.5+ years</b> of experience designing and operating large-scale data platforms, workflow orchestration systems, and enterprise automation solutions. Experienced in managing <b class="mark">800+ production Apache Airflow DAGs</b>, developing SQL-driven workflows and CI/CD automation frameworks, and building GenAI-powered operational intelligence and Agentic AI solutions using LLMs, Copilot Studio, and Power Automate.</p>
        </section>

        <section class="sec anim d2">
          <h2 class="sec-title"><span class="node"></span>Experience<span class="edge"></span></h2>
          <div class="item">
            <div class="item-head">
              <p class="org">Accenture Solutions Pvt. Ltd. <span class="at">— Data Engineer (Management &amp; Governance Analyst)</span></p>
              <span class="when">Sep 2023 — Present</span>
            </div>
            <p class="sub">Noida, India</p>
            <ul class="pts">
              <li>Orchestrated and governed approximately <b class="mark">800 production Apache Airflow DAGs</b>, ensuring reliable execution of large-scale enterprise data workflows.</li>
              <li>Developed reusable <b class="mark">AutoDAG</b> templates to standardize pipeline creation and accelerate onboarding of new workflows.</li>
              <li>Automated Selenium-based test execution using Docker and GitHub Actions, streamlining CI/CD validation.</li>
              <li>Built a GenAI-powered Airflow <b class="mark">Auto-Healing Framework</b> using Copilot Studio and Power Automate to automate failure detection and remediation.</li>
              <li>Reduced manual operational effort by <b class="mark">20%</b>, saving <b class="mark">50+ engineering hours/month</b>.</li>
            </ul>
          </div>
        </section>

        <section class="sec anim d3">
          <h2 class="sec-title"><span class="node"></span>Projects<span class="edge"></span></h2>

          <div class="item proj">
            <p class="proj-name">GenAI-Powered Airflow Auto-Healing Framework</p>
            <div class="stack">
              <span class="tag">Apache Airflow</span><span class="tag">Python</span><span class="tag">Copilot Studio</span><span class="tag">Power Automate</span><span class="tag">REST APIs</span><span class="tag">ServiceNow</span><span class="tag">LLMs</span>
            </div>
            <ul class="pts">
              <li>Designed an enterprise-grade GenAI auto-healing solution for Apache Airflow.</li>
              <li>Automated failure analysis and remediation using LLMs.</li>
              <li>Integrated intelligent recovery workflows and automated DAG retriggering.</li>
              <li>Reduced <b class="mark">MTTR by 20%</b> and saved <b class="mark">50+ engineering hours/month</b>.</li>
            </ul>
          </div>

          <div class="item proj">
            <p class="proj-name">OmniSpark — Enterprise Agentic AI Software Engineering Platform</p>
            <div class="stack">
              <span class="tag">Python</span><span class="tag">Multi-LLM</span><span class="tag">Jira REST APIs</span><span class="tag">Git</span><span class="tag">GitHub</span><span class="tag">VS Code Extension</span><span class="tag">Power Automate</span>
            </div>
            <ul class="pts">
              <li>Co-created <b class="mark">OmniSpark</b>, an enterprise Agentic AI platform supporting multiple LLM providers that automates the complete software development lifecycle (SDLC).</li>
              <li>Enabled AI agents to author detailed Jira stories (or select backlog items) and autonomously handle feature branches, production-ready code generation, testing, code reviews, PR creation, continuous Jira updates, and LLM policy-gate validation through delivery.</li>
              <li>Built reusable AI engineering workflows to standardize software delivery and reduce manual engineering effort.</li>
              <li>Co-developed <b class="mark">RAGENTS</b>, an enterprise-grade VS Code extension providing a centralized marketplace of reusable AI agents, engineering skills, prompts, and workflows.</li>
            </ul>
          </div>
        </section>
      </section>

      <!-- RAIL COLUMN -->
      <aside class="rail">
        <section class="sec anim d3">
          <h2 class="sec-title"><span class="node"></span>Skills<span class="edge"></span></h2>
          <div class="skill"><p class="skill-k">Programming</p><div class="skill-v">Python, SQL</div></div>
          <div class="skill"><p class="skill-k">Data Engineering</p><div class="skill-v">Apache Airflow, Workflow Orchestration, Data Pipeline Management, DAG Monitoring &amp; Governance, Databricks</div></div>
          <div class="skill"><p class="skill-k">DevOps</p><div class="skill-v">Docker, Git, GitHub Actions, CI/CD Pipelines, REST APIs, Power Automate</div></div>
          <div class="skill"><p class="skill-k">GenAI</p><div class="skill-v">Agentic AI, Multi-LLM, Copilot Studio, Prompt Engineering, Semantic Search, Vector Embeddings, RAG, LLM-Powered Workflows</div></div>
          <div class="skill"><p class="skill-k">Tools</p><div class="skill-v">Jira &amp; Confluence, GitHub, ServiceNow</div></div>
        </section>

        <section class="sec anim d4">
          <h2 class="sec-title"><span class="node"></span>Certifications<span class="edge"></span></h2>
          <ul class="stack-list">
            <li>Microsoft Certified: DP-203<span class="cert-i">Data Engineering on Azure</span></li>
            <li>Astronomer: Airflow Fundamentals</li>
            <li>Astronomer: DAG Monitoring &amp; Auditing</li>
            <li>Databricks: Generative AI Engineer Associate</li>
            <li>Microsoft: GitHub GHE-300</li>
            <li>Anthropic CCA-F</li>
          </ul>
        </section>

        <section class="sec anim d5">
          <h2 class="sec-title"><span class="node"></span>Awards<span class="edge"></span></h2>
          <ul class="stack-list">
            <li>ACE Award, Accenture<span class="cert-i">May 2026</span></li>
            <li>MC Star Award<span class="cert-i">Client Recognition</span></li>
            <li>SOS Award<span class="cert-i">Client Recognition</span></li>
          </ul>
        </section>

        <section class="sec anim d6">
          <h2 class="sec-title"><span class="node"></span>Education<span class="edge"></span></h2>
          <div class="edu">
            <div class="edu-d">B.Tech</div>
            <div class="edu-s">ABES Engineering College</div>
            <div class="edu-y">2023</div>
          </div>
          <div class="edu">
            <div class="edu-d">Class XII &amp; Class X</div>
            <div class="edu-s">Dewan Public School International</div>
            <div class="edu-y">2019 · 2017</div>
          </div>
        </section>

        <section class="sec anim d7">
          <h2 class="sec-title"><span class="node"></span>Languages<span class="edge"></span></h2>
          <p class="langs"><b>English</b> · <b>Hindi</b></p>
        </section>
      </aside>
    </div>

    <footer class="foot">
      <span>Ansh Bhardwaj · Platform &amp; Data Engineer</span>
      <a href="mailto:anshbhardwaj16@gmail.com">anshbhardwaj16@gmail.com</a>
    </footer>

  </main>
</body>
</html>
