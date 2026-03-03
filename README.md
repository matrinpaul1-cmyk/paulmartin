# paulmartin
Mon portfolio
[index.html](https://github.com/user-attachments/files/25727441/index.html)
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Paul Martin — Portfolio · Marketing &amp; Business Development</title>
  <meta name="description" content="Portfolio de Paul Martin, étudiant en BUT Techniques de Commercialisation. Marketing stratégique, vente, alternance Nespresso, semestre UQAC Canada. En recherche de master." />
  <meta name="keywords" content="Paul Martin, portfolio, BUT TC, marketing, vente, Nespresso, UQAC, école de commerce, alternance, business development" />
  <meta name="author" content="Paul Martin" />
  <meta name="robots" content="index, follow" />
  <!-- Open Graph -->
  <meta property="og:type" content="website" />
  <meta property="og:title" content="Paul Martin — Portfolio Marketing &amp; Business" />
  <meta property="og:description" content="Étudiant BUT TC, alternant Nespresso, semestre international Canada. Marketing stratégique, vente premium, orienté résultats." />
  <meta property="og:locale" content="fr_FR" />
  <!-- Twitter Card -->
  <meta name="twitter:card" content="summary_large_image" />
  <meta name="twitter:title" content="Paul Martin — Portfolio" />
  <meta name="twitter:description" content="Étudiant BUT TC, alternant Nespresso, semestre international Canada." />
  <!-- Favicon inline -->
  <link rel="icon" href="data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'><text y='.9em' font-size='90'>P</text></svg>" />
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;0,600;1,300;1,400&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet" />
  <style>
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
    :root {
      --white: #ffffff; --off-white: #f8f8f6; --light: #f0eeea; --muted: #c8c4bc;
      --mid: #8a8680; --dark: #2a2825; --black: #0d0c0b;
      --accent: #9a7c5a; --accent-light: #e8dfd4;
      --serif: 'Cormorant Garamond', Georgia, serif;
      --sans: 'DM Sans', Helvetica, sans-serif;
      --radius: 2px; --ease: cubic-bezier(0.25, 0.46, 0.45, 0.94);
    }
    html { scroll-behavior: smooth; scroll-padding-top: 80px; }
    body { font-family: var(--sans); background: var(--white); color: var(--black); font-size: 16px; line-height: 1.6; overflow-x: hidden; cursor: none; }
    @media (hover: none), (pointer: coarse) {
      body { cursor: auto; }
      .cursor, .cursor-ring { display: none !important; }
    }

    .cursor { width: 8px; height: 8px; background: var(--black); border-radius: 50%; position: fixed; top: 0; left: 0; pointer-events: none; z-index: 9999; transition: transform 0.15s var(--ease); transform: translate(-50%, -50%); }
    .cursor-ring { width: 32px; height: 32px; border: 1px solid rgba(0,0,0,0.3); border-radius: 50%; position: fixed; top: 0; left: 0; pointer-events: none; z-index: 9998; transition: transform 0.4s var(--ease), width 0.3s, height 0.3s, border-color 0.2s; transform: translate(-50%, -50%); }

    nav { position: fixed; top: 0; left: 0; right: 0; z-index: 100; display: flex; align-items: center; justify-content: space-between; padding: 0 60px; height: 72px; background: rgba(255,255,255,0.88); backdrop-filter: blur(20px); -webkit-backdrop-filter: blur(20px); border-bottom: 1px solid rgba(0,0,0,0.06); }
    .nav-logo { font-family: var(--serif); font-size: 20px; font-weight: 400; color: var(--black); text-decoration: none; }
    .nav-links { display: flex; gap: 36px; list-style: none; }
    .nav-links a { font-size: 12px; font-weight: 400; letter-spacing: 0.08em; text-transform: uppercase; color: var(--mid); text-decoration: none; transition: color 0.2s; }
    .nav-links a:hover { color: var(--black); }

    section { padding: 140px 0; }
    .container { max-width: 1160px; margin: 0 auto; padding: 0 60px; }

    .reveal { opacity: 0; transform: translateY(36px); transition: opacity 0.85s var(--ease), transform 0.85s var(--ease); }
    .reveal.visible { opacity: 1; transform: translateY(0); }
    .reveal-delay-1 { transition-delay: 0.1s; }
    .reveal-delay-2 { transition-delay: 0.2s; }
    .reveal-delay-3 { transition-delay: 0.3s; }
    .reveal-delay-4 { transition-delay: 0.45s; }

    /* HERO */
    #hero { min-height: 100vh; display: flex; align-items: center; position: relative; padding: 0; background: var(--white); overflow: hidden; }
    .hero-bg-text { position: absolute; top: 50%; right: -40px; transform: translateY(-50%); font-family: var(--serif); font-size: clamp(120px, 18vw, 260px); font-weight: 300; color: transparent; -webkit-text-stroke: 1px rgba(0,0,0,0.04); letter-spacing: -0.04em; line-height: 1; pointer-events: none; user-select: none; white-space: nowrap; }
    .hero-inner { display: grid; grid-template-columns: 1fr 1fr; gap: 80px; align-items: center; width: 100%; max-width: 1160px; margin: 0 auto; padding: 140px 60px; }
    .hero-eyebrow { font-size: 11px; font-weight: 500; letter-spacing: 0.2em; text-transform: uppercase; color: var(--accent); margin-bottom: 28px; display: flex; align-items: center; gap: 12px; }
    .hero-eyebrow::before { content: ''; display: block; width: 40px; height: 1px; background: var(--accent); }
    .hero-name { font-family: var(--serif); font-size: clamp(52px, 7vw, 96px); font-weight: 300; line-height: 1.05; letter-spacing: -0.02em; color: var(--black); margin-bottom: 8px; }
    .hero-name em { font-style: italic; color: var(--accent); }
    .hero-title { font-size: 13px; font-weight: 400; letter-spacing: 0.06em; text-transform: uppercase; color: var(--mid); margin-bottom: 32px; }
    .hero-desc { font-size: 18px; font-weight: 300; line-height: 1.75; color: var(--dark); max-width: 440px; margin-bottom: 48px; }
    .hero-btns { display: flex; gap: 16px; flex-wrap: wrap; }
    .hero-cta { display: inline-flex; align-items: center; gap: 10px; padding: 15px 32px; background: var(--black); color: var(--white); font-size: 12px; font-weight: 500; letter-spacing: 0.07em; text-transform: uppercase; text-decoration: none; border-radius: var(--radius); transition: background 0.25s, transform 0.25s; }
    .hero-cta:hover { background: var(--accent); transform: translateY(-2px); }
    .hero-cta svg { transition: transform 0.25s; }
    .hero-cta:hover svg { transform: translateX(4px); }
    .hero-cta-outline { display: inline-flex; align-items: center; gap: 10px; padding: 15px 32px; background: transparent; color: var(--black); font-size: 12px; font-weight: 500; letter-spacing: 0.07em; text-transform: uppercase; text-decoration: none; border: 1px solid var(--muted); border-radius: var(--radius); transition: border-color 0.25s, background 0.25s, transform 0.25s; }
    .hero-cta-outline:hover { border-color: var(--black); transform: translateY(-2px); }

    .hero-visual { position: relative; display: flex; align-items: center; justify-content: center; }
    .hero-photo-wrap { width: 100%; max-width: 400px; aspect-ratio: 3/4; border-radius: 4px; overflow: hidden; position: relative; box-shadow: 0 40px 80px rgba(0,0,0,0.12); }
    .hero-photo-wrap img { width: 100%; height: 100%; object-fit: cover; object-position: top center; filter: grayscale(15%); transition: filter 0.5s; }
    .hero-photo-wrap:hover img { filter: grayscale(0%); }
    .hero-photo-overlay { position: absolute; bottom: 0; left: 0; right: 0; background: linear-gradient(to top, rgba(13,12,11,0.8) 0%, transparent 60%); padding: 32px; }
    .hero-photo-name { font-family: var(--serif); font-size: 24px; font-weight: 300; color: var(--white); margin-bottom: 4px; }
    .hero-photo-sub { font-size: 11px; letter-spacing: 0.12em; text-transform: uppercase; color: rgba(255,255,255,0.55); }
    .hero-badge { position: absolute; top: 24px; right: -24px; background: var(--white); border: 1px solid var(--light); padding: 14px 20px; border-radius: 4px; box-shadow: 0 12px 40px rgba(0,0,0,0.1); text-align: center; }
    .hero-badge-num { font-family: var(--serif); font-size: 28px; font-weight: 300; color: var(--accent); line-height: 1; }
    .hero-badge-txt { font-size: 10px; letter-spacing: 0.1em; text-transform: uppercase; color: var(--mid); margin-top: 4px; }
    .hero-badge-2 { position: absolute; bottom: -24px; left: -24px; background: var(--black); padding: 14px 20px; border-radius: 4px; box-shadow: 0 12px 40px rgba(0,0,0,0.18); text-align: center; }
    .hero-badge-2 .hero-badge-num { color: var(--accent); }
    .hero-badge-2 .hero-badge-txt { color: rgba(255,255,255,0.4); }

    /* ABOUT */
    #about { background: var(--off-white); }
    .about-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 100px; align-items: start; }
    .section-label { font-size: 11px; font-weight: 500; letter-spacing: 0.2em; text-transform: uppercase; color: var(--accent); margin-bottom: 20px; display: flex; align-items: center; gap: 14px; }
    .section-label::after { content: ''; display: block; width: 48px; height: 1px; background: var(--accent); }
    .section-title { font-family: var(--serif); font-size: clamp(34px, 5vw, 56px); font-weight: 300; line-height: 1.1; letter-spacing: -0.01em; color: var(--black); margin-bottom: 22px; }
    .section-title em { font-style: italic; color: var(--accent); }
    .section-body { font-size: 17px; font-weight: 300; line-height: 1.8; color: var(--dark); max-width: 560px; }
    .about-quote { margin-top: 40px; padding: 28px 36px; border-left: 2px solid var(--accent); background: var(--accent-light); }
    .about-quote blockquote { font-family: var(--serif); font-size: 19px; font-weight: 300; font-style: italic; line-height: 1.6; color: var(--dark); }
    .about-quote cite { display: block; margin-top: 10px; font-size: 11px; letter-spacing: 0.1em; text-transform: uppercase; color: var(--accent); font-style: normal; }
    .about-traits { display: grid; grid-template-columns: 1fr 1fr; gap: 1px; background: var(--muted); border: 1px solid var(--muted); }
    .trait { background: var(--off-white); padding: 24px; transition: background 0.25s; }
    .trait:hover { background: var(--white); }
    .trait-icon { width: 32px; height: 32px; margin-bottom: 12px; color: var(--accent); }
    .trait-name { font-size: 12px; font-weight: 500; letter-spacing: 0.06em; text-transform: uppercase; color: var(--black); margin-bottom: 6px; }
    .trait-desc { font-size: 13px; font-weight: 300; color: var(--mid); line-height: 1.55; }
    .kpi-row { display: grid; grid-template-columns: repeat(3, 1fr); gap: 2px; background: var(--muted); border: 1px solid var(--muted); margin-top: 40px; }
    .kpi-box { background: var(--white); padding: 22px 16px; text-align: center; }
    .kpi-num { font-family: var(--serif); font-size: 28px; font-weight: 300; color: var(--accent); line-height: 1; margin-bottom: 5px; }
    .kpi-label { font-size: 10px; font-weight: 400; letter-spacing: 0.08em; text-transform: uppercase; color: var(--mid); }

    /* PARCOURS */
    #parcours { background: var(--white); }
    .parcours-timeline { margin-top: 56px; display: flex; flex-direction: column; border-left: 1px solid var(--muted); padding-left: 48px; margin-left: 20px; }
    .timeline-item { position: relative; padding-bottom: 60px; }
    .timeline-item:last-child { padding-bottom: 0; }
    .timeline-dot { position: absolute; left: -57px; top: 4px; width: 16px; height: 16px; border-radius: 50%; background: var(--white); border: 2px solid var(--accent); transition: background 0.3s; }
    .timeline-item:hover .timeline-dot { background: var(--accent); }
    .timeline-year { font-size: 11px; font-weight: 500; letter-spacing: 0.15em; text-transform: uppercase; color: var(--accent); margin-bottom: 10px; }
    .timeline-school { font-family: var(--serif); font-size: 26px; font-weight: 300; color: var(--black); margin-bottom: 4px; }
    .timeline-degree { font-size: 13px; font-weight: 400; color: var(--mid); letter-spacing: 0.04em; margin-bottom: 18px; }
    .timeline-pills { display: flex; flex-wrap: wrap; gap: 8px; }
    .pill { padding: 5px 13px; background: var(--light); border-radius: var(--radius); font-size: 12px; color: var(--dark); border: 1px solid var(--muted); }

    /* Canada gallery */
    .canada-gallery { display: grid; grid-template-columns: 1fr 1fr; gap: 8px; margin-top: 20px; border-radius: 4px; overflow: hidden; }
    .canada-gallery img { width: 100%; height: 160px; object-fit: cover; display: block; transition: transform 0.4s var(--ease); }
    .canada-gallery:hover img { transform: scale(1.03); }

    /* COMPÉTENCES */
    #competences { background: var(--black); }
    #competences .section-label { color: var(--accent); }
    #competences .section-title { color: var(--white); }
    .comp-grid { margin-top: 56px; display: grid; grid-template-columns: repeat(3, 1fr); gap: 1px; background: rgba(255,255,255,0.07); border: 1px solid rgba(255,255,255,0.07); }
    .comp-col { padding: 44px 36px; background: var(--black); transition: background 0.3s; }
    .comp-col:hover { background: #141311; }
    .comp-col-num { font-family: var(--serif); font-size: 60px; font-weight: 300; color: var(--accent); opacity: 0.35; line-height: 1; margin-bottom: 18px; }
    .comp-col-title { font-size: 10px; font-weight: 500; letter-spacing: 0.2em; text-transform: uppercase; color: var(--accent); margin-bottom: 24px; padding-bottom: 14px; border-bottom: 1px solid rgba(154,124,90,0.2); }
    .comp-list { list-style: none; display: flex; flex-direction: column; gap: 12px; }
    .comp-list li { font-size: 13px; font-weight: 300; color: rgba(255,255,255,0.6); display: flex; align-items: center; gap: 10px; line-height: 1.4; }
    .comp-list li::before { content: ''; width: 4px; height: 4px; border-radius: 50%; background: var(--accent); flex-shrink: 0; }

    /* OUTILS */
    #outils { background: var(--off-white); }
    .tools-grid { margin-top: 56px; display: grid; grid-template-columns: repeat(6, 1fr); gap: 14px; }
    .tool-card { background: var(--white); border: 1px solid var(--light); padding: 26px 16px; text-align: center; border-radius: 4px; transition: transform 0.3s var(--ease), box-shadow 0.3s var(--ease), border-color 0.3s; }
    .tool-card:hover { transform: translateY(-4px); box-shadow: 0 16px 40px rgba(0,0,0,0.07); border-color: var(--accent); }
    .tool-icon { width: 40px; height: 40px; margin: 0 auto 12px; display: flex; align-items: center; justify-content: center; color: var(--accent); }
    .tool-name { font-size: 11px; font-weight: 500; letter-spacing: 0.06em; text-transform: uppercase; color: var(--dark); }

    /* EXPÉRIENCES */
    #experiences { background: var(--white); }
    .exp-grid { margin-top: 56px; display: grid; grid-template-columns: 1fr 1fr; gap: 2px; background: var(--light); }
    .exp-card { background: var(--white); padding: 44px; position: relative; overflow: hidden; transition: background 0.3s; }
    .exp-card:hover { background: var(--off-white); }
    .exp-card-accent { position: absolute; top: 0; left: 0; width: 3px; height: 0; background: var(--accent); transition: height 0.5s var(--ease); }
    .exp-card:hover .exp-card-accent { height: 100%; }
    .exp-period { font-size: 11px; font-weight: 500; letter-spacing: 0.15em; text-transform: uppercase; color: var(--accent); margin-bottom: 12px; }
    .exp-company { font-family: var(--serif); font-size: 26px; font-weight: 300; color: var(--black); margin-bottom: 4px; }
    .exp-role { font-size: 13px; font-weight: 400; color: var(--mid); letter-spacing: 0.04em; margin-bottom: 22px; }
    .exp-points { list-style: none; display: flex; flex-direction: column; gap: 9px; }
    .exp-points li { font-size: 13px; font-weight: 300; color: var(--dark); display: flex; align-items: flex-start; gap: 10px; line-height: 1.5; }
    .exp-points li::before { content: '—'; color: var(--accent); flex-shrink: 0; font-size: 11px; margin-top: 2px; }
    .exp-kpi { margin-top: 20px; padding: 14px 18px; background: var(--accent-light); border-radius: 2px; font-size: 12px; color: var(--accent); }
    .exp-kpi strong { font-weight: 500; }

    /* PROJETS */
    #projets { background: var(--off-white); }
    .projects-grid { margin-top: 56px; display: grid; grid-template-columns: repeat(3, 1fr); gap: 18px; }
    .project-card { background: var(--white); border-radius: 4px; overflow: hidden; border: 1px solid var(--light); transition: transform 0.35s var(--ease), box-shadow 0.35s var(--ease); cursor: none; }
    .project-card:hover { transform: translateY(-6px); box-shadow: 0 24px 60px rgba(0,0,0,0.09); }
    .project-thumb { height: 200px; overflow: hidden; position: relative; }
    .project-thumb img { width: 100%; height: 100%; object-fit: cover; transition: transform 0.5s var(--ease); }
    .project-card:hover .project-thumb img { transform: scale(1.05); }
    .project-thumb-placeholder { width: 100%; height: 100%; display: flex; align-items: center; justify-content: center; }
    .project-body { padding: 26px; }
    .project-tag { font-size: 10px; font-weight: 500; letter-spacing: 0.15em; text-transform: uppercase; color: var(--accent); margin-bottom: 9px; }
    .project-title { font-family: var(--serif); font-size: 19px; font-weight: 400; color: var(--black); margin-bottom: 8px; line-height: 1.3; }
    .project-desc { font-size: 13px; font-weight: 300; color: var(--mid); line-height: 1.6; }

    /* TÉMOIGNAGES */
    #temoignages { background: var(--white); }
    .temo-grid { margin-top: 56px; display: grid; grid-template-columns: repeat(2, 1fr); gap: 20px; }
    .temo-card { padding: 36px; border: 1px solid var(--light); border-radius: 4px; position: relative; transition: border-color 0.3s, box-shadow 0.3s; }
    .temo-card:hover { border-color: var(--accent); box-shadow: 0 12px 40px rgba(0,0,0,0.05); }
    .temo-stars { display: flex; gap: 3px; margin-bottom: 18px; color: #f0a500; font-size: 16px; }
    .temo-text { font-family: var(--serif); font-size: 18px; font-weight: 300; font-style: italic; line-height: 1.7; color: var(--dark); margin-bottom: 20px; }
    .temo-author { font-size: 12px; font-weight: 500; letter-spacing: 0.08em; text-transform: uppercase; color: var(--accent); }
    .temo-source { font-size: 11px; color: var(--muted); margin-top: 2px; }
    .temo-quote-mark { position: absolute; top: 20px; right: 28px; font-family: var(--serif); font-size: 80px; color: var(--light); line-height: 1; font-weight: 300; }

    /* CONTACT */
    #contact { background: var(--black); padding: 100px 0; }
    #contact .section-label { color: var(--accent); }
    #contact .section-title { color: var(--white); }
    .contact-inner { display: grid; grid-template-columns: 1fr 1fr; gap: 80px; align-items: start; }
    .contact-desc { font-size: 17px; font-weight: 300; color: rgba(255,255,255,0.55); line-height: 1.8; margin-top: 22px; }
    .contact-links { display: flex; flex-direction: column; gap: 14px; margin-top: 44px; }
    .contact-link { display: flex; align-items: center; gap: 16px; padding: 18px 22px; background: rgba(255,255,255,0.04); border: 1px solid rgba(255,255,255,0.08); border-radius: 4px; text-decoration: none; transition: background 0.25s, border-color 0.25s, transform 0.25s; color: inherit; }
    .contact-link:hover { background: rgba(154,124,90,0.12); border-color: var(--accent); transform: translateX(4px); }
    .contact-link-icon { width: 38px; height: 38px; border-radius: 50%; background: rgba(255,255,255,0.05); display: flex; align-items: center; justify-content: center; color: var(--accent); flex-shrink: 0; }
    .contact-link-label { font-size: 10px; font-weight: 500; letter-spacing: 0.12em; text-transform: uppercase; color: var(--mid); margin-bottom: 2px; }
    .contact-link-value { font-size: 13px; font-weight: 300; color: rgba(255,255,255,0.75); }
    .contact-form { margin-top: 8px; }
    .form-row { display: grid; grid-template-columns: 1fr 1fr; gap: 14px; margin-bottom: 14px; }
    .form-group { display: flex; flex-direction: column; gap: 7px; margin-bottom: 14px; }
    .form-label { font-size: 10px; font-weight: 500; letter-spacing: 0.12em; text-transform: uppercase; color: rgba(255,255,255,0.35); }
    .form-input, .form-textarea { background: rgba(255,255,255,0.04); border: 1px solid rgba(255,255,255,0.1); border-radius: 2px; padding: 13px 16px; color: var(--white); font-family: var(--sans); font-size: 14px; font-weight: 300; transition: border-color 0.25s; resize: none; outline: none; }
    .form-input:focus, .form-textarea:focus { border-color: var(--accent); }
    .form-textarea { height: 110px; }
    .form-submit { padding: 15px 36px; background: var(--accent); color: var(--white); font-family: var(--sans); font-size: 12px; font-weight: 500; letter-spacing: 0.08em; text-transform: uppercase; border: none; border-radius: 2px; cursor: none; transition: background 0.25s, transform 0.25s; }
    .form-submit:hover { background: #876847; transform: translateY(-2px); }
    .form-submit.sent { background: #4a7c5a; }

    footer { padding: 28px 60px; background: var(--black); border-top: 1px solid rgba(255,255,255,0.06); display: flex; align-items: center; justify-content: space-between; }
    .footer-name { font-family: var(--serif); font-size: 16px; font-weight: 300; color: rgba(255,255,255,0.35); }
    .footer-copy { font-size: 11px; color: rgba(255,255,255,0.18); letter-spacing: 0.06em; }

    ::-webkit-scrollbar { width: 3px; }
    ::-webkit-scrollbar-track { background: var(--white); }
    ::-webkit-scrollbar-thumb { background: var(--muted); border-radius: 2px; }

    @media (max-width: 900px) {
      nav { padding: 0 20px; }
      .nav-links { gap: 20px; }
      .hero-inner { grid-template-columns: 1fr; padding: 100px 24px 60px; }
      .hero-visual { display: none; }
      .about-grid, .contact-inner { grid-template-columns: 1fr; gap: 40px; }
      .comp-grid, .exp-grid { grid-template-columns: 1fr; }
      .tools-grid { grid-template-columns: repeat(3, 1fr); }
      .projects-grid { grid-template-columns: 1fr; }
      .temo-grid { grid-template-columns: 1fr; }
      .container { padding: 0 20px; }
      .form-row { grid-template-columns: 1fr; }
      footer { padding: 20px; flex-direction: column; gap: 6px; text-align: center; }
    }
  </style>
</head>
<body>
  <div class="cursor" id="cursor"></div>
  <div class="cursor-ring" id="cursorRing"></div>

  <nav>
    <a href="#hero" class="nav-logo">Paul Martin</a>
    <ul class="nav-links">
      <li><a href="#about">À propos</a></li>
      <li><a href="#parcours">Parcours</a></li>
      <li><a href="#competences">Compétences</a></li>
      <li><a href="#experiences">Expériences</a></li>
      <li><a href="#projets">Projets</a></li>
      <li><a href="#temoignages">Témoignages</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <!-- HERO -->
  <section id="hero">
    <div class="hero-bg-text">Martin</div>
    <div class="hero-inner">
      <div>
        <div class="hero-eyebrow reveal">Portfolio Académique &amp; Professionnel</div>
        <h1 class="hero-name reveal reveal-delay-1">Paul<br><em>Martin</em></h1>
        <p class="hero-title reveal reveal-delay-2">BUT Techniques de Commercialisation · Marketing · Vente · Stratégie</p>
        <p class="hero-desc reveal reveal-delay-3">Construire des stratégies marketing et commerciales fondées sur l'analyse, la créativité et la compréhension du client.</p>
        <div class="hero-btns reveal reveal-delay-4">
          <a href="#parcours" class="hero-cta">Voir mon parcours <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="5" y1="12" x2="19" y2="12"/><polyline points="12 5 19 12 12 19"/></svg></a>
          <a href="#contact" class="hero-cta-outline">Me contacter</a>
        </div>
      </div>
      <div class="hero-visual reveal reveal-delay-2">
        <div class="hero-photo-wrap">
          <img loading="lazy" src="images/photo.jpg" alt="Paul Martin" />
          <div class="hero-photo-overlay">
            <div class="hero-photo-name">Paul Martin</div>
            <div class="hero-photo-sub">BUT TC · Nespresso · UQAC Canada</div>
          </div>
        </div>
        <div class="hero-badge">
          <div class="hero-badge-num">+111%</div>
          <div class="hero-badge-txt">Objectif Nespresso</div>
        </div>
        <div class="hero-badge-2">
          <div class="hero-badge-num">895</div>
          <div class="hero-badge-txt">TOEIC Score</div>
        </div>
      </div>
    </div>
  </section>

  <!-- ABOUT -->
  <section id="about">
    <div class="container">
      <div class="about-grid">
        <div>
          <p class="section-label reveal">À propos</p>
          <h2 class="section-title reveal reveal-delay-1">Analytique,<br><em>orienté résultats.</em></h2>
          <p class="section-body reveal reveal-delay-2">Étudiant en BUT Techniques de Commercialisation à Issoudun, j'ai construit un parcours résolument international avec un semestre au Canada (UQAC) et une alternance chez Nespresso. Mon ambition : intégrer un master en école de commerce pour évoluer dans le marketing stratégique, le business development ou le consulting.</p>
          <div class="about-quote reveal reveal-delay-3">
            <blockquote>« Le succès c'est d'aller d'échec en échec sans perdre son enthousiasme. »</blockquote>
            <cite>Winston Churchill</cite>
          </div>
        </div>
        <div>
          <div class="about-traits reveal reveal-delay-1">
            <div class="trait">
              <svg class="trait-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><circle cx="12" cy="12" r="10"/><path d="M12 8v4l3 3"/></svg>
              <div class="trait-name">Persévérant</div>
              <div class="trait-desc">Je ne rien abandonne, que ce soit dans mes projets personnels ou académiques.</div>
            </div>
            <div class="trait">
              <svg class="trait-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"/><circle cx="9" cy="7" r="4"/><path d="M23 21v-2a4 4 0 0 0-3-3.87"/><path d="M16 3.13a4 4 0 0 1 0 7.75"/></svg>
              <div class="trait-name">Esprit d'équipe</div>
              <div class="trait-desc">À plusieurs on va plus loin. La diversité des idées est une force.</div>
            </div>
            <div class="trait">
              <svg class="trait-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><polyline points="22 12 18 12 15 21 9 3 6 12 2 12"/></svg>
              <div class="trait-name">Analytique</div>
              <div class="trait-desc">Orienté données et résultats, je pilote ma performance par les KPI.</div>
            </div>
            <div class="trait">
              <svg class="trait-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/></svg>
              <div class="trait-name">Optimiste</div>
              <div class="trait-desc">Il vaut mieux être optimiste et se tromper que pessimiste et avoir raison.</div>
            </div>
          </div>
          <div class="kpi-row reveal reveal-delay-2">
            <div class="kpi-box"><div class="kpi-num">B2</div><div class="kpi-label">Niveau anglais</div></div>
            <div class="kpi-box"><div class="kpi-num">895</div><div class="kpi-label">Score TOEIC</div></div>
            <div class="kpi-box"><div class="kpi-num">+111%</div><div class="kpi-label">Obj. Nespresso</div></div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- PARCOURS -->
  <section id="parcours">
    <div class="container">
      <p class="section-label reveal">Parcours Académique</p>
      <h2 class="section-title reveal reveal-delay-1">Formation &amp; <em>expérience internationale</em></h2>
      <div class="parcours-timeline">
        <div class="timeline-item reveal">
          <div class="timeline-dot"></div>
          <div class="timeline-year">2023 – 2026 · En cours</div>
          <div class="timeline-school">BUT Techniques de Commercialisation</div>
          <div class="timeline-degree">IUT d'Issoudun, France · Marketing · Vente · Communication</div>
          <div class="timeline-pills">
            <span class="pill">Analyse de marché</span><span class="pill">PESTEL / SWOT</span><span class="pill">Marketing mix 4P</span><span class="pill">Négociation commerciale</span><span class="pill">CRM</span><span class="pill">Communication digitale</span><span class="pill">KPI / Reporting</span><span class="pill">Power BI</span>
          </div>
        </div>
        <div class="timeline-item reveal reveal-delay-1">
          <div class="timeline-dot"></div>
          <div class="timeline-year">Août 2024 – Janvier 2025 · Semestre international</div>
          <div class="timeline-school">Baccalauréat en Administration</div>
          <div class="timeline-degree">UQAC – Université du Québec à Chicoutimi, Canada</div>
          <div class="timeline-pills">
            <span class="pill">Gestion financière</span><span class="pill">Entrepreneuriat</span><span class="pill">Marketing stratégique</span><span class="pill">Veille économique mondiale</span><span class="pill">Pitch devant jury</span><span class="pill">Business plan</span>
          </div>
          <div class="canada-gallery reveal reveal-delay-2">
            <img loading="lazy" src="images/canada.png" alt="UQAC Canada" style="object-position: left top;" />
            <img loading="lazy" src="images/canada.png" alt="UQAC Campus" style="object-position: right bottom;" />
          </div>
        </div>
        <div class="timeline-item reveal reveal-delay-2">
          <div class="timeline-dot"></div>
          <div class="timeline-year">2021 – 2023</div>
          <div class="timeline-school">Baccalauréat STMG</div>
          <div class="timeline-degree">France · Marketing · Gestion &amp; Finance · RH</div>
          <div class="timeline-pills">
            <span class="pill">Marketing</span><span class="pill">Gestion &amp; Finance</span><span class="pill">Ressources humaines</span><span class="pill">Communication</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- COMPÉTENCES -->
  <section id="competences">
    <div class="container">
      <p class="section-label reveal">Compétences</p>
      <h2 class="section-title reveal reveal-delay-1">Trois piliers,<br><em>une vision.</em></h2>
      <div class="comp-grid">
        <div class="comp-col reveal">
          <div class="comp-col-num">01</div>
          <div class="comp-col-title">Marketing</div>
          <ul class="comp-list">
            <li>Analyse de marché &amp; segmentation</li><li>Études consommateurs</li><li>Positionnement de marque (STP)</li><li>Stratégie marketing (4P)</li><li>Marketing digital</li><li>Veille concurrentielle</li><li>Brand management</li><li>PESTEL / SWOT</li>
          </ul>
        </div>
        <div class="comp-col reveal reveal-delay-1">
          <div class="comp-col-num">02</div>
          <div class="comp-col-title">Vente &amp; Business Dev.</div>
          <ul class="comp-list">
            <li>Négociation commerciale</li><li>Relation client premium</li><li>Parcours d'achat &amp; CX</li><li>Développement du CA</li><li>Upselling / Cross-selling</li><li>Fidélisation client (CRM)</li><li>Pilotage KPI &amp; ROI</li><li>Techniques SONCASE / CROC</li>
          </ul>
        </div>
        <div class="comp-col reveal reveal-delay-2">
          <div class="comp-col-num">03</div>
          <div class="comp-col-title">Communication</div>
          <ul class="comp-list">
            <li>Communication digitale</li><li>Création de contenu</li><li>Branding &amp; storytelling</li><li>Rédaction de communiqués</li><li>Réseaux sociaux</li><li>Design graphique (Canva)</li><li>Présentation &amp; pitch</li><li>Communication interne</li>
          </ul>
        </div>
      </div>
    </div>
  </section>

  <!-- OUTILS -->
  <section id="outils">
    <div class="container">
      <p class="section-label reveal">Outils &amp; Technologies</p>
      <h2 class="section-title reveal reveal-delay-1">Maîtrise <em>technique</em></h2>
      <div class="tools-grid">
        <div class="tool-card reveal"><div class="tool-icon"><svg width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><polyline points="14 2 14 8 20 8"/><line x1="16" y1="13" x2="8" y2="13"/><line x1="16" y1="17" x2="8" y2="17"/></svg></div><div class="tool-name">Excel</div></div>
        <div class="tool-card reveal reveal-delay-1"><div class="tool-icon"><svg width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><rect x="2" y="3" width="20" height="14" rx="2"/><line x1="8" y1="21" x2="16" y2="21"/><line x1="12" y1="17" x2="12" y2="21"/></svg></div><div class="tool-name">Power BI</div></div>
        <div class="tool-card reveal reveal-delay-2"><div class="tool-icon"><svg width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><rect x="3" y="3" width="18" height="18" rx="2"/><circle cx="8.5" cy="8.5" r="1.5"/><polyline points="21 15 16 10 5 21"/></svg></div><div class="tool-name">Canva</div></div>
        <div class="tool-card reveal reveal-delay-3"><div class="tool-icon"><svg width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><circle cx="12" cy="12" r="3"/><path d="M19.07 4.93a10 10 0 0 1 0 14.14"/><path d="M4.93 4.93a10 10 0 0 0 0 14.14"/></svg></div><div class="tool-name">Claude AI</div></div>
        <div class="tool-card reveal reveal-delay-1"><div class="tool-icon"><svg width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M21 16V8a2 2 0 0 0-1-1.73l-7-4a2 2 0 0 0-2 0l-7 4A2 2 0 0 0 3 8v8a2 2 0 0 0 1 1.73l7 4a2 2 0 0 0 2 0l7-4A2 2 0 0 0 21 16z"/></svg></div><div class="tool-name">PowerPoint</div></div>
        <div class="tool-card reveal reveal-delay-2"><div class="tool-icon"><svg width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><line x1="18" y1="20" x2="18" y2="10"/><line x1="12" y1="20" x2="12" y2="4"/><line x1="6" y1="20" x2="6" y2="14"/></svg></div><div class="tool-name">Data Analyse</div></div>
      </div>
    </div>
  </section>

  <!-- EXPÉRIENCES -->
  <section id="experiences">
    <div class="container">
      <p class="section-label reveal">Expériences Professionnelles</p>
      <h2 class="section-title reveal reveal-delay-1">Terrain &amp; <em>excellence opérationnelle</em></h2>
      <div class="exp-grid">
        <div class="exp-card reveal">
          <div class="exp-card-accent"></div>
          <div class="exp-period">Août 2025 – Août 2026 · Alternance</div>
          <div class="exp-company">Nespresso</div>
          <div class="exp-role">Spécialiste Café — Conseiller Commercial · Tours</div>
          <ul class="exp-points">
            <li>Conseil client premium et accompagnement personnalisé</li>
            <li>Démonstration des Grands Crus et animation dégustations</li>
            <li>Fidélisation Nespresso Club, upselling &amp; cross-selling</li>
            <li>Analyse des performances via tableau de bord Power BI</li>
          </ul>
          <div class="exp-kpi"><strong>KPIs :</strong> Panier Moyen 98% · Cde Moyenne 99% · Vertuo +103% · Accessoires +111%</div>
        </div>
        <div class="exp-card reveal reveal-delay-1">
          <div class="exp-card-accent"></div>
          <div class="exp-period">Juillet 2023 — Août 2024 · Saisonnier</div>
          <div class="exp-company">Château de la Bourdaisière</div>
          <div class="exp-role">Employé Polyvalent · Montlouis-sur-Loire</div>
          <ul class="exp-points">
            <li>Service client en environnement hôtelier haut de gamme</li>
            <li>Coordination des équipes en conditions exigeantes</li>
            <li>Valorisation de l'image du domaine et de ses événements</li>
          </ul>
        </div>
        <div class="exp-card reveal reveal-delay-2">
          <div class="exp-card-accent"></div>
          <div class="exp-period">Juillet 2023 · Officiel</div>
          <div class="exp-company">Championnats du Monde FISEC-FICEP</div>
          <div class="exp-role">Arbitre International · Dunkerque</div>
          <ul class="exp-points">
            <li>Arbitrage officiel en compétition internationale</li>
            <li>Gestion du stress et prise de décision sous pression</li>
            <li>Management de jeunes sportifs</li>
          </ul>
        </div>
        <div class="exp-card reveal reveal-delay-3">
          <div class="exp-card-accent"></div>
          <div class="exp-period">2022 – Présent · Bénévolat</div>
          <div class="exp-company">Basket &amp; Engagement</div>
          <div class="exp-role">Arbitre National FFBB · Président BDE</div>
          <ul class="exp-points">
            <li>Arbitre national de basketball en championnat de France</li>
            <li>Joueur et formateur de jeunes basketteurs</li>
            <li>Président BDE : management, budget, organisation d'événements</li>
          </ul>
        </div>
      </div>
    </div>
  </section>

  <!-- PROJETS -->
  <section id="projets">
    <div class="container">
      <p class="section-label reveal">Projets &amp; Réalisations</p>
      <h2 class="section-title reveal reveal-delay-1">Ce que j'ai <em>construit</em></h2>
      <div class="projects-grid">

        <div class="project-card reveal">
          <div class="project-thumb">
            <img loading="lazy" src="images/issoudurable.png" alt="IssouDurable" />
          </div>
          <div class="project-body">
            <div class="project-tag">Projet transverse · Entrepreneuriat</div>
            <div class="project-title">IssouDurable — Friperie innovante</div>
            <div class="project-desc">Création d'une friperie étudiante alliant mode durable, accessibilité et engagement écologique. Démocratiser la mode seconde main pour les jeunes actifs.</div>
          </div>
        </div>

        <div class="project-card reveal reveal-delay-1">
          <div class="project-thumb">
            <img loading="lazy" src="images/combier.png" alt="Combier La Folie" />
          </div>
          <div class="project-body">
            <div class="project-tag">Stratégie · Étude de marché</div>
            <div class="project-title">Distillerie Combier — Lancement La Folie</div>
            <div class="project-desc">Analyse concurrentielle complète du marché du sirop (475M€), positionnement et stratégie de lancement du nouveau produit artisanal premium.</div>
          </div>
        </div>

        <div class="project-card reveal reveal-delay-2">
          <div class="project-thumb">
            <img loading="lazy" src="images/combier2.png" alt="Analyse concurrentielle" />
          </div>
          <div class="project-body">
            <div class="project-tag">Analyse · Business Intelligence</div>
            <div class="project-title">Forces &amp; faiblesses concurrentielles — Sirop</div>
            <div class="project-desc">Benchmark approfondi des acteurs (Teisseire, Monin, 1883, Moulin de Valdonne) — parts de marché, positionnement et recommandations stratégiques.</div>
          </div>
        </div>

        <div class="project-card reveal reveal-delay-1">
          <div class="project-thumb">
            <img loading="lazy" src="images/sanex.png" alt="Flyer Sanex" />
          </div>
          <div class="project-body">
            <div class="project-tag">Communication · Design</div>
            <div class="project-title">Flyer produit — Sanex Friendly</div>
            <div class="project-desc">Création d'un flyer publicitaire produit pour le lancement de Sanex Friendly. Maîtrise du sens de lecture, hiérarchie visuelle et impact message.</div>
          </div>
        </div>

        <div class="project-card reveal reveal-delay-2">
          <div class="project-thumb">
            <img loading="lazy" src="images/presse.png" alt="Communiqué de presse" />
          </div>
          <div class="project-body">
            <div class="project-tag">Communication · Rédaction</div>
            <div class="project-title">Communiqué de presse — Musée Hospice Saint-Roch</div>
            <div class="project-desc">Rédaction d'un communiqué de presse professionnel pour valoriser le musée d'Issoudun. Structure, ton éditorial et respect des codes du genre.</div>
          </div>
        </div>

        <div class="project-card reveal reveal-delay-3">
          <div class="project-thumb">
            <div class="project-thumb-placeholder" style="background: linear-gradient(135deg, #2a2825 0%, #9a7c5a 100%);">
              <span style="font-family:var(--serif);font-size:70px;font-weight:300;color:rgba(255,255,255,0.18);">06</span>
            </div>
          </div>
          <div class="project-body">
            <div class="project-tag">Finance · Marchés</div>
            <div class="project-title">Système de veille — Marchés financiers</div>
            <div class="project-desc">Mise en place d'un système personnel de suivi et d'analyse de différents marchés financiers. Curiosité autodidacte pour la gestion de patrimoine.</div>
          </div>
        </div>

      </div>
    </div>
  </section>

  <!-- TÉMOIGNAGES -->
  <section id="temoignages">
    <div class="container">
      <p class="section-label reveal">Témoignages Clients</p>
      <h2 class="section-title reveal reveal-delay-1">Ce qu'ils disent <em>de moi</em></h2>
      <div class="temo-grid">
        <div class="temo-card reveal">
          <div class="temo-quote-mark">"</div>
          <div class="temo-stars">★★★★★</div>
          <div class="temo-text">Je tiens à remercier sincèrement Thomas et Paul de la boutique Nespresso de Tours pour leur accueil exceptionnel. Ils ont été non seulement très professionnels, mais aussi particulièrement à l'écoute, bienveillants et pleins de bonne humeur. Leur qualité de conseil et leur gentillesse ont vraiment rendu ma visite agréable.</div>
          <div class="temo-author">Audrey Fosse</div>
          <div class="temo-source">Avis Google · Boutique Nespresso Tours · Local Guide</div>
        </div>
        <div class="temo-card reveal reveal-delay-1">
          <div class="temo-quote-mark">"</div>
          <div class="temo-stars">★★★★★</div>
          <div class="temo-text">Mention à Paul, qui nous a super bien accueillis et ce qui est du café : TOP ! Il a été à l'écoute et nous a conseillés de la meilleure des manières. Je recommande !</div>
          <div class="temo-author">Sabrina Medienne</div>
          <div class="temo-source">Avis Google · Boutique Nespresso Tours</div>
        </div>
      </div>
    </div>
  </section>

  <!-- CONTACT -->
  <section id="contact">
    <div class="container">
      <div class="contact-inner">
        <div>
          <p class="section-label reveal">Contact</p>
          <h2 class="section-title reveal reveal-delay-1">Travaillons <em>ensemble.</em></h2>
          <p class="contact-desc reveal reveal-delay-2">À la recherche d'une alternance en master dans les domaines du marketing, du business development, du CRM ou de la stratégie commerciale.</p>
          <div class="contact-links reveal reveal-delay-3">
            <a href="mailto:paul.martin37700@gmail.com" class="contact-link">
              <div class="contact-link-icon"><svg width="17" height="17" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"/><polyline points="22,6 12,13 2,6"/></svg></div>
              <div><div class="contact-link-label">Email</div><div class="contact-link-value">paul.martin37700@gmail.com</div></div>
            </a>
            <a href="tel:+33689751117" class="contact-link">
              <div class="contact-link-icon"><svg width="17" height="17" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07A19.5 19.5 0 0 1 4.69 12a19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 3.6 1.17h3a2 2 0 0 1 2 1.72c.127.96.361 1.903.7 2.81a2 2 0 0 1-.45 2.11L7.91 8.69a16 16 0 0 0 6 6l.91-.91a2 2 0 0 1 2.11-.45c.907.339 1.85.573 2.81.7A2 2 0 0 1 22 16.92z"/></svg></div>
              <div><div class="contact-link-label">Téléphone</div><div class="contact-link-value">(+33) 6 89 75 11 17</div></div>
            </a>
            <a href="https://www.linkedin.com" target="_blank" class="contact-link">
              <div class="contact-link-icon"><svg width="17" height="17" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"/><rect x="2" y="9" width="4" height="12"/><circle cx="4" cy="4" r="2"/></svg></div>
              <div><div class="contact-link-label">LinkedIn</div><div class="contact-link-value">Paul Martin</div></div>
            </a>
          </div>
        </div>
        <div class="contact-form reveal reveal-delay-2">
          <div class="form-row">
            <div class="form-group"><label class="form-label">Prénom</label><input class="form-input" type="text" placeholder="Votre prénom" /></div>
            <div class="form-group"><label class="form-label">Nom</label><input class="form-input" type="text" placeholder="Votre nom" /></div>
          </div>
          <div class="form-group"><label class="form-label">Email</label><input class="form-input" type="email" placeholder="votre@email.com" /></div>
          <div class="form-group"><label class="form-label">Sujet</label><input class="form-input" type="text" placeholder="Opportunité de master, alternance..." /></div>
          <div class="form-group"><label class="form-label">Message</label><textarea class="form-textarea" placeholder="Décrivez votre projet ou opportunité..."></textarea></div>
          <button class="form-submit">Envoyer le message</button>
        </div>
      </div>
    </div>
  </section>

  <footer>
    <div class="footer-name">Paul Martin</div>
    <div class="footer-copy">© 2025 · BUT Techniques de Commercialisation · Issoudun</div>
  </footer>

  <script>
    const cursor = document.getElementById('cursor');
    const ring = document.getElementById('cursorRing');
    let mx=0,my=0,rx=0,ry=0;
    document.addEventListener('mousemove',e=>{mx=e.clientX;my=e.clientY;});
    function animateCursor(){
      cursor.style.left=mx+'px';cursor.style.top=my+'px';
      rx+=(mx-rx)*0.12;ry+=(my-ry)*0.12;
      ring.style.left=rx+'px';ring.style.top=ry+'px';
      requestAnimationFrame(animateCursor);
    }
    animateCursor();
    document.querySelectorAll('a,button').forEach(el=>{
      el.addEventListener('mouseenter',()=>{ring.style.width='52px';ring.style.height='52px';ring.style.borderColor='rgba(154,124,90,0.55)';});
      el.addEventListener('mouseleave',()=>{ring.style.width='32px';ring.style.height='32px';ring.style.borderColor='rgba(0,0,0,0.3)';});
    });
    const reveals=document.querySelectorAll('.reveal');
    const obs=new IntersectionObserver(entries=>{entries.forEach(e=>{if(e.isIntersecting)e.target.classList.add('visible');});},{threshold:0.1});
    reveals.forEach(el=>obs.observe(el));
    // Form feedback
    document.querySelector('.form-submit').addEventListener('click', function(e) {
      e.preventDefault();
      const btn = this;
      btn.textContent = 'Message envoyé ✓';
      btn.classList.add('sent');
      setTimeout(() => { btn.textContent = 'Envoyer le message'; btn.classList.remove('sent'); }, 3000);
    });
    window.addEventListener('scroll',()=>{
      document.querySelector('nav').style.borderBottomColor=window.scrollY>40?'rgba(0,0,0,0.09)':'rgba(0,0,0,0.06)';
    });
  </script>
</body>
</html>
