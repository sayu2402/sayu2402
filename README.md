<!--
  Professional GitHub Profile README (HTML template)
  Instructions:
  - Copy this HTML into your repository's README.md or into the GitHub profile README (in a repo named <your-username>.github.io or profile README repo).
  - Replace placeholders: {{NAME}}, {{TITLE}}, {{SHORT_BIO}}, {{LOCATION}}, {{EMAIL}}, {{LINKEDIN_URL}}, {{TWITTER_URL}}, {{RESUME_URL}}, and project sections.
  - Shields/badges and repo widgets are already included as examples.
  - GitHub strips some CSS in markdown-rendered READMEs (but inline styles and simple HTML usually work). If something is stripped, convert to Markdown using the section contents.
-->

<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>{{NAME}} — GitHub Profile README</title>
  <style>
    /* Simple, self-contained styling suitable for GitHub README (inline CSS). Keep selectors narrow to reduce collisions. */
    .gh-card{max-width:980px;margin:18px auto;padding:20px;border-radius:12px;background:#0b1220;color:#e6eef6;font-family:Inter,system-ui,-apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,"Helvetica Neue",Arial;box-shadow:0 6px 20px rgba(2,6,23,0.6);}
    .gh-header{display:flex;gap:18px;align-items:center}
    .avatar{width:108px;height:108px;border-radius:12px;flex:0 0 108px;object-fit:cover;border:2px solid rgba(255,255,255,0.06)}
    .title{display:flex;flex-direction:column}
    .title h1{margin:0;font-size:22px;letter-spacing:-0.4px}
    .title p{margin:6px 0 0;color:#a9bbcf}
    .badges{margin-top:10px;display:flex;gap:8px;flex-wrap:wrap}
    .badges img{height:20px}

    .grid{display:grid;grid-template-columns:1fr 320px;gap:18px;margin-top:20px}
    .panel{background:linear-gradient(180deg,rgba(255,255,255,0.02),transparent);padding:16px;border-radius:10px;border:1px solid rgba(255,255,255,0.03)}

    ul.skills{display:flex;flex-wrap:wrap;gap:8px;padding:0;margin:0;list-style:none}
    ul.skills li{background:rgba(255,255,255,0.03);padding:8px 10px;border-radius:8px;font-size:13px}

    .projects .proj{margin-bottom:12px}
    .proj a{font-weight:600;color:#dbefff;text-decoration:none}
    .stats{display:flex;gap:8px;flex-direction:column}
    .contact a{display:inline-block;margin-right:10px;margin-bottom:8px;text-decoration:none;padding:8px 10px;border-radius:8px;background:rgba(255,255,255,0.02);color:#cfe7ff}

    .footer{margin-top:18px;color:#92a7c4;font-size:13px}
    @media (max-width:880px){.grid{grid-template-columns:1fr;}.avatar{width:88px;height:88px}}
  </style>
</head>
<body>
  <div class="gh-card">
    <div class="gh-header">
      <!-- Avatar: replace the src with your avatar or GitHub profile image URL -->
      <img class="avatar" src="https://github.com/{{USERNAME}}.png" alt="{{NAME}} avatar" />
      <div class="title">
        <h1>{{NAME}} <span style="color:#7fd0ff;font-weight:600">• {{TITLE}}</span></h1>
        <p>{{SHORT_BIO}}</p>
        <div class="badges">
          <!-- Example shields (edit to your details) -->
          <img src="https://img.shields.io/badge/Status-Open%20to%20Work-green?style=for-the-badge&logo=linkedin" alt="open to work" />
          <img src="https://img.shields.io/badge/TopLangs-Python%20%7C%20JavaScript-blue?style=for-the-badge&logo=python" alt="top langs" />
          <img src="https://img.shields.io/badge/Followers-{{FOLLOWERS}}-informational?style=for-the-badge&logo=github" alt="followers" />
        </div>
      </div>
    </div>

    <div class="grid">
      <!-- Left: About + Skills + Projects -->
      <div>
        <div class="panel">
          <h3>About</h3>
          <p style="color:#bcd3ea;margin-top:8px">📍 {{LOCATION}} • ✉️ <a href="mailto:{{EMAIL}}">{{EMAIL}}</a></p>
          <p style="margin-top:12px;color:#d7e9ff">{{LONGER_BIO}}
          </p>
        </div>

        <div class="panel" style="margin-top:12px">
          <h3>Core Skills</h3>
          <ul class="skills">
            <li>Python</li>
            <li>Django / DRF</li>
            <li>REST APIs</li>
            <li>SQL</li>
            <li>Docker</li>
            <li>React</li>
            <li>Unit testing</li>
          </ul>
        </div>

        <div class="panel projects" style="margin-top:12px">
          <h3>Featured Projects</h3>
          <div class="proj">
            <a href="https://github.com/{{USERNAME}}/project-1">project-1</a>
            <div style="color:#a9bbcf;font-size:13px">Short one-line description of project-1 — tech used: Django, PostgreSQL, Docker</div>
          </div>
          <div class="proj">
            <a href="https://github.com/{{USERNAME}}/project-2">project-2</a>
            <div style="color:#a9bbcf;font-size:13px">Short one-line description of project-2 — tech used: React, Vite, Tailwind</div>
          </div>
          <div class="proj">
            <a href="https://github.com/{{USERNAME}}/project-3">project-3</a>
            <div style="color:#a9bbcf;font-size:13px">Short one-line description of project-3 — what problem it solves</div>
          </div>
        </div>

      </div>

      <!-- Right: Stats / Socials / Contact -->
      <div>
        <div class="panel">
          <h3>GitHub Stats</h3>
          <!-- GitHub stats cards (these are images from third-party services) -->
          <div style="margin-top:10px">
            <img src="https://github-readme-stats.vercel.app/api?username={{USERNAME}}&show_icons=true&hide_border=true" alt="GitHub stats" style="max-width:100%;border-radius:8px" />
          </div>
          <div style="margin-top:10px">
            <img src="https://github-readme-streak-stats.herokuapp.com/?user={{USERNAME}}&hide_border=true" alt="GitHub streak" style="max-width:100%;border-radius:8px" />
          </div>
        </div>

        <div class="panel" style="margin-top:12px">
          <h3>Contact & Socials</h3>
          <div class="contact" style="margin-top:8px">
            <a href="https://github.com/{{USERNAME}}">GitHub</a>
            <a href="{{LINKEDIN_URL}}">LinkedIn</a>
            <a href="{{TWITTER_URL}}">Twitter</a>
            <a href="mailto:{{EMAIL}}">Email</a>
          </div>
          <div style="margin-top:8px;color:#9ec6ff;font-size:13px">Resume: <a href="{{RESUME_URL}}">Download</a></div>
        </div>

        <div class="panel" style="margin-top:12px">
          <h3>Open to</h3>
          <p style="color:#bcd3ea">• Full-time roles • Freelance / contract • Mentoring</p>
        </div>

      </div>
    </div>

    <div class="footer">
      <div>🔭 Currently working on: <strong>project-1</strong> • 🌱 Learning: GraphQL & Kubernetes</div>
      <div style="margin-top:6px">✨ Fun fact: I love anime, especially <em>One Piece</em>.</div>
    </div>
  </div>
</body>
</html>
