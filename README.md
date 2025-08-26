<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Shantanu Pundir — Android Developer</title>
  <meta name="description" content="Shantanu Pundir — Android Developer. Java • Kotlin • Python • JavaScript. MVVM, Room, Jetpack components." />
  <style>
    :root{
      --bg:#0f1724; --card:#0b1220; --muted:#9aa5b1; --accent:#7c3aed; --glass:rgba(255,255,255,0.04);
      --radius:14px; --fg:#e6eef6;
      font-family: Inter, ui-sans-serif, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0; background:linear-gradient(180deg,#071027 0%, #071226 100%); color:var(--fg); -webkit-font-smoothing:antialiased;
      display:flex; align-items:center; justify-content:center; padding:40px;
    }
    .wrap{max-width:900px; width:100%;}

    .card{
      background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
      border-radius:var(--radius); padding:28px; box-shadow: 0 8px 30px rgba(2,6,23,0.7); backdrop-filter: blur(6px);
      border:1px solid rgba(255,255,255,0.03);
    }

    header{display:flex; gap:20px; align-items:center}
    .avatar{
      width:96px; height:96px; border-radius:12px; background:linear-gradient(135deg,var(--accent),#0ea5e9); display:flex; align-items:center; justify-content:center; font-weight:700; font-size:28px; color:white; flex-shrink:0;
    }
    h1{margin:0; font-size:22px}
    p.lead{margin:6px 0 0; color:var(--muted)}

    .grid{display:grid; grid-template-columns:1fr 300px; gap:20px; margin-top:22px}

    .section{background:var(--card); padding:18px; border-radius:12px; border:1px solid rgba(255,255,255,0.02)}
    .tech-badges{display:flex; flex-wrap:wrap; gap:8px}
    .badge{padding:6px 10px; border-radius:999px; font-size:13px; background:var(--glass); color:var(--fg); border:1px solid rgba(255,255,255,0.03)}

    .skills{display:flex; flex-wrap:wrap; gap:8px; margin-top:10px}
    ul{margin:8px 0 0 18px}

    .right .contact{display:flex; flex-direction:column; gap:10px}
    .contact a.btn{display:inline-block; text-decoration:none; padding:10px 12px; border-radius:10px; text-align:center; background:linear-gradient(90deg,var(--accent),#06b6d4); color:#fff; font-weight:600}

    .stats{display:flex; gap:8px; margin-top:8px; flex-wrap:wrap}
    .stat-card{flex:1; min-width:120px; padding:10px; border-radius:10px; background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01)); border:1px solid rgba(255,255,255,0.02)}

    footer{margin-top:18px; display:flex; justify-content:space-between; align-items:center; color:var(--muted); font-size:13px}

    /* responsive */
    @media (max-width:880px){
      .grid{grid-template-columns:1fr;}
      .right{order:2}
    }

    /* small utility */
    .muted{color:var(--muted)}
    .mono{font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, 'Roboto Mono', monospace}
    .copy{cursor:pointer; display:inline-block; padding:6px 8px; border-radius:8px; background:rgba(255,255,255,0.02); border:1px solid rgba(255,255,255,0.03)}
  </style>
</head>
<body>
  <div class="wrap">
    <div class="card">
      <header>
        <div class="avatar">SP</div>
        <div>
          <h1>Shantanu Pundir <span style="color:var(--accent); font-weight:600; font-size:14px">• Android Developer</span></h1>
          <p class="lead">🚀 Android Developer | 💻 Programmer | 📱 Tech Enthusiast — building clean, efficient, scalable apps.</p>
        </div>
      </header>

      <div class="grid">
        <main>
          <div class="section">
            <h3>About</h3>
            <p class="muted">I’m passionate about Android app development and love building applications that provide real value to users. With strong foundations in Java, Kotlin, Python, JavaScript, and hands-on experience with modern Android tools & architectures, I aim to craft clean, efficient, and scalable solutions.</p>

            <h4 style="margin-top:14px">What I build</h4>
            <ul>
              <li>Robust MVVM-based Android apps with offline-first Room databases.</li>
              <li>Clean UI using Jetpack components & Material Design.</li>
              <li>Performant network layers (Retrofit + Coroutines/Flow).</li>
              <li>Modular, testable code with DI (Hilt) and clear architecture.</li>
            </ul>

          </div>

          <div class="section" style="margin-top:14px">
            <h3>Tech Stack & Skills</h3>
            <div class="tech-badges">
              <span class="badge">Java</span>
              <span class="badge">Kotlin</span>
              <span class="badge">Python</span>
              <span class="badge">JavaScript</span>
              <span class="badge">MVVM</span>
              <span class="badge">Room</span>
              <span class="badge">Jetpack</span>
              <span class="badge">Retrofit</span>
              <span class="badge">Hilt</span>
              <span class="badge">Coroutines</span>
            </div>

            <div class="skills">
              <div style="min-width:220px">
                <strong class="muted">Android Development:</strong>
                <div class="muted">Room Database • MVVM Architecture • Jetpack Components (LiveData, ViewModel, Navigation)</div>
              </div>

              <div>
                <strong class="muted">Other:</strong>
                <div class="muted">API Integration • UI/UX design principles • Debugging & Optimization</div>
              </div>
            </div>
          </div>
        </main>

        <aside class="right">
          <div class="section">
            <h3>Contact</h3>
            <div class="contact">
              <a class="btn" href="https://www.linkedin.com/in/shantanu-pundir9/" target="_blank" rel="noopener">💼 LinkedIn</a>
              <a class="btn" href="mailto:ranaaryan997@gmail.com">✉️ Email</a>
              <div style="display:flex; gap:8px; align-items:center; margin-top:8px">
                <span class="muted">Email:</span>
                <span class="mono">ranaaryan997@gmail.com</span>
                <span class="copy" id="copyEmail" title="Copy email">📋</span>
              </div>
            </div>

            <div style="margin-top:12px">
              <h4 class="muted" style="margin:0 0 6px 0">GitHub Stats</h4>
              <div class="stats">
                <div class="stat-card">
                  <img src="https://github-readme-stats.vercel.app/api?username=Shantanu-Pundir&show_icons=true&include_all_commits=true&count_private=true" alt="GitHub stats" style="width:100%; border-radius:8px; display:block" />
                </div>
                <div class="stat-card">
                  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Shantanu-Pundir&layout=compact" alt="Top langs" style="width:100%; border-radius:8px; display:block" />
                </div>
              </div>
            </div>
          </div>

          <div class="section" style="margin-top:14px">
            <h3>Quick Setup</h3>
            <pre class="mono" style="margin:0; padding:10px; border-radius:8px; background:rgba(255,255,255,0.02);">git clone https://github.com/USERNAME/REPO.git
cd REPO
./gradlew assembleDebug</pre>
          </div>
        </aside>
      </div>

      <footer>
        <div>Built with ❤️ • <span class="muted">Android • Kotlin • MVVM</span></div>
        <div class="muted">© Shantanu Pundir</div>
      </footer>
    </div>
  </div>

  <script>
    // copy email interaction
    document.getElementById('copyEmail').addEventListener('click', async function(){
      try{
        await navigator.clipboard.writeText('ranaaryan997@gmail.com');
        this.textContent='✅';
        setTimeout(()=> this.textContent='📋',1200);
      }catch(e){
        alert('Copy failed — select and copy manually');
      }
    });

    // small accessibility: prefers-reduced-motion
    if (window.matchMedia('(prefers-reduced-motion: reduce)').matches){
      document.documentElement.style.scrollBehavior='auto';
    }
  </script>
</body>
</html>




📫 Connect with Me
💼 LinkedIn: https://www.linkedin.com/in/shantanu-pundir9/
📧 Email: ranaaryan997@gmail.com
