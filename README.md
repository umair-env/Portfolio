<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Umair — Student &amp; Self-taught Developer</title>
  <meta name="description" content="Umair — Student, late-night coder, web developer & AI enthusiast" />
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#0f1724; --card:#0b1220; --muted:#94a3b8; --accent:#7c3aed; --glass: rgba(255,255,255,0.04);
      --max-w:1100px; --radius:14px;
      font-family: 'Inter', system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
    }
    *{box-sizing:border-box}
    html,body{height:100%;margin:0;background:linear-gradient(180deg,#071023 0%, #071428 50%, #02101a 100%);color:#e6eef8}
    .wrap{max-width:var(--max-w);margin:36px auto;padding:28px}

    .header{display:flex;gap:20px;align-items:center}
    .avatar{width:124px;height:124px;border-radius:18px;flex:0 0 124px;background:linear-gradient(135deg,var(--accent),#0ea5a7);display:grid;place-items:center;box-shadow:0 8px 30px rgba(2,6,23,0.7)}
    .avatar svg{width:92px;height:92px;filter:drop-shadow(0 6px 18px rgba(0,0,0,0.6))}

    .title h1{margin:0;font-size:28px;letter-spacing:-0.5px}
    .title p.lead{margin:6px 0 0;color:var(--muted)}

    .grid{display:grid;grid-template-columns:1fr 340px;gap:22px;margin-top:22px}

    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));padding:20px;border-radius:var(--radius);box-shadow:0 6px 24px rgba(2,6,23,0.6);border:1px solid rgba(255,255,255,0.03)}

    /* left column */
    .bio{display:flex;flex-direction:column;gap:12px}
    .badges{display:flex;gap:8px;flex-wrap:wrap}
    .badge{background:var(--glass);padding:8px 10px;border-radius:10px;color:var(--muted);font-weight:600;font-size:13px}

    .skills{display:flex;flex-wrap:wrap;gap:10px;margin-top:8px}
    .skill{background:rgba(255,255,255,0.03);padding:8px 10px;border-radius:10px;font-weight:600;color:#dbeafe}

    .section-title{color:var(--muted);font-size:13px;margin-bottom:8px}

    /* right column */
    .contact-list{display:flex;flex-direction:column;gap:8px}
    .contact-item{display:flex;align-items:center;gap:10px}
    .btn{display:inline-block;padding:10px 14px;border-radius:12px;background:linear-gradient(90deg,var(--accent),#06b6d4);color:white;font-weight:700;text-decoration:none}

    /* projects */
    .projects{display:grid;grid-template-columns:repeat(auto-fill,minmax(220px,1fr));gap:12px;margin-top:12px}
    .proj{padding:12px;border-radius:12px;background:linear-gradient(180deg, rgba(255,255,255,0.018), rgba(255,255,255,0.01));border:1px solid rgba(255,255,255,0.02)}
    .proj h4{margin:0 0 6px;font-size:15px}
    .proj p{margin:0;color:var(--muted);font-size:13px}

    footer{margin-top:18px;text-align:center;color:var(--muted);font-size:13px}

    /* responsive */
    @media (max-width:880px){
      .grid{grid-template-columns:1fr}
      .avatar{width:96px;height:96px}
    }
  </style>
</head>
<body>
  <div class="wrap">
    <div class="header">
      <div class="avatar card" aria-hidden="true">
        <!-- simple SVG avatar placeholder -->
        <svg viewBox="0 0 120 120" xmlns="http://www.w3.org/2000/svg" fill="none">
          <rect width="120" height="120" rx="18" fill="white" opacity="0.06"/>
          <circle cx="60" cy="40" r="20" fill="white" opacity="0.15"/>
          <rect x="24" y="70" width="72" height="18" rx="6" fill="white" opacity="0.08"/>
        </svg>
      </div>

      <div class="title">
        <h1>Hi, I'm <strong>Umair</strong> <span style="opacity:.9">👋</span></h1>
        <p class="lead">✨ Student | Self-taught Developer — <span style="color:var(--accent);font-weight:700">late night coder</span></p>
        <div style="margin-top:10px" class="badges">
          <div class="badge">Web Developer</div>
          <div class="badge">AI Enthusiast</div>
          <div class="badge">Hackathon Ready</div>
        </div>
      </div>
    </div>

    <div class="grid">
      <!-- LEFT: main content -->
      <div>
        <div class="card bio">
          <div>
            <div class="section-title">About</div>
            <p style="margin:0;line-height:1.6;color:#dbeafe">I'm a student and self-taught developer who codes late at night. I focus on building websites and learning AI tools and prompting. I enjoy participating in hackathons and bringing ideas to life.</p>
          </div>

          <div>
            <div class="section-title">Skills</div>
            <div class="skills">
              <div class="skill">HTML</div>
              <div class="skill">CSS</div>
              <div class="skill">JavaScript</div>
              <div class="skill">Node.js</div>
              <div class="skill">Python</div>
              <div class="skill">AI Prompting</div>
              <div class="skill">LLM (learning)</div>
              <div class="skill">RIG (learning)</div>
            </div>
          </div>

          <div>
            <div class="section-title">Projects &amp; Notes</div>
            <div class="projects">
              <div class="proj">
                <h4>OpenBook (idea)</h4>
                <p>Education platform concept: textbooks, AI tutor (VEDA), and student dashboard.</p>
              </div>
              <div class="proj">
                <h4>Portfolio</h4>
                <p>Personal website hosted on GitHub to show projects and README.</p>
              </div>
              <div class="proj">
                <h4>AI Tutor MVP</h4>
                <p>Chatbot MVP built with Gemini model; next: NOVA backend.</p>
              </div>
            </div>
          </div>

          <div style="margin-top:12px;display:flex;gap:10px;flex-wrap:wrap;align-items:center">
            <a class="btn" href="#download-readme" onclick="downloadREADME()">Download README.md</a>
            <a class="btn" href="#" style="background:transparent;border:1px solid rgba(255,255,255,0.06);font-weight:700;text-decoration:none;color:var(--muted)">View on GitHub</a>
          </div>
        </div>

        <div style="margin-top:14px" class="card">
          <div class="section-title">Contact</div>
          <p style="margin:0;color:var(--muted)">You can add links to your GitHub, LinkedIn, or email here so recruiters and collaborators can reach you.</p>

          <div style="margin-top:10px;display:flex;gap:8px;flex-wrap:wrap">
            <input id="copyEmail" value="your_email@example.com" style="background:transparent;border:1px solid rgba(255,255,255,0.04);padding:10px;border-radius:10px;color:#e6eef8;width:300px" />
            <button class="btn" onclick="copyEmail()">Copy Email</button>
          </div>
        </div>

      </div>

      <!-- RIGHT: side column -->
      <aside>
        <div class="card">
          <div class="section-title">Quick Info</div>
          <div style="display:flex;flex-direction:column;gap:8px;margin-top:8px" class="contact-list">
            <div class="contact-item"><strong>Location:</strong><span style="margin-left:auto;color:var(--muted)">India</span></div>
            <div class="contact-item"><strong>Availability:</strong><span style="margin-left:auto;color:var(--muted)">Part-time</span></div>
            <div class="contact-item"><strong>Languages:</strong><span style="margin-left:auto;color:var(--muted)">English, Urdu</span></div>
          </div>
        </div>

        <div style="margin-top:12px" class="card">
          <div class="section-title">Education</div>
          <p style="margin:0;color:var(--muted)">8th class — student. Learning web dev & AI on the side.</p>
        </div>

        <div style="margin-top:12px" class="card">
          <div class="section-title">Social</div>
          <div style="display:flex;flex-direction:column;gap:8px;margin-top:8px">
            <a href="#" style="text-decoration:none;color:#e6eef8">GitHub: @umair-env</a>
            <a href="#" style="text-decoration:none;color:#e6eef8">LinkedIn</a>
            <a href="#" style="text-decoration:none;color:#e6eef8">Twitter / X</a>
          </div>
        </div>
      </aside>
    </div>

    <footer>
      Made with ❤️ by Umair — change this page freely. Save it as <code>index.html</code> and open locally to preview.
    </footer>
  </div>

  <script>
    function copyEmail(){
      const el = document.getElementById('copyEmail');
      el.select();
      el.setSelectionRange(0,99999);
      navigator.clipboard.writeText(el.value).then(()=>{
        alert('Email copied to clipboard')
      })
    }

    function downloadREADME(){
      const content = `# Hi, I'm Umair 👋\n\n✨ Student | Self-taught Developer \n\n💡 late night coder\n\n# skills\nwebdeveloper:HTML,CSS,JAVASCRIPT,NODE.js\n\nAi: python, Ai prompting,Ai tools,(learning LLM,RIG)`;
      const blob = new Blob([content], {type:'text/plain'});
      const url = URL.createObjectURL(blob);
      const a = document.createElement('a');
      a.href = url; a.download = 'README.md'; document.body.appendChild(a); a.click(); a.remove(); URL.revokeObjectURL(url);
    }
  </script>
</body>
</html>

