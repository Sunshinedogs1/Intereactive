file:///C:/Users/USER/AppData/Local/Temp/4597c989-4e5d-43e2-9526-782ba237b1eb_sunshine-pet-care-k9-training.zip.1eb/assets/logo.svg
# Intereactive
dog-progress
/* Sunshine Pet Care & K9 Training - Theme */
@import url('https://fonts.googleapis.com/css2?family=Baloo+2:wght@400;600;700&family=Nunito:wght@400;600;800&display=swap');
:root {
  --sunshine: #FFD23F; /* sunny yellow */
  --orange: #FF9F1C;
  --purple: #6A4C93;
  --blue: #1B9AAA;
  --green: #2CA58D;
  --bg: #FFF9E9;
  --text: #222;
}
* { box-sizing: border-box; }
html, body { margin: 0; padding: 0; background: var(--bg); color: var(--text); font-family: 'Nunito', system-ui, -apple-system; }
header {
  position: sticky; top: 0; z-index: 1000; background: white; box-shadow: 0 6px 18px rgba(0,0,0,.08);
}
.navbar { display: flex; align-items: center; gap: 1rem; padding: .75rem 1rem; max-width: 1200px; margin: 0 auto; }
.navbar img { width: 56px; height: 56px; }
.brand { font-family: 'Baloo 2'; font-weight: 800; font-size: 1.4rem; color: var(--purple); }
.navlinks { margin-left: auto; display: flex; flex-wrap: wrap; gap: .5rem; }
.navlinks a { text-decoration: none; color: var(--purple); background: #f4e8ff; padding: .5rem .8rem; border-radius: 999px; font-weight: 700; }
.navlinks a:hover { background: var(--sunshine); color: #3b2a63; }

.hero { display: grid; grid-template-columns: 1.1fr .9fr; gap: 2rem; align-items: center; max-width: 1200px; margin: 0 auto; padding: 2rem 1rem; }
.hero-card { background: white; border-radius: 24px; padding: 2rem; box-shadow: 0 12px 24px rgba(0,0,0,.08); }
.hero h1 { font-family: 'Baloo 2'; font-size: clamp(2rem, 4vw, 3rem); color: var(--orange); margin: 0 0 .5rem; }
.hero p { font-size: 1.2rem; }
.cta { display: flex; gap: 1rem; margin-top: 1rem; }
.btn { border: none; border-radius: 16px; padding: .8rem 1.2rem; font-weight: 800; cursor: pointer; }
.btn.primary { background: var(--orange); color: #fff; }
.btn.secondary { background: var(--blue); color: #fff; }
.btn.tertiary { background: var(--green); color: #fff; }
.btn:hover { filter: brightness(1.05); transform: translateY(-1px); transition: all .2s ease; }

.section { max-width: 1200px; margin: 0 auto; padding: 2rem 1rem; }
.section h2 { font-family: 'Baloo 2'; color: var(--purple); font-size: clamp(1.6rem, 3vw, 2.2rem); }
.grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(260px, 1fr)); gap: 1rem; }
.card { background: white; border-radius: 20px; padding: 1rem; box-shadow: 0 8px 18px rgba(0,0,0,.06); }
.card h3 { margin-top: 0; }
.badge { display: inline-flex; align-items: center; gap: .4rem; background: #fff3c4; color: #6a4c00; padding: .3rem .6rem; border-radius: 999px; font-weight: 700; }

/* Progress tracker */
.progress-wrapper { background: white; border-radius: 20px; padding: 1rem; box-shadow: 0 8px 18px rgba(0,0,0,.06); }
.progress-bar { height: 20px; background: #eee; border-radius: 999px; overflow: hidden; }
.progress-fill { height: 100%; width: 0%; background: linear-gradient(90deg, var(--green), var(--blue)); transition: width .8s ease; }
.levels { display: grid; grid-template-columns: repeat(5, 1fr); gap: .5rem; margin-top: 1rem; }
.level { text-align: center; padding: .6rem; border-radius: 12px; background: #f6fafe; border: 2px dashed #cde3f1; }
.level.unlocked { background: #e8fff6; border-color: #b5f0d9; }
.trophy { font-size: 2rem; }
.ribbon { display:inline-block; background: var(--sunshine); color:#5b4400; padding:.2rem .5rem; border-radius:8px; font-weight:800; }

footer { background: #fff; border-top: 1px solid #eee; }
footer .section { display: grid; gap: 1rem; }
.small { font-size: .9rem; color: #555; }

/* Responsive */
@media (max-width: 800px) { .hero { grid-template-columns: 1fr; } }
