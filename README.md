<!-- README.md for GitHub profile: chornsokreaksa -->
<div align="center">

<!-- ===== Header: Animated starfield + comet ===== -->
<svg viewBox="0 0 900 220" width="100%" height="200" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid slice" style="background: linear-gradient(180deg,#020111 0%, #2b0b3a 100%); border-radius: 12px;">
  <defs>
    <radialGradient id="g1"><stop offset="0" stop-color="#fff" stop-opacity="0.95"/><stop offset="1" stop-color="#fff" stop-opacity="0"/></radialGradient>
    <filter id="blur"><feGaussianBlur stdDeviation="1.2" /></filter>
    <g id="star">
      <circle cx="0" cy="0" r="1.6" fill="url(#g1)" />
    </g>
    <linearGradient id="tail" x1="0" x2="1">
      <stop offset="0" stop-color="#fff" stop-opacity="0.9"/>
      <stop offset="1" stop-color="#fff" stop-opacity="0"/>
    </linearGradient>
  </defs>

  <!-- random-ish stars (static: GitHub caches but still looks nice) -->
  <g id="stars" fill="#fff" fill-opacity="0.9" transform="translate(0,0)">
    <use href="#star" x="40"  y="22"  style="opacity:0.9; transform-origin:40px 22px;">
      <animate attributeName="opacity" values="0.1;0.9;0.1" dur="3.6s" repeatCount="indefinite" begin="0s"/>
    </use>
    <use href="#star" x="110" y="80" style="opacity:0.7;">
      <animate attributeName="opacity" values="0.2;1;0.2" dur="4.2s" repeatCount="indefinite" begin="0.3s"/>
    </use>
    <use href="#star" x="200" y="30" style="opacity:0.8;">
      <animate attributeName="opacity" values="0.1;1;0.1" dur="5s" repeatCount="indefinite" begin="0.7s"/>
    </use>
    <use href="#star" x="300" y="140" style="opacity:0.6;">
      <animate attributeName="opacity" values="0.2;0.95;0.2" dur="3.2s" repeatCount="indefinite" begin="0.4s"/>
    </use>
    <use href="#star" x="420" y="50" style="opacity:0.7;">
      <animate attributeName="opacity" values="0.1;0.9;0.1" dur="4.6s" repeatCount="indefinite" begin="0.1s"/>
    </use>
    <use href="#star" x="600" y="120" style="opacity:0.8;">
      <animate attributeName="opacity" values="0.1;0.95;0.1" dur="6s" repeatCount="indefinite" begin="0.8s"/>
    </use>
    <use href="#star" x="780" y="30" style="opacity:0.7;">
      <animate attributeName="opacity" values="0.2;1;0.2" dur="4.8s" repeatCount="indefinite" begin="0.5s"/>
    </use>
  </g>

  <!-- twinkling large planet / moon -->
  <g transform="translate(140,110)">
    <circle cx="0" cy="0" r="28" fill="#c8c8ff" fill-opacity="0.06" />
    <circle cx="0" cy="0" r="16" fill="#bfc4ff" fill-opacity="0.16">
      <animate attributeName="r" values="15;17;15" dur="6s" repeatCount="indefinite"/>
    </circle>
  </g>

  <!-- comet (moving across) -->
  <g id="comet" transform="translate(-120,40)" opacity="0.95">
    <g transform="rotate(-12)">
      <ellipse cx="0" cy="0" rx="40" ry="6" fill="url(#tail)" />
      <circle cx="50" cy="0" r="3.8" fill="#fff" />
    </g>
    <animateTransform attributeName="transform" type="translate"
      values="-120,40; 980,-40" dur="6.2s" repeatCount="indefinite" />
  </g>

  <!-- main title (centered) -->
  <foreignObject x="0" y="40" width="900" height="140">
    <div xmlns="http://www.w3.org/1999/xhtml" style="width:100%;height:100%;display:flex;flex-direction:column;align-items:center;justify-content:center;">
      <h1 style="margin:0;color:#fff;font-family:system-ui,-apple-system,Segoe UI,Roboto;letter-spacing:1px;font-size:34px;">
        ✨ chornsokreaksa — cosmic coder ✨
      </h1>

      <p style="margin:8px 0 0 0;color:#d8c8ff;opacity:0.95;font-family:ui-sans-serif,system-ui,Segoe UI,Roboto;font-size:14px;">
        <span style="white-space:pre"> </span>
        <span style="display:inline-block;vertical-align:middle;">
          <span style="border-right:2px solid rgba(255,255,255,0.6);padding-right:8px;animation: typing 3s steps(30,end) infinite;">
            aligning code with constellations...
          </span>
        </span>
      </p>

      <style>
        @keyframes typing { 0% { width:0 } 50% { width:260px } 100% { width:0 } }
      </style>
    </div>
  </foreignObject>
</svg>

</div>

<!-- ===== Profile section (HTML inside markdown) ===== -->
<div align="center" style="margin-top:14px;">

<p align="center" style="font-size:15px; margin:6px 0 12px 0;">
  Hi — I'm <strong>Reaksa</strong> (aka <code>@chornsokreaksa</code>) — an obsessive stargazer & developer.  
  I build microservices, tame clouds, and read star charts like bug reports.
</p>

<!-- Skill badges (simple emoji + text) -->
<p>
  🚀 <strong>Tech:</strong> Node.js · Python · Docker · AWS · MongoDB &nbsp; • &nbsp;
  🧭 <strong>Focus:</strong> microservices · infra · automation
</p>

<!-- Animated project cards using CSS-only hover (works in GitHub flavor to some extent) -->
<div style="display:flex;gap:14px;justify-content:center;flex-wrap:wrap;margin-top:16px;">
  <div style="width:250px;border-radius:12px;padding:12px;background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));backdrop-filter:blur(4px);box-shadow:0 8px 30px rgba(20,10,40,0.35);transition:transform .35s;transform-origin:center;">
    <h3 style="margin:4px 0 6px 0;color:#e8dfff;">🌌 Microservices</h3>
    <p style="margin:0 0 8px 0;color:#cfc7ef;font-size:13px;">APIs that behave like constellations: decoupled, observable, resilient.</p>
    <a href="#" style="font-size:13px;text-decoration:none;color:#fff;padding:6px 10px;border-radius:8px;background:linear-gradient(90deg,#6d28d9,#9f7aea);display:inline-block;">Explore →</a>
  </div>

  <div style="width:250px;border-radius:12px;padding:12px;background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));backdrop-filter:blur(4px);box-shadow:0 8px 30px rgba(20,10,40,0.35);transition:transform .35s;transform-origin:center;">
    <h3 style="margin:4px 0 6px 0;color:#e8dfff;">☁️ Cloud & Infra</h3>
    <p style="margin:0 0 8px 0;color:#cfc7ef;font-size:13px;">Docker, AWS, k8s patterns & deployment pipelines — production-ready.</p>
    <a href="#" style="font-size:13px;text-decoration:none;color:#fff;padding:6px 10px;border-radius:8px;background:linear-gradient(90deg,#07c;#6d28d9);display:inline-block;">Infra →</a>
  </div>

  <div style="width:250px;border-radius:12px;padding:12px;background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));backdrop-filter:blur(4px);box-shadow:0 8px 30px rgba(20,10,40,0.35);transition:transform .35s;transform-origin:center;">
    <h3 style="margin:4px 0 6px 0;color:#e8dfff;">🔭 Research</h3>
    <p style="margin:0 0 8px 0;color:#cfc7ef;font-size:13px;">Security, small ML tools, and astro-inspired side projects.</p>
    <a href="#" style="font-size:13px;text-decoration:none;color:#fff;padding:6px 10px;border-radius:8px;background:linear-gradient(90deg,#9f7aea,#06b);display:inline-block;">Read →</a>
  </div>
</div>

</div>

<!-- ===== Footer with stats & socials ===== -->
<div align="center" style="margin-top:18px;">
  <!-- GitHub stats (uses third-party service - keep if you want dynamic images) -->
  <img src="https://github-readme-stats.vercel.app/api?username=chornsokreaksa&show_icons=true&theme=dark" alt="chornsokreaksa github stats" style="max-width:100%;border-radius:8px;margin-top:10px;" />

  <p style="margin-top:10px;font-size:13px;color:#bfb3ff;">
    Connect with me — <a href="https://www.linkedin.com/" target="_blank">LinkedIn</a> • <a href="https://twitter.com/" target="_blank">X</a> • <a href="mailto:your@email.com">Email</a>
  </p>
</div>
