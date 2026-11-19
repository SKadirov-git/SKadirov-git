<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Subhon | Software development &amp; creative technology</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Instrument+Serif:ital@0;1&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>
:root{--bg:#080A0D;--panel:#10151B;--line:#1B232C;--tx:#F2F4F5;--mu:#8B949E;--mint:#54E1C0;--blue:#7AA2FF;--warm:#DDAA72;
--serif:"Instrument Serif",Georgia,"Times New Roman",serif;--mono:"JetBrains Mono",ui-monospace,SFMono-Regular,Menlo,Consolas,monospace}
*{box-sizing:border-box;margin:0}
html{background:var(--bg);color-scheme:dark}
body{color:var(--tx);font:16px/1.6 var(--serif);-webkit-font-smoothing:antialiased}
a{color:var(--mint);text-decoration:none;border-bottom:1px solid transparent}
a:hover,a:focus-visible{border-color:var(--mint)}
.wrap{max-width:960px;margin:0 auto;padding:0 20px}
code,.mono{font-family:var(--mono)}

/* HERO */
.hero{position:relative;aspect-ratio:1200/380;container-type:inline-size;overflow:hidden;background:var(--bg);border-bottom:1px solid var(--line)}
.hero>*{position:absolute}
.grid{inset:0;background-image:linear-gradient(#151c24 1px,transparent 1px),linear-gradient(90deg,#151c24 1px,transparent 1px);background-size:3.333cqw 3.333cqw;-webkit-mask-image:radial-gradient(ellipse at center,#000 25%,transparent 85%);mask-image:radial-gradient(ellipse at center,#000 25%,transparent 85%)}
.marks{inset:0}
.marks .c{position:absolute;width:1.8cqw;height:1.8cqw;border:0 solid #5b636c}
.c.tl{left:2.3cqw;top:7.4%;border-width:1px 0 0 1px}.c.tr{right:2.3cqw;top:7.4%;border-width:1px 1px 0 0}
.c.bl{left:2.3cqw;bottom:7.4%;border-width:0 0 1px 1px}.c.br{right:2.3cqw;bottom:7.4%;border-width:0 1px 1px 0}
.hl{position:absolute;left:5.3%;right:5.3%;height:1px;background:#222b34;transform-origin:center}
.hl.t{top:14.7%}.hl.b{top:84.7%}
.x{position:absolute;font:.8cqw var(--mono);color:#4b6199;padding-left:.9cqw;white-space:nowrap}
.x::before{content:"+";position:absolute;left:-.45cqw;top:-.35cqw;font-size:1.3cqw;color:var(--blue);opacity:.7}
.meta{left:5.3%;right:5.3%;top:8.2%;display:flex;justify-content:space-between;font:1.08cqw var(--mono);letter-spacing:.05em;color:var(--mu)}
.term{left:26.7%;top:36%;font:2cqw/1.55 var(--mono);color:#dfe3e6}
.term b{color:var(--mint);font-weight:400}
.ln{margin:0}.clip{display:inline-block;white-space:nowrap}
.car{display:inline-block;width:1.1cqw;height:1.7cqw;margin-left:.3cqw;vertical-align:-.25cqw;background:var(--mint);animation:bl 1s steps(2) infinite}
@keyframes bl{50%{background:transparent}}
.bar{width:30cqw;height:.5cqw;margin-top:1.6cqw;border:1px solid #2a343e}
.bar span{display:block;height:100%;background:var(--mint);transform-origin:left}
.main{inset:0;display:flex;flex-direction:column;align-items:center;padding-top:22.5%}
.name{display:flex;font:400 11cqw/.9 var(--serif);letter-spacing:.167em;padding-left:.167em}
.name span{display:block;overflow:hidden;padding-bottom:.06em}.name i{display:block;font-style:normal}
.rule{width:8cqw;height:.3cqw;margin-top:2.2cqw;background:var(--mint);transform-origin:center}
.sub{margin-top:3.4cqw;font:1.42cqw var(--mono);letter-spacing:.25em;color:var(--mu);white-space:nowrap}
.tag{margin-top:1.3cqw;font:italic 2.6cqw/1.2 var(--serif);white-space:nowrap}
.cur{display:inline-block;width:.18cqw;height:2.2cqw;margin-left:.5cqw;vertical-align:-.3cqw;background:var(--warm);animation:bl 1s steps(2) infinite}
.status{left:5.3%;right:5.3%;bottom:3.2%;display:flex;justify-content:space-between;align-items:center;font:1.08cqw var(--mono);letter-spacing:.05em;color:var(--mu)}
.status .d{display:inline-block;width:.7cqw;height:.7cqw;margin-right:1.2cqw;border-radius:50%;background:var(--mint);box-shadow:0 0 0 0 rgba(84,225,192,.45);animation:pu 1.6s ease-out infinite}
@keyframes pu{to{box-shadow:0 0 0 1cqw rgba(84,225,192,0)}}

/* SECTIONS */
section{padding:56px 0 8px}
h2{display:flex;align-items:center;gap:16px;font:500 .78rem var(--mono);letter-spacing:.22em;color:var(--mu);margin-bottom:28px}
h2 em{font-style:normal;color:var(--mint)}
h2::after{content:"";flex:1;height:1px;background:linear-gradient(90deg,#3a444e,transparent)}
.lead{display:grid;grid-template-columns:1.5fr 1fr;gap:40px;align-items:start}
.lead p{font-size:1.4rem;line-height:1.45;margin-bottom:1rem}
.lead p:first-child{font-size:1.9rem;line-height:1.2}
dl{font:.85rem/1.9 var(--mono);background:var(--panel);border:1px solid var(--line);padding:18px 20px}
dl div{display:flex;gap:16px}dt{color:var(--mu);min-width:68px}dd{color:var(--tx)}
.shop{display:grid;grid-template-columns:repeat(4,1fr);gap:1px;background:var(--line);border:1px solid var(--line)}
.g{background:var(--bg);padding:20px}
.g h3{font:500 .72rem var(--mono);letter-spacing:.2em;color:var(--mu);margin-bottom:16px}
.g ul{list-style:none;padding:0}
.g li{display:flex;align-items:center;gap:12px;padding:7px 0;font:.9rem var(--mono)}
.g svg{width:24px;height:24px;flex:none}
.works{display:grid;grid-template-columns:1fr 1fr;gap:20px}
.card{background:var(--panel);border:1px solid var(--line);padding:22px;min-height:190px;display:flex;flex-direction:column}
.card .n{font:.75rem var(--mono);color:var(--mu)}
.card h3{font:400 2rem/1.1 var(--serif);margin:10px 0 8px}
.card h3 a{color:var(--tx)}
.card p{color:#b4bcc4;font-size:1.1rem;line-height:1.35}
.tags{margin-top:auto;padding-top:16px;display:flex;gap:8px;flex-wrap:wrap;align-items:center;font:.75rem var(--mono)}
.tags span{border:1px solid #2a343e;padding:2px 8px;color:var(--mu)}.tags a{margin-left:auto}
.card.slot{background:transparent;border:1px dashed #2a343e;justify-content:center;align-items:center;text-align:center}
.card.slot h3{color:var(--mu)}
pre{font:.92rem/1.9 var(--mono);background:var(--panel);border:1px solid var(--line);padding:20px 24px;color:var(--mint);overflow-x:auto}
pre s{text-decoration:none;color:var(--tx)}pre .car{height:1rem;width:.55rem;margin:0 0 0 2px;vertical-align:-.1rem}
.act img{display:block;width:100%}
.act .two{display:grid;grid-template-columns:1fr 1fr;gap:20px;margin-top:20px}
table{width:100%;border-collapse:collapse;font:.9rem var(--mono)}
th,td{text-align:left;padding:12px 16px;border-bottom:1px solid var(--line)}
th{color:var(--mu);font-weight:400;border-bottom-color:#2a343e}td:first-child{color:var(--mu);width:120px}
.ph{color:var(--mu)}
footer{text-align:center;padding:80px 20px 64px}
.dash{position:relative;width:min(680px,80%);height:9px;margin:0 auto 34px;background:repeating-linear-gradient(90deg,#3a444e 0 8px,transparent 8px 14px) center/100% 1px no-repeat;border-left:1px solid #4b555f;border-right:1px solid #4b555f}
.dash i{position:absolute;top:0;left:0;width:8px;height:8px;background:var(--mint);animation:mv 3s ease-in-out infinite alternate}
@keyframes mv{to{left:calc(100% - 8px)}}
footer p:first-of-type{font:clamp(1.1rem,3.2vw,2.1rem) var(--serif);letter-spacing:.1em}
footer p:last-child{margin-top:14px;font:.85rem var(--mono);color:var(--mu);letter-spacing:.05em}
@media(max-width:760px){.lead,.works,.act .two{grid-template-columns:1fr}.shop{grid-template-columns:1fr 1fr}
.hero{aspect-ratio:1/.9}.name{font-size:15cqw}.main{padding-top:30%}.sub{font-size:2.3cqw;letter-spacing:.12em}.tag{font-size:5cqw}
.term{left:8%;font-size:3.3cqw}.meta,.x,.status{font-size:2cqw}.x{display:none}.rule{width:16cqw}}
@media(prefers-reduced-motion:reduce){*{animation:none!important}}
</style>
</head>
<body>

<header class="hero" id="hero">
  <div class="grid" data-a="grid"></div>
  <div class="marks" aria-hidden="true">
    <div data-a="marks" style="position:absolute;inset:0">
      <i class="c tl"></i><i class="c tr"></i><i class="c bl"></i><i class="c br"></i>
      <span class="x" style="left:16.7%;top:31.6%">x200 y120</span>
      <span class="x" style="left:83.3%;top:65.8%">x1000 y250</span>
      <span class="x" style="left:13.3%;top:73.7%">x160 y280</span>
      <span class="x" style="left:78.3%;top:26.3%">x940 y100</span>
    </div>
    <b class="hl t" data-a="hl"></b><b class="hl b" data-a="hl"></b>
  </div>
  <div class="meta" data-a="meta" aria-hidden="true"><span>subhon / digital builder</span><span>tajikistan&nbsp; 38.86&deg;N 71.28&deg;E</span></div>
  <div class="term" data-a="term" aria-hidden="true">
    <p class="ln"><span class="clip" data-a="l1"><b>$</b> initializing creative workspace...<i class="car" data-a="c1"></i></span></p>
    <p class="ln"><span class="clip" data-a="l2"><b>$</b> loading developer identity...<i class="car"></i></span></p>
    <div class="bar" data-a="bar"><span data-a="fill"></span></div>
  </div>
  <div class="main" data-a="fade">
    <h1 class="name" aria-label="Subhon"><span><i>S</i></span><span><i>U</i></span><span><i>B</i></span><span><i>H</i></span><span><i>O</i></span><span><i>N</i></span></h1>
    <div class="rule" data-a="rule"></div>
    <p class="sub" data-a="sub">SOFTWARE DEVELOPMENT / CREATIVE TECHNOLOGY</p>
    <p class="tag"><span class="clip" data-a="tag">Building ideas into reality, one line at a time.</span><span data-a="cur"><i class="cur"></i></span></p>
  </div>
  <div class="status" data-a="status" aria-hidden="true"><span><i class="d"></i>status: building</span><span>midnight workshop</span></div>
</header>

<main class="wrap">

<section id="identity">
  <h2><em>01</em> / IDENTITY</h2>
  <div class="lead">
    <div>
      <p>I&rsquo;m Subhon, an aspiring software developer and creative technologist from Tajikistan. I learn by building: pick a problem, get something running, then make it better.</p>
      <p>Right now my public work is Android games written in Kotlin. My curiosity runs wider: C and C++ to understand how machines actually work, the web for things anyone can open with a click, and AI and cybersecurity for the questions that don&rsquo;t have tidy answers yet. Game development is where most of it meets.</p>
      <p>I&rsquo;m not trying to look finished. I&rsquo;m trying to keep shipping small, useful, well-made things, and to be a little better at it each month.</p>
    </div>
    <dl>
      <div><dt>name</dt><dd>Subhon</dd></div>
      <div><dt>role</dt><dd>aspiring software developer / creative technologist</dd></div>
      <div><dt>base</dt><dd>Tajikistan</dd></div>
      <div><dt>works</dt><dd>Kotlin, C, C++, web</dd></div>
      <div><dt>curious</dt><dd>AI, cybersecurity, game development</dd></div>
    </dl>
  </div>
</section>

<section id="workshop">
  <h2><em>02</em> / THE WORKSHOP</h2>
  <div class="shop">
    <div class="g"><h3>PROGRAMMING</h3><ul><li><svg aria-hidden="true" fill="#8B949E" role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M16.5921 9.1962s-.354-3.298-3.627-3.39c-3.2741-.09-4.9552 2.474-4.9552 6.14 0 3.6651 1.858 6.5972 5.0451 6.5972 3.184 0 3.5381-3.665 3.5381-3.665l6.1041.365s.36 3.31-2.196 5.836c-2.552 2.5241-5.6901 2.9371-7.8762 2.9201-2.19-.017-5.2261.034-8.1602-2.97-2.938-3.0101-3.436-5.9302-3.436-8.8002 0-2.8701.556-6.6702 4.047-9.5502C7.444.72 9.849 0 12.254 0c10.0422 0 10.7172 9.2602 10.7172 9.2602z"/></svg>C</li><li><svg aria-hidden="true" fill="#8B949E" role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M22.394 6c-.167-.29-.398-.543-.652-.69L12.926.22c-.509-.294-1.34-.294-1.848 0L2.26 5.31c-.508.293-.923 1.013-.923 1.6v10.18c0 .294.104.62.271.91.167.29.398.543.652.69l8.816 5.09c.508.293 1.34.293 1.848 0l8.816-5.09c.254-.147.485-.4.652-.69.167-.29.27-.616.27-.91V6.91c.003-.294-.1-.62-.268-.91zM12 19.11c-3.92 0-7.109-3.19-7.109-7.11 0-3.92 3.19-7.11 7.11-7.11a7.133 7.133 0 016.156 3.553l-3.076 1.78a3.567 3.567 0 00-3.08-1.78A3.56 3.56 0 008.444 12 3.56 3.56 0 0012 15.555a3.57 3.57 0 003.08-1.778l3.078 1.78A7.135 7.135 0 0112 19.11zm7.11-6.715h-.79v.79h-.79v-.79h-.79v-.79h.79v-.79h.79v.79h.79zm2.962 0h-.79v.79h-.79v-.79h-.79v-.79h.79v-.79h.79v.79h.79z"/></svg>C++</li><li><svg aria-hidden="true" fill="#8B949E" role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M24 24H0V0h24L12 12Z"/></svg>Kotlin</li></ul></div>
    <div class="g"><h3>WEB</h3><ul><li><svg aria-hidden="true" fill="#8B949E" role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M1.5 0h21l-1.91 21.563L11.977 24l-8.564-2.438L1.5 0zm7.031 9.75l-.232-2.718 10.059.003.23-2.622L5.412 4.41l.698 8.01h9.126l-.326 3.426-2.91.804-2.955-.81-.188-2.11H6.248l.33 4.171L12 19.351l5.379-1.443.744-8.157H8.531z"/></svg>HTML</li><li><svg aria-hidden="true" fill="#8B949E" role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M0 0v20.16A3.84 3.84 0 0 0 3.84 24h16.32A3.84 3.84 0 0 0 24 20.16V3.84A3.84 3.84 0 0 0 20.16 0Zm14.256 13.08c1.56 0 2.28 1.08 2.304 2.64h-1.608c.024-.288-.048-.6-.144-.84-.096-.192-.288-.264-.552-.264-.456 0-.696.264-.696.84-.024.576.288.888.768 1.08.72.288 1.608.744 1.92 1.296q.432.648.432 1.656c0 1.608-.912 2.592-2.496 2.592-1.656 0-2.4-1.032-2.424-2.688h1.68c0 .792.264 1.176.792 1.176.264 0 .456-.072.552-.24.192-.312.24-1.176-.048-1.512-.312-.408-.912-.6-1.32-.816q-.828-.396-1.224-.936c-.24-.36-.36-.888-.36-1.536 0-1.44.936-2.472 2.424-2.448m5.4 0c1.584 0 2.304 1.08 2.328 2.64h-1.608c0-.288-.048-.6-.168-.84-.096-.192-.264-.264-.528-.264-.48 0-.72.264-.72.84s.288.888.792 1.08c.696.288 1.608.744 1.92 1.296.264.432.408.984.408 1.656.024 1.608-.888 2.592-2.472 2.592-1.68 0-2.424-1.056-2.448-2.688h1.68c0 .744.264 1.176.792 1.176.264 0 .456-.072.552-.24.216-.312.264-1.176-.048-1.512-.288-.408-.888-.6-1.32-.816-.552-.264-.96-.576-1.2-.936s-.36-.888-.36-1.536c-.024-1.44.912-2.472 2.4-2.448m-11.031.018c.711-.006 1.419.198 1.839.63.432.432.672 1.128.648 1.992H9.336c.024-.456-.096-.792-.432-.96-.312-.144-.768-.048-.888.24-.12.264-.192.576-.168.864v3.504c0 .744.264 1.128.768 1.128a.65.65 0 0 0 .552-.264c.168-.24.192-.552.168-.84h1.776c.096 1.632-.984 2.712-2.568 2.688-1.536 0-2.496-.864-2.472-2.472v-4.032c0-.816.24-1.44.696-1.848.432-.408 1.146-.624 1.857-.63"/></svg>CSS</li><li><svg aria-hidden="true" fill="#8B949E" role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M0 0h24v24H0V0zm22.034 18.276c-.175-1.095-.888-2.015-3.003-2.873-.736-.345-1.554-.585-1.797-1.14-.091-.33-.105-.51-.046-.705.15-.646.915-.84 1.515-.66.39.12.75.42.976.9 1.034-.676 1.034-.676 1.755-1.125-.27-.42-.404-.601-.586-.78-.63-.705-1.469-1.065-2.834-1.034l-.705.089c-.676.165-1.32.525-1.71 1.005-1.14 1.291-.811 3.541.569 4.471 1.365 1.02 3.361 1.244 3.616 2.205.24 1.17-.87 1.545-1.966 1.41-.811-.18-1.26-.586-1.755-1.336l-1.83 1.051c.21.48.45.689.81 1.109 1.74 1.756 6.09 1.666 6.871-1.004.029-.09.24-.705.074-1.65l.046.067zm-8.983-7.245h-2.248c0 1.938-.009 3.864-.009 5.805 0 1.232.063 2.363-.138 2.711-.33.689-1.18.601-1.566.48-.396-.196-.597-.466-.83-.855-.063-.105-.11-.196-.127-.196l-1.825 1.125c.305.63.75 1.172 1.324 1.517.855.51 2.004.675 3.207.405.783-.226 1.458-.691 1.811-1.411.51-.93.402-2.07.397-3.346.012-2.054 0-4.109 0-6.179l.004-.056z"/></svg>JavaScript</li></ul></div>
    <div class="g"><h3>TOOLS</h3><ul><li><svg aria-hidden="true" fill="#8B949E" role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M13.09 23.549a1.54 1.54 0 0 1-2.18 0L.451 13.089a1.54 1.54 0 0 1 0-2.179l7.191-7.19 2.733 2.733a1.85 1.85 0 0 0 .964 2.326v6.66a1.849 1.849 0 1 0 1.54 0V8.957l2.508 2.508a1.85 1.85 0 1 0 1.09-1.09l-2.634-2.634a1.85 1.85 0 0 0-2.378-2.377L8.73 2.63 10.91.451a1.54 1.54 0 0 1 2.179 0l10.459 10.46a1.54 1.54 0 0 1 0 2.179z"/></svg>Git</li><li><svg aria-hidden="true" fill="#8B949E" role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61C4.422 18.07 3.633 17.7 3.633 17.7c-1.087-.744.084-.729.084-.729 1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.305 3.495.998.108-.776.417-1.305.76-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.606-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 22.092 24 17.592 24 12.297c0-6.627-5.373-12-12-12"/></svg>GitHub</li><li><svg aria-hidden="true" fill="#8B949E" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 128 128"><path fill-rule="evenodd" d="M90.767 127.126a7.968 7.968 0 0 0 6.35-.244l26.353-12.681a8 8 0 0 0 4.53-7.209V21.009a8 8 0 0 0-4.53-7.21L97.117 1.12a7.97 7.97 0 0 0-9.093 1.548l-50.45 46.026L15.6 32.013a5.328 5.328 0 0 0-6.807.302l-7.048 6.411a5.335 5.335 0 0 0-.006 7.888L20.796 64 1.74 81.387a5.336 5.336 0 0 0 .006 7.887l7.048 6.411a5.327 5.327 0 0 0 6.807.303l21.974-16.68 50.45 46.025a7.96 7.96 0 0 0 2.743 1.793Zm5.252-92.183L57.74 64l38.28 29.058V34.943Z" clip-rule="evenodd"/></svg>VS Code</li></ul></div>
    <div class="g"><h3>EXPLORING</h3><ul><li><svg aria-hidden="true" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="#54E1C0" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"><path d="M5 6.5L12 12M5 17.5L12 12M12 12L19 6.5M12 12L19 17.5"/><circle cx="5" cy="6.5" r="2"/><circle cx="5" cy="17.5" r="2"/><circle cx="12" cy="12" r="2.4"/><circle cx="19" cy="6.5" r="2"/><circle cx="19" cy="17.5" r="2"/></svg>AI</li><li><svg aria-hidden="true" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="#54E1C0" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"><path d="M12 3L19 6V12C19 16.3 16 19.5 12 21C8 19.5 5 16.3 5 12V6Z"/><circle cx="12" cy="10.6" r="1.7"/><path d="M12 12.4V15.2"/></svg>Cybersecurity</li><li><svg aria-hidden="true" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="#54E1C0" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"><rect x="2.5" y="7" width="19" height="10.5" rx="5"/><path d="M7 12.2H10.4M8.7 10.5V13.9"/><circle cx="15.2" cy="11.2" r="0.6"/><circle cx="17.6" cy="13.2" r="0.6"/></svg>Game dev</li></ul></div>
  </div>
</section>

<section id="works">
  <h2><em>03</em> / SELECTED WORKS</h2>
  <div class="works">
    <article class="card"><span class="n">01</span><h3><a href="https://github.com/SKadirov-git/ss-block-puzzle">ss-block-puzzle</a></h3><p>S&amp;S Block Puzzle, an Android game.</p>
      <div class="tags"><span>Kotlin</span><span>Android</span><a href="https://github.com/SKadirov-git/ss-block-puzzle">repository</a></div></article>
    <article class="card"><span class="n">02</span><h3><a href="https://github.com/SKadirov-git/Beatbounce">Beatbounce</a></h3><p>A game project written in Kotlin.</p>
      <div class="tags"><span>Kotlin</span><a href="https://github.com/SKadirov-git/Beatbounce">repository</a></div></article>
    <article class="card"><span class="n">03</span><h3><a href="https://github.com/SKadirov-git/Droids">Droids</a></h3><p>A game project written in Kotlin.</p>
      <div class="tags"><span>Kotlin</span><a href="https://github.com/SKadirov-git/Droids">repository</a></div></article>
    <article class="card slot"><span class="n">04</span><h3>Next build</h3><p>Open slot for the next project worth showing.</p></article>
  </div>
</section>

<section id="experiments">
  <h2><em>04</em> / CURRENT EXPERIMENTS</h2>
<pre>$ <s>current_focus</s>
&gt; experimenting with new ideas
&gt; improving problem-solving
&gt; building useful software
$ <i class="car"></i></pre>
</section>

<section id="activity" class="act">
  <h2><em>05</em> / GITHUB ACTIVITY</h2>
  <img loading="lazy" src="https://ghchart.rshah.org/54e1c0/SKadirov-git" alt="Contribution graph for SKadirov-git over the last year">
  <div class="two">
    <img loading="lazy" src="https://github-readme-stats.vercel.app/api/top-langs/?username=SKadirov-git&amp;layout=compact&amp;hide_border=true&amp;bg_color=10151B&amp;title_color=54E1C0&amp;text_color=8B949E&amp;card_width=420" alt="Most used languages across SKadirov-git repositories">
    <img loading="lazy" src="https://streak-stats.demolab.com?user=SKadirov-git&amp;hide_border=true&amp;background=10151B&amp;ring=54E1C0&amp;fire=DDAA72&amp;currStreakNum=F2F4F5&amp;sideNums=F2F4F5&amp;currStreakLabel=54E1C0&amp;sideLabels=8B949E&amp;dates=8B949E" alt="Contribution streak for SKadirov-git">
  </div>
</section>

<section id="connections">
  <h2><em>06</em> / CONNECTIONS</h2>
  <table>
    <tr><th>channel</th><th>link</th></tr>
    <tr><td>github</td><td><a href="https://github.com/SKadirov-git">github.com/SKadirov-git</a></td></tr>
    <tr><td>linkedin</td><td><a class="ph" href="https://www.linkedin.com/in/YOUR-HANDLE">linkedin.com/in/YOUR-HANDLE</a></td></tr>
    <tr><td>email</td><td><a class="ph" href="mailto:YOUR-EMAIL">YOUR-EMAIL</a></td></tr>
    <tr><td>website</td><td><a class="ph" href="https://YOUR-WEBSITE">YOUR-WEBSITE</a></td></tr>
  </table>
</section>

</main>

<footer>
  <div class="dash" aria-hidden="true"><i></i></div>
  <p>THE BEST IDEAS ARE STILL UNDER CONSTRUCTION.</p>
  <p>Designed &amp; developed by Subhon.</p>
</footer>

<script>
(()=>{
if(matchMedia('(prefers-reduced-motion: reduce)').matches)return;
const T=8,$=s=>document.querySelector(`[data-a="${s}"]`),$$=s=>[...document.querySelectorAll(`[data-a="${s}"]`)];
const go=(el,st)=>el&&el.animate(st.map(([s,p])=>({offset:s/T,...p})),{duration:T*1e3,iterations:Infinity});
const op=(...v)=>v.map(([s,o,e])=>[s,{opacity:o,...(e?{easing:e}:{})}]);
const cl=(a,b)=>`inset(0 ${a}% 0 0)`;
go($('grid'),op([0,0],[.15,0],[1.5,1],[7.4,1],[8,0]));
go($('marks'),op([0,0],[.5,0],[1.5,1],[7.4,1],[8,0]));
$$('hl').forEach(e=>go(e,[[0,{transform:'scaleX(0)'}],[.5,{transform:'scaleX(0)'}],[1.5,{transform:'scaleX(1)'}],[8,{transform:'scaleX(1)'}]]));
go($('meta'),op([0,0],[1,0],[1.6,1],[7.4,1],[8,0]));
go($('term'),op([0,1],[3.5,1],[3.85,0],[8,0]));
go($('l1'),[[0,{clipPath:cl(100)}],[1.15,{clipPath:cl(100),easing:'steps(33,end)'}],[1.95,{clipPath:cl(0)}],[8,{clipPath:cl(0)}]]);
go($('c1'),op([0,1],[2.1,1],[2.15,0],[8,0]));
go($('l2'),[[0,{clipPath:cl(100)}],[2.15,{clipPath:cl(100),easing:'steps(29,end)'}],[2.85,{clipPath:cl(0)}],[8,{clipPath:cl(0)}]]);
go($('bar'),op([0,0],[2.4,0],[2.5,1],[8,1]));
go($('fill'),[[0,{transform:'scaleX(0)'}],[2.45,{transform:'scaleX(0)',easing:'ease-in-out'}],[3.35,{transform:'scaleX(1)'}],[8,{transform:'scaleX(1)'}]]);
go($('fade'),op([0,1],[7.4,1],[8,0]));
document.querySelectorAll('.name i').forEach((e,k)=>{const s=3.75+.07*k;
 go(e,[[0,{transform:'translateY(110%)'}],[s,{transform:'translateY(110%)',easing:'cubic-bezier(.2,.7,.2,1)'}],[s+.6,{transform:'translateY(0)'}],[8,{transform:'translateY(0)'}]]);});
go($('rule'),[[0,{transform:'scaleX(0)'}],[4.45,{transform:'scaleX(0)',easing:'ease-out'}],[4.95,{transform:'scaleX(1)'}],[8,{transform:'scaleX(1)'}]]);
const sb=(y)=>({opacity:y,transform:`translateY(${y?0:8}px)`});
go($('sub'),[[0,sb(0)],[4.95,{...sb(0),easing:'ease-out'}],[5.6,sb(1)],[8,sb(1)]]);
go($('tag'),[[0,{clipPath:cl(100)}],[5.5,{clipPath:cl(100),easing:'ease-in-out'}],[6.3,{clipPath:cl(0)}],[8,{clipPath:cl(0)}]]);
go($('cur'),op([0,0],[6.35,0],[6.36,1],[8,1]));
go($('status'),op([0,0],[6.2,0],[6.7,1],[7.4,1],[8,0]));
})();
</script>
</body>
</html>
