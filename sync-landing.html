<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Sync — Estude. Conecte. Flua.</title>
<link href="https://fonts.googleapis.com/css2?family=Syne:wght@400;500;600;700;800&family=DM+Mono:ital,wght@0,300;0,400;1,300&family=DM+Sans:ital,opsz,wght@0,9..40,300;0,9..40,400;1,9..40,300&display=swap" rel="stylesheet">
<style>
  *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

  :root {
    --bg: #0a0a0f;
    --surface: #12121a;
    --surface2: #1a1a26;
    --border: rgba(255,255,255,0.07);
    --accent: #7c6fff;
    --accent2: #ff6f91;
    --accent3: #6fffd4;
    --text: #e8e8f0;
    --muted: #6b6b80;
    --font-display: 'Syne', sans-serif;
    --font-mono: 'DM Mono', monospace;
    --font-body: 'DM Sans', sans-serif;
  }

  html { scroll-behavior: smooth; }

  body {
    background: var(--bg);
    color: var(--text);
    font-family: var(--font-body);
    overflow-x: hidden;
    cursor: none;
  }

  /* Custom cursor */
  .cursor {
    position: fixed;
    width: 10px; height: 10px;
    background: var(--accent);
    border-radius: 50%;
    pointer-events: none;
    z-index: 9999;
    transform: translate(-50%, -50%);
    transition: transform 0.1s, background 0.2s;
    mix-blend-mode: screen;
  }
  .cursor-ring {
    position: fixed;
    width: 36px; height: 36px;
    border: 1px solid rgba(124,111,255,0.5);
    border-radius: 50%;
    pointer-events: none;
    z-index: 9998;
    transform: translate(-50%, -50%);
    transition: transform 0.18s ease, width 0.2s, height 0.2s, border-color 0.2s;
  }

  /* Noise overlay */
  body::before {
    content: '';
    position: fixed;
    inset: 0;
    background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)' opacity='0.04'/%3E%3C/svg%3E");
    pointer-events: none;
    z-index: 100;
    opacity: 0.4;
  }

  /* ---- NAV ---- */
  nav {
    position: fixed;
    top: 0; left: 0; right: 0;
    z-index: 50;
    padding: 20px 48px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    border-bottom: 1px solid transparent;
    transition: border-color 0.3s, backdrop-filter 0.3s;
  }
  nav.scrolled {
    border-bottom-color: var(--border);
    backdrop-filter: blur(20px);
    background: rgba(10,10,15,0.7);
  }
  .nav-logo {
    font-family: var(--font-display);
    font-size: 22px;
    font-weight: 800;
    letter-spacing: -0.5px;
    display: flex;
    align-items: center;
    gap: 8px;
  }
  .logo-dot {
    width: 8px; height: 8px;
    background: var(--accent);
    border-radius: 50%;
    display: inline-block;
    animation: pulse-dot 2s ease-in-out infinite;
  }
  @keyframes pulse-dot {
    0%,100% { box-shadow: 0 0 0 0 rgba(124,111,255,0.6); }
    50% { box-shadow: 0 0 0 8px rgba(124,111,255,0); }
  }
  .nav-links {
    display: flex;
    gap: 36px;
    list-style: none;
  }
  .nav-links a {
    font-family: var(--font-mono);
    font-size: 12px;
    color: var(--muted);
    text-decoration: none;
    letter-spacing: 0.05em;
    transition: color 0.2s;
  }
  .nav-links a:hover { color: var(--text); }
  .nav-cta {
    font-family: var(--font-mono);
    font-size: 12px;
    padding: 9px 20px;
    border: 1px solid var(--accent);
    color: var(--accent);
    background: transparent;
    border-radius: 4px;
    cursor: none;
    transition: background 0.2s, color 0.2s;
    letter-spacing: 0.05em;
  }
  .nav-cta:hover { background: var(--accent); color: #fff; }

  /* ---- HERO ---- */
  .hero {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding: 120px 48px 80px;
    position: relative;
    overflow: hidden;
  }

  /* Gradient orbs */
  .orb {
    position: absolute;
    border-radius: 50%;
    filter: blur(80px);
    pointer-events: none;
    opacity: 0.25;
  }
  .orb-1 {
    width: 600px; height: 600px;
    background: radial-gradient(circle, var(--accent), transparent 70%);
    top: -200px; left: -150px;
    animation: float1 12s ease-in-out infinite;
  }
  .orb-2 {
    width: 400px; height: 400px;
    background: radial-gradient(circle, var(--accent2), transparent 70%);
    bottom: -100px; right: -100px;
    animation: float2 15s ease-in-out infinite;
  }
  .orb-3 {
    width: 300px; height: 300px;
    background: radial-gradient(circle, var(--accent3), transparent 70%);
    top: 50%; right: 15%;
    animation: float3 10s ease-in-out infinite;
    opacity: 0.12;
  }
  @keyframes float1 { 0%,100% { transform: translate(0,0); } 50% { transform: translate(60px, 40px); } }
  @keyframes float2 { 0%,100% { transform: translate(0,0); } 50% { transform: translate(-40px, -60px); } }
  @keyframes float3 { 0%,100% { transform: translateY(0); } 50% { transform: translateY(-40px); } }

  /* Grid lines */
  .hero::after {
    content: '';
    position: absolute;
    inset: 0;
    background-image:
      linear-gradient(rgba(255,255,255,0.02) 1px, transparent 1px),
      linear-gradient(90deg, rgba(255,255,255,0.02) 1px, transparent 1px);
    background-size: 60px 60px;
    pointer-events: none;
  }

  .hero-badge {
    font-family: var(--font-mono);
    font-size: 11px;
    letter-spacing: 0.15em;
    color: var(--accent);
    border: 1px solid rgba(124,111,255,0.3);
    background: rgba(124,111,255,0.08);
    padding: 6px 16px;
    border-radius: 2px;
    margin-bottom: 32px;
    opacity: 0;
    animation: fadeUp 0.8s 0.2s forwards;
    position: relative; z-index: 1;
  }

  .hero-title {
    font-family: var(--font-display);
    font-size: clamp(56px, 8vw, 120px);
    font-weight: 800;
    line-height: 0.92;
    letter-spacing: -0.04em;
    margin-bottom: 32px;
    opacity: 0;
    animation: fadeUp 0.8s 0.4s forwards;
    position: relative; z-index: 1;
  }

  .hero-title .line-2 {
    display: block;
    background: linear-gradient(135deg, var(--accent) 0%, var(--accent2) 50%, var(--accent3) 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
  }

  .hero-sub {
    font-family: var(--font-body);
    font-size: clamp(16px, 2vw, 20px);
    font-weight: 300;
    color: var(--muted);
    max-width: 540px;
    line-height: 1.65;
    margin-bottom: 48px;
    opacity: 0;
    animation: fadeUp 0.8s 0.6s forwards;
    position: relative; z-index: 1;
  }

  .hero-actions {
    display: flex;
    gap: 16px;
    align-items: center;
    opacity: 0;
    animation: fadeUp 0.8s 0.8s forwards;
    position: relative; z-index: 1;
  }

  .btn-primary {
    font-family: var(--font-mono);
    font-size: 13px;
    padding: 14px 32px;
    background: var(--accent);
    color: #fff;
    border: none;
    border-radius: 4px;
    cursor: none;
    letter-spacing: 0.03em;
    transition: transform 0.2s, box-shadow 0.2s;
  }
  .btn-primary:hover {
    transform: translateY(-2px);
    box-shadow: 0 12px 40px rgba(124,111,255,0.4);
  }

  .btn-ghost {
    font-family: var(--font-mono);
    font-size: 13px;
    padding: 14px 32px;
    background: transparent;
    color: var(--muted);
    border: 1px solid var(--border);
    border-radius: 4px;
    cursor: none;
    letter-spacing: 0.03em;
    transition: color 0.2s, border-color 0.2s;
  }
  .btn-ghost:hover { color: var(--text); border-color: rgba(255,255,255,0.2); }

  /* Integration chips */
  .integrations {
    position: relative; z-index: 1;
    display: flex;
    gap: 12px;
    align-items: center;
    margin-top: 64px;
    opacity: 0;
    animation: fadeUp 0.8s 1s forwards;
    flex-wrap: wrap;
    justify-content: center;
  }
  .int-label {
    font-family: var(--font-mono);
    font-size: 10px;
    color: var(--muted);
    letter-spacing: 0.1em;
    margin-right: 4px;
  }
  .int-chip {
    font-family: var(--font-mono);
    font-size: 11px;
    padding: 5px 14px;
    border-radius: 2px;
    border: 1px solid var(--border);
    background: var(--surface);
    color: var(--muted);
    transition: border-color 0.2s, color 0.2s;
  }
  .int-chip:hover { border-color: var(--accent); color: var(--text); }
  .int-chip.discord:hover { border-color: #5865F2; color: #5865F2; }
  .int-chip.spotify:hover { border-color: #1DB954; color: #1DB954; }
  .int-chip.notion:hover { border-color: #e8e8e8; color: #e8e8e8; }
  .int-chip.youtube:hover { border-color: #FF0000; color: #FF0000; }

  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(24px); }
    to { opacity: 1; transform: translateY(0); }
  }

  /* ---- MOCKUP / APP PREVIEW ---- */
  .preview-section {
    padding: 80px 48px 120px;
    display: flex;
    justify-content: center;
  }

  .app-mockup {
    width: 100%;
    max-width: 960px;
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 16px;
    overflow: hidden;
    box-shadow: 0 60px 120px rgba(0,0,0,0.6), 0 0 0 1px rgba(255,255,255,0.04);
    opacity: 0;
    transform: translateY(40px);
    transition: opacity 0.8s, transform 0.8s;
  }
  .app-mockup.visible { opacity: 1; transform: translateY(0); }

  /* Titlebar */
  .titlebar {
    background: var(--surface2);
    padding: 12px 16px;
    display: flex;
    align-items: center;
    gap: 8px;
    border-bottom: 1px solid var(--border);
  }
  .tb-dot {
    width: 10px; height: 10px; border-radius: 50%;
  }
  .tb-dot:nth-child(1) { background: #ff5f57; }
  .tb-dot:nth-child(2) { background: #febc2e; }
  .tb-dot:nth-child(3) { background: #28c840; }
  .tb-url {
    flex: 1;
    text-align: center;
    font-family: var(--font-mono);
    font-size: 11px;
    color: var(--muted);
    margin-left: -36px;
  }

  /* App interior */
  .app-interior {
    display: grid;
    grid-template-columns: 56px 220px 1fr 260px;
    height: 500px;
  }

  /* Sidebar icons */
  .sidebar-icons {
    background: #0d0d14;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 16px 0;
    gap: 8px;
    border-right: 1px solid var(--border);
  }
  .si-avatar {
    width: 32px; height: 32px;
    background: linear-gradient(135deg, var(--accent), var(--accent2));
    border-radius: 8px;
    margin-bottom: 12px;
    display: flex; align-items: center; justify-content: center;
    font-family: var(--font-display);
    font-size: 13px;
    font-weight: 800;
    color: white;
  }
  .si-icon {
    width: 36px; height: 36px;
    border-radius: 8px;
    background: var(--surface2);
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 16px;
    cursor: none;
    transition: background 0.15s;
    border: 1px solid transparent;
  }
  .si-icon.active { background: rgba(124,111,255,0.2); border-color: rgba(124,111,255,0.4); }
  .si-icon:hover { background: var(--border); }

  /* Channel panel */
  .channel-panel {
    background: #0f0f18;
    border-right: 1px solid var(--border);
    display: flex;
    flex-direction: column;
    overflow: hidden;
  }
  .cp-header {
    padding: 16px;
    border-bottom: 1px solid var(--border);
    font-family: var(--font-display);
    font-size: 14px;
    font-weight: 700;
    letter-spacing: -0.02em;
    display: flex;
    align-items: center;
    gap: 8px;
  }
  .cp-status {
    width: 7px; height: 7px;
    background: var(--accent3);
    border-radius: 50%;
    animation: pulse-dot 2s infinite;
  }
  .cp-section-label {
    padding: 12px 16px 4px;
    font-family: var(--font-mono);
    font-size: 9px;
    color: var(--muted);
    letter-spacing: 0.12em;
    text-transform: uppercase;
  }
  .cp-channel {
    padding: 6px 14px;
    display: flex;
    align-items: center;
    gap: 8px;
    border-radius: 4px;
    margin: 1px 6px;
    cursor: none;
    transition: background 0.15s;
  }
  .cp-channel:hover { background: rgba(255,255,255,0.04); }
  .cp-channel.active { background: rgba(124,111,255,0.15); }
  .cp-channel-icon { font-size: 13px; width: 18px; text-align: center; }
  .cp-channel-name { font-family: var(--font-body); font-size: 13px; color: var(--muted); }
  .cp-channel.active .cp-channel-name { color: var(--text); }
  .cp-badge {
    margin-left: auto;
    font-family: var(--font-mono);
    font-size: 9px;
    background: var(--accent);
    color: white;
    padding: 1px 6px;
    border-radius: 10px;
  }

  /* Spotify bar at bottom of channel panel */
  .now-playing {
    margin-top: auto;
    border-top: 1px solid var(--border);
    padding: 10px 14px;
    display: flex;
    align-items: center;
    gap: 10px;
  }
  .np-art {
    width: 32px; height: 32px;
    background: linear-gradient(135deg, #1DB954 0%, #0a8a3a 100%);
    border-radius: 4px;
    display: flex; align-items: center; justify-content: center;
    font-size: 15px;
    flex-shrink: 0;
  }
  .np-info { flex: 1; overflow: hidden; }
  .np-track { font-family: var(--font-body); font-size: 11px; color: var(--text); white-space: nowrap; overflow: hidden; text-overflow: ellipsis; }
  .np-artist { font-family: var(--font-mono); font-size: 10px; color: var(--muted); }
  .np-controls { display: flex; gap: 6px; }
  .np-btn { font-size: 12px; cursor: none; }

  /* Main content area */
  .main-area {
    display: flex;
    flex-direction: column;
    overflow: hidden;
  }
  .main-header {
    padding: 14px 20px;
    border-bottom: 1px solid var(--border);
    display: flex;
    align-items: center;
    gap: 12px;
  }
  .mh-channel {
    font-family: var(--font-display);
    font-size: 15px;
    font-weight: 700;
    display: flex;
    align-items: center;
    gap: 6px;
  }
  .mh-divider {
    width: 1px; height: 16px;
    background: var(--border);
  }
  .mh-desc {
    font-family: var(--font-body);
    font-size: 12px;
    color: var(--muted);
  }
  .mh-actions {
    margin-left: auto;
    display: flex;
    gap: 10px;
  }
  .mh-btn {
    width: 28px; height: 28px;
    background: var(--surface2);
    border-radius: 6px;
    display: flex; align-items: center; justify-content: center;
    font-size: 13px;
    cursor: none;
    border: 1px solid var(--border);
  }

  /* Doc content */
  .doc-area {
    flex: 1;
    padding: 24px 28px;
    overflow-y: auto;
    scrollbar-width: thin;
    scrollbar-color: var(--border) transparent;
  }
  .doc-title-bar {
    display: flex;
    align-items: flex-start;
    gap: 14px;
    margin-bottom: 20px;
  }
  .doc-emoji { font-size: 28px; }
  .doc-title {
    font-family: var(--font-display);
    font-size: 20px;
    font-weight: 800;
    letter-spacing: -0.03em;
    margin-bottom: 4px;
  }
  .doc-meta {
    font-family: var(--font-mono);
    font-size: 10px;
    color: var(--muted);
    display: flex;
    gap: 10px;
  }
  .doc-meta span { display: flex; align-items: center; gap: 4px; }
  .doc-block {
    margin-bottom: 16px;
  }
  .doc-h2 {
    font-family: var(--font-display);
    font-size: 13px;
    font-weight: 700;
    letter-spacing: -0.01em;
    margin-bottom: 6px;
    color: var(--text);
  }
  .doc-p {
    font-family: var(--font-body);
    font-size: 12px;
    color: var(--muted);
    line-height: 1.7;
  }
  .doc-p strong { color: var(--text); font-weight: 500; }

  /* Callout */
  .doc-callout {
    background: rgba(124,111,255,0.08);
    border-left: 2px solid var(--accent);
    border-radius: 0 6px 6px 0;
    padding: 10px 14px;
    margin-bottom: 14px;
    font-family: var(--font-body);
    font-size: 12px;
    color: var(--muted);
  }
  .doc-callout b { color: var(--accent); }

  /* Checklist */
  .checklist { list-style: none; margin-bottom: 14px; }
  .checklist li {
    font-family: var(--font-body);
    font-size: 12px;
    color: var(--muted);
    padding: 3px 0;
    display: flex;
    align-items: center;
    gap: 8px;
  }
  .check-box {
    width: 14px; height: 14px;
    border: 1px solid var(--muted);
    border-radius: 3px;
    display: flex; align-items: center; justify-content: center;
    flex-shrink: 0;
    font-size: 9px;
  }
  .check-box.checked {
    background: var(--accent);
    border-color: var(--accent);
    color: white;
  }
  .checked-text { text-decoration: line-through; opacity: 0.5; }

  /* Typing cursors */
  .collab-cursors {
    position: relative;
    height: 2px;
    margin: -4px 0 14px;
  }
  .collab-cursor {
    position: absolute;
    width: 2px; height: 16px;
    border-radius: 1px;
    animation: blink 1s step-end infinite;
  }
  .collab-cursor::before {
    content: attr(data-name);
    position: absolute;
    top: -18px;
    left: 0;
    font-family: var(--font-mono);
    font-size: 9px;
    padding: 2px 5px;
    border-radius: 3px;
    white-space: nowrap;
    color: white;
    background: inherit;
  }
  @keyframes blink { 0%,100%{opacity:1} 50%{opacity:0} }

  /* Right panel */
  .right-panel {
    background: #0d0d16;
    border-left: 1px solid var(--border);
    display: flex;
    flex-direction: column;
    overflow: hidden;
  }
  .rp-tabs {
    display: flex;
    border-bottom: 1px solid var(--border);
  }
  .rp-tab {
    flex: 1;
    padding: 12px;
    font-family: var(--font-mono);
    font-size: 10px;
    text-align: center;
    color: var(--muted);
    cursor: none;
    letter-spacing: 0.08em;
    border-bottom: 2px solid transparent;
    transition: color 0.15s;
  }
  .rp-tab.active {
    color: var(--text);
    border-bottom-color: var(--accent);
  }
  .rp-content { padding: 14px; flex: 1; overflow-y: auto; }

  /* Focus timer */
  .focus-timer {
    background: var(--surface2);
    border: 1px solid var(--border);
    border-radius: 10px;
    padding: 16px;
    margin-bottom: 14px;
    text-align: center;
  }
  .ft-label {
    font-family: var(--font-mono);
    font-size: 10px;
    color: var(--muted);
    letter-spacing: 0.1em;
    margin-bottom: 8px;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 6px;
  }
  .ft-dot { width: 6px; height: 6px; background: var(--accent3); border-radius: 50%; }
  .ft-time {
    font-family: var(--font-display);
    font-size: 36px;
    font-weight: 800;
    letter-spacing: -0.04em;
    background: linear-gradient(90deg, var(--accent), var(--accent3));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    line-height: 1;
    margin-bottom: 10px;
  }
  .ft-ring {
    width: 80px; height: 80px;
    margin: 0 auto 10px;
    position: relative;
  }
  .ft-ring svg { transform: rotate(-90deg); }
  .ft-ring-bg { fill: none; stroke: var(--surface); stroke-width: 4; }
  .ft-ring-fill {
    fill: none;
    stroke: url(#timerGrad);
    stroke-width: 4;
    stroke-linecap: round;
    stroke-dasharray: 220;
    stroke-dashoffset: 60;
    animation: ring-progress 25s linear infinite;
  }
  @keyframes ring-progress { from { stroke-dashoffset: 220; } to { stroke-dashoffset: 0; } }
  .ft-time-inside {
    position: absolute;
    top: 50%; left: 50%;
    transform: translate(-50%, -50%);
    font-family: var(--font-display);
    font-size: 15px;
    font-weight: 800;
    letter-spacing: -0.04em;
  }
  .ft-controls {
    display: flex;
    gap: 8px;
    justify-content: center;
  }
  .ft-ctrl {
    padding: 5px 14px;
    border-radius: 4px;
    font-family: var(--font-mono);
    font-size: 10px;
    cursor: none;
    border: 1px solid var(--border);
    background: transparent;
    color: var(--muted);
    transition: all 0.15s;
  }
  .ft-ctrl.primary { background: var(--accent); border-color: var(--accent); color: white; }
  .ft-ctrl:hover { opacity: 0.8; }

  /* Online members */
  .members-section { margin-top: 2px; }
  .ms-label {
    font-family: var(--font-mono);
    font-size: 9px;
    color: var(--muted);
    letter-spacing: 0.12em;
    text-transform: uppercase;
    margin-bottom: 8px;
  }
  .member {
    display: flex;
    align-items: center;
    gap: 8px;
    padding: 5px 0;
  }
  .member-av {
    width: 26px; height: 26px;
    border-radius: 50%;
    display: flex; align-items: center; justify-content: center;
    font-size: 11px;
    font-weight: 700;
    font-family: var(--font-display);
    color: white;
    position: relative;
    flex-shrink: 0;
  }
  .member-av::after {
    content: '';
    position: absolute;
    bottom: -1px; right: -1px;
    width: 8px; height: 8px;
    border-radius: 50%;
    border: 1.5px solid #0d0d16;
  }
  .online::after { background: var(--accent3); }
  .focusing::after { background: var(--accent); }
  .idle::after { background: #febc2e; }
  .member-info { flex: 1; }
  .member-name {
    font-family: var(--font-body);
    font-size: 12px;
    color: var(--text);
    line-height: 1;
    margin-bottom: 2px;
  }
  .member-status {
    font-family: var(--font-mono);
    font-size: 9px;
    color: var(--muted);
  }

  /* XP bar */
  .xp-bar-section {
    margin-top: 12px;
    background: var(--surface2);
    border: 1px solid var(--border);
    border-radius: 8px;
    padding: 10px 12px;
  }
  .xp-header {
    display: flex;
    justify-content: space-between;
    margin-bottom: 6px;
  }
  .xp-label { font-family: var(--font-mono); font-size: 9px; color: var(--muted); letter-spacing: 0.08em; }
  .xp-value { font-family: var(--font-mono); font-size: 9px; color: var(--accent); }
  .xp-track {
    height: 4px;
    background: var(--surface);
    border-radius: 2px;
    overflow: hidden;
  }
  .xp-fill {
    height: 100%;
    background: linear-gradient(90deg, var(--accent), var(--accent3));
    border-radius: 2px;
    width: 68%;
    animation: xp-grow 2s 1.2s ease forwards;
    transform-origin: left;
  }
  @keyframes xp-grow { from { width: 0%; } to { width: 68%; } }

  /* ---- FEATURES ---- */
  .features-section {
    padding: 80px 48px 120px;
    max-width: 1100px;
    margin: 0 auto;
    width: 100%;
  }

  .section-eyebrow {
    font-family: var(--font-mono);
    font-size: 11px;
    color: var(--accent);
    letter-spacing: 0.15em;
    text-transform: uppercase;
    margin-bottom: 16px;
  }

  .section-title {
    font-family: var(--font-display);
    font-size: clamp(32px, 4vw, 52px);
    font-weight: 800;
    letter-spacing: -0.04em;
    line-height: 1.05;
    margin-bottom: 64px;
  }

  .features-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2px;
  }

  .feature-card {
    background: var(--surface);
    padding: 32px;
    border: 1px solid var(--border);
    position: relative;
    overflow: hidden;
    transition: border-color 0.25s;
    opacity: 0;
    transform: translateY(20px);
    transition: opacity 0.6s, transform 0.6s, border-color 0.25s;
  }
  .feature-card.visible { opacity: 1; transform: translateY(0); }
  .feature-card:hover { border-color: rgba(124,111,255,0.3); }
  .feature-card::before {
    content: '';
    position: absolute;
    top: 0; left: 0; right: 0;
    height: 1px;
    background: linear-gradient(90deg, transparent, var(--accent), transparent);
    opacity: 0;
    transition: opacity 0.25s;
  }
  .feature-card:hover::before { opacity: 1; }

  .feature-icon {
    font-size: 28px;
    margin-bottom: 20px;
    display: block;
  }

  .feature-title {
    font-family: var(--font-display);
    font-size: 18px;
    font-weight: 700;
    letter-spacing: -0.02em;
    margin-bottom: 10px;
  }

  .feature-desc {
    font-family: var(--font-body);
    font-size: 14px;
    color: var(--muted);
    line-height: 1.65;
  }

  .feature-tag {
    display: inline-block;
    margin-top: 16px;
    font-family: var(--font-mono);
    font-size: 10px;
    color: var(--accent);
    letter-spacing: 0.05em;
  }

  /* ---- HOW IT WORKS ---- */
  .how-section {
    padding: 0 48px 120px;
    max-width: 1100px;
    margin: 0 auto;
    width: 100%;
  }

  .steps {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 32px;
  }

  .step {
    position: relative;
    opacity: 0;
    transform: translateY(16px);
    transition: opacity 0.6s, transform 0.6s;
  }
  .step.visible { opacity: 1; transform: translateY(0); }

  .step-num {
    font-family: var(--font-display);
    font-size: 11px;
    font-weight: 700;
    color: var(--accent);
    letter-spacing: 0.1em;
    margin-bottom: 16px;
    font-variant-numeric: tabular-nums;
  }

  .step-title {
    font-family: var(--font-display);
    font-size: 17px;
    font-weight: 700;
    letter-spacing: -0.02em;
    margin-bottom: 8px;
  }

  .step-desc {
    font-family: var(--font-body);
    font-size: 13px;
    color: var(--muted);
    line-height: 1.65;
  }

  .step-connector {
    position: absolute;
    top: 6px;
    right: -16px;
    width: 32px;
    height: 1px;
    background: linear-gradient(90deg, var(--border), transparent);
  }

  /* ---- CTA ---- */
  .cta-section {
    padding: 80px 48px 140px;
    text-align: center;
    position: relative;
    overflow: hidden;
  }

  .cta-glow {
    position: absolute;
    top: 50%; left: 50%;
    transform: translate(-50%, -50%);
    width: 600px; height: 400px;
    background: radial-gradient(ellipse, rgba(124,111,255,0.12) 0%, transparent 70%);
    pointer-events: none;
  }

  .cta-title {
    font-family: var(--font-display);
    font-size: clamp(36px, 5vw, 72px);
    font-weight: 800;
    letter-spacing: -0.04em;
    line-height: 1.0;
    margin-bottom: 24px;
    position: relative; z-index: 1;
  }

  .cta-sub {
    font-family: var(--font-body);
    font-size: 18px;
    color: var(--muted);
    margin-bottom: 40px;
    position: relative; z-index: 1;
  }

  .cta-input-group {
    display: flex;
    gap: 0;
    max-width: 440px;
    margin: 0 auto;
    position: relative; z-index: 1;
  }

  .cta-input {
    flex: 1;
    padding: 14px 20px;
    background: var(--surface);
    border: 1px solid var(--border);
    border-right: none;
    border-radius: 4px 0 0 4px;
    color: var(--text);
    font-family: var(--font-body);
    font-size: 14px;
    outline: none;
    transition: border-color 0.2s;
  }
  .cta-input:focus { border-color: var(--accent); }
  .cta-input::placeholder { color: var(--muted); }

  .cta-btn {
    padding: 14px 28px;
    background: var(--accent);
    border: 1px solid var(--accent);
    border-radius: 0 4px 4px 0;
    color: white;
    font-family: var(--font-mono);
    font-size: 12px;
    letter-spacing: 0.05em;
    cursor: none;
    transition: opacity 0.2s;
  }
  .cta-btn:hover { opacity: 0.85; }

  /* ---- FOOTER ---- */
  footer {
    border-top: 1px solid var(--border);
    padding: 32px 48px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .footer-logo {
    font-family: var(--font-display);
    font-size: 16px;
    font-weight: 800;
    display: flex;
    align-items: center;
    gap: 8px;
  }

  .footer-copy {
    font-family: var(--font-mono);
    font-size: 11px;
    color: var(--muted);
  }

  .footer-links {
    display: flex;
    gap: 24px;
    list-style: none;
  }

  .footer-links a {
    font-family: var(--font-mono);
    font-size: 11px;
    color: var(--muted);
    text-decoration: none;
    transition: color 0.2s;
  }
  .footer-links a:hover { color: var(--text); }

  /* Responsive */
  @media (max-width: 900px) {
    nav { padding: 16px 24px; }
    .nav-links { display: none; }
    .hero { padding: 100px 24px 60px; }
    .features-grid { grid-template-columns: 1fr; }
    .steps { grid-template-columns: 1fr 1fr; }
    .app-interior { grid-template-columns: 48px 1fr; }
    .channel-panel, .right-panel { display: none; }
    footer { flex-direction: column; gap: 16px; text-align: center; }
    .preview-section { padding: 40px 24px 60px; }
    .features-section, .how-section { padding: 40px 24px 80px; }
  }
</style>
</head>
<body>

<div class="cursor" id="cursor"></div>
<div class="cursor-ring" id="cursorRing"></div>

<nav id="nav">
  <div class="nav-logo">
    <span class="logo-dot"></span>
    Sync
  </div>
  <ul class="nav-links">
    <li><a href="#">produto</a></li>
    <li><a href="#">funcionalidades</a></li>
    <li><a href="#">comunidade</a></li>
    <li><a href="#">preços</a></li>
  </ul>
  <button class="nav-cta">acesso antecipado</button>
</nav>

<!-- HERO -->
<section class="hero">
  <div class="orb orb-1"></div>
  <div class="orb orb-2"></div>
  <div class="orb orb-3"></div>

  <div class="hero-badge">▸ em desenvolvimento</div>
  <h1 class="hero-title">
    Estude junto.<br>
    <span class="line-2">Flua em sincronia.</span>
  </h1>
  <p class="hero-sub">
    Sync é o espaço onde conhecimento encontra comunidade. Estude sozinho ou colabore em tempo real — tudo conectado com as ferramentas que você já usa.
  </p>
  <div class="hero-actions">
    <button class="btn-primary">Entrar na lista de espera</button>
    <button class="btn-ghost">Ver demo →</button>
  </div>
  <div class="integrations">
    <span class="int-label">INTEGRA COM</span>
    <span class="int-chip discord">Discord</span>
    <span class="int-chip spotify">Spotify</span>
    <span class="int-chip notion">Notion</span>
    <span class="int-chip youtube">YouTube</span>
    <span class="int-chip">Google Drive</span>
    <span class="int-chip">Anki</span>
  </div>
</section>

<!-- APP MOCKUP -->
<section class="preview-section">
  <div class="app-mockup" id="mockup">
    <div class="titlebar">
      <div class="tb-dot"></div>
      <div class="tb-dot"></div>
      <div class="tb-dot"></div>
      <div class="tb-url">sync.app / sala / calculo-i</div>
    </div>
    <div class="app-interior">

      <!-- Sidebar icons -->
      <div class="sidebar-icons">
        <div class="si-avatar">E</div>
        <div class="si-icon active">📚</div>
        <div class="si-icon">🔊</div>
        <div class="si-icon">🤝</div>
        <div class="si-icon">📊</div>
        <div class="si-icon">⚙️</div>
      </div>

      <!-- Channel panel -->
      <div class="channel-panel">
        <div class="cp-header">
          <span class="cp-status"></span>
          Cálculo I
        </div>
        <div class="cp-section-label">salas de estudo</div>
        <div class="cp-channel active">
          <span class="cp-channel-icon">📝</span>
          <span class="cp-channel-name">anotações</span>
        </div>
        <div class="cp-channel">
          <span class="cp-channel-icon">❓</span>
          <span class="cp-channel-name">dúvidas</span>
          <span class="cp-badge">3</span>
        </div>
        <div class="cp-channel">
          <span class="cp-channel-icon">🎯</span>
          <span class="cp-channel-name">exercícios</span>
        </div>
        <div class="cp-channel">
          <span class="cp-channel-icon">🧪</span>
          <span class="cp-channel-name">simulados</span>
        </div>
        <div class="cp-section-label">recursos</div>
        <div class="cp-channel">
          <span class="cp-channel-icon">🔗</span>
          <span class="cp-channel-name">links salvos</span>
        </div>
        <div class="cp-channel">
          <span class="cp-channel-icon">📎</span>
          <span class="cp-channel-name">arquivos</span>
        </div>

        <div class="now-playing">
          <div class="np-art">♪</div>
          <div class="np-info">
            <div class="np-track">lo-fi beats to study</div>
            <div class="np-artist">Chillhop Music</div>
          </div>
          <div class="np-controls">
            <span class="np-btn">⏮</span>
            <span class="np-btn">⏸</span>
            <span class="np-btn">⏭</span>
          </div>
        </div>
      </div>

      <!-- Main doc area -->
      <div class="main-area">
        <div class="main-header">
          <div class="mh-channel">📝 anotações</div>
          <div class="mh-divider"></div>
          <div class="mh-desc">Colaborando com 4 pessoas</div>
          <div class="mh-actions">
            <div class="mh-btn">👥</div>
            <div class="mh-btn">🔍</div>
            <div class="mh-btn">⋯</div>
          </div>
        </div>
        <div class="doc-area">
          <div class="doc-title-bar">
            <span class="doc-emoji">📐</span>
            <div>
              <div class="doc-title">Limites e Continuidade</div>
              <div class="doc-meta">
                <span>✏️ editando</span>
                <span>👀 4 visualizando</span>
                <span>🕐 atualizado há 2min</span>
              </div>
            </div>
          </div>

          <div class="doc-callout">
            <b>💡 Lembrete:</b> Prova na sexta-feira, 14h. Foco nos exercícios de epsilon-delta!
          </div>

          <div class="doc-block">
            <div class="doc-h2">Definição Formal de Limite</div>
            <p class="doc-p">Dizemos que <strong>lim(x→a) f(x) = L</strong> se para todo ε > 0, existe δ > 0 tal que: se 0 &lt; |x − a| &lt; δ, então |f(x) − L| &lt; ε.</p>
          </div>

          <div class="collab-cursors">
            <div class="collab-cursor" data-name="Marina" style="left:40px; background:#ff6f91; height:14px;"></div>
            <div class="collab-cursor" data-name="João" style="left:160px; background:#6fffd4; animation-delay:0.5s; height:14px;"></div>
          </div>

          <div class="doc-block">
            <div class="doc-h2">Checklist — o que revisar</div>
            <ul class="checklist">
              <li><div class="check-box checked">✓</div><span class="checked-text">Limite lateral esquerdo e direito</span></li>
              <li><div class="check-box checked">✓</div><span class="checked-text">Limites no infinito</span></li>
              <li><div class="check-box">·</div><span>Definição epsilon-delta</span></li>
              <li><div class="check-box">·</div><span>Continuidade em um ponto</span></li>
              <li><div class="check-box">·</div><span>Teorema do Valor Intermediário</span></li>
            </ul>
          </div>

          <div class="doc-block">
            <div class="doc-h2">Exercícios pendentes</div>
            <p class="doc-p">Lista 3 — questões <strong>7, 8 e 11</strong> ainda sem resolução colaborativa. Alguém quer tentar juntos na sala de voz?</p>
          </div>
        </div>
      </div>

      <!-- Right panel -->
      <div class="right-panel">
        <div class="rp-tabs">
          <div class="rp-tab active">FOCO</div>
          <div class="rp-tab">MEMBROS</div>
          <div class="rp-tab">XP</div>
        </div>
        <div class="rp-content">

          <div class="focus-timer">
            <div class="ft-label">
              <div class="ft-dot"></div>
              POMODORO ATIVO
            </div>
            <div class="ft-ring">
              <svg width="80" height="80" viewBox="0 0 80 80">
                <defs>
                  <linearGradient id="timerGrad" x1="0%" y1="0%" x2="100%" y2="0%">
                    <stop offset="0%" style="stop-color:#7c6fff"/>
                    <stop offset="100%" style="stop-color:#6fffd4"/>
                  </linearGradient>
                </defs>
                <circle class="ft-ring-bg" cx="40" cy="40" r="35"/>
                <circle class="ft-ring-fill" cx="40" cy="40" r="35"/>
              </svg>
              <div class="ft-time-inside">18:42</div>
            </div>
            <div class="ft-controls">
              <button class="ft-ctrl primary">⏸ Pausar</button>
              <button class="ft-ctrl">↺ Reset</button>
            </div>
          </div>

          <div class="members-section">
            <div class="ms-label">ONLINE AGORA — 4</div>
            <div class="member">
              <div class="member-av online" style="background: linear-gradient(135deg,#7c6fff,#b09fff)">E</div>
              <div class="member-info">
                <div class="member-name">Você</div>
                <div class="member-status">🎯 em foco</div>
              </div>
            </div>
            <div class="member">
              <div class="member-av focusing" style="background: linear-gradient(135deg,#ff6f91,#ffaa6f)">M</div>
              <div class="member-info">
                <div class="member-name">Marina</div>
                <div class="member-status">✏️ editando doc</div>
              </div>
            </div>
            <div class="member">
              <div class="member-av online" style="background: linear-gradient(135deg,#6fffd4,#6fb3ff)">J</div>
              <div class="member-info">
                <div class="member-name">João</div>
                <div class="member-status">👀 lendo</div>
              </div>
            </div>
            <div class="member">
              <div class="member-av idle" style="background: linear-gradient(135deg,#febc2e,#fe8a2e)">A</div>
              <div class="member-info">
                <div class="member-name">Ana</div>
                <div class="member-status">⏸ pausa</div>
              </div>
            </div>
          </div>

          <div class="xp-bar-section">
            <div class="xp-header">
              <div class="xp-label">⚡ PROGRESSO — NÍVEL 7</div>
              <div class="xp-value">680 / 1000 XP</div>
            </div>
            <div class="xp-track">
              <div class="xp-fill"></div>
            </div>
          </div>

        </div>
      </div>

    </div>
  </div>
</section>

<!-- FEATURES -->
<section class="features-section">
  <div class="section-eyebrow">funcionalidades</div>
  <h2 class="section-title">Tudo que você precisa,<br>num só lugar.</h2>
  <div class="features-grid" id="featuresGrid">
    <div class="feature-card">
      <span class="feature-icon">📝</span>
      <div class="feature-title">Docs colaborativos</div>
      <p class="feature-desc">Notas em tempo real com múltiplos cursores, comentários e histórico de versões. Conecta direto com seu Notion.</p>
      <span class="feature-tag">↗ INTEGRA COM NOTION</span>
    </div>
    <div class="feature-card">
      <span class="feature-icon">🎵</span>
      <div class="feature-title">Trilha sonora da sessão</div>
      <p class="feature-desc">Todos da sala ouvem a mesma playlist sincronizada. Conecta ao Spotify ou usa as playlists curadas da comunidade.</p>
      <span class="feature-tag">↗ INTEGRA COM SPOTIFY</span>
    </div>
    <div class="feature-card">
      <span class="feature-icon">🔊</span>
      <div class="feature-title">Salas de voz</div>
      <p class="feature-desc">Chame amigos pra resolver um exercício difícil. Salas temáticas com canais de texto paralelos, como no Discord.</p>
      <span class="feature-tag">↗ INTEGRA COM DISCORD</span>
    </div>
    <div class="feature-card">
      <span class="feature-icon">⏱️</span>
      <div class="feature-title">Foco compartilhado</div>
      <p class="feature-desc">Pomodoro sincronizado pra toda a sala. Veja quem está em foco, em pausa ou estudando em modo solo.</p>
      <span class="feature-tag">→ PRODUTIVIDADE</span>
    </div>
    <div class="feature-card">
      <span class="feature-icon">🗺️</span>
      <div class="feature-title">Mapa de progresso</div>
      <p class="feature-desc">Visualize sua jornada de aprendizado. XP, conquistas e streaks que tornam o estudo genuinamente motivador.</p>
      <span class="feature-tag">→ GAMIFICAÇÃO</span>
    </div>
    <div class="feature-card">
      <span class="feature-icon">🤖</span>
      <div class="feature-title">IA de contexto</div>
      <p class="feature-desc">Uma IA que conhece suas notas, o conteúdo da sala e seu histórico — pra tirar dúvidas com contexto real.</p>
      <span class="feature-tag">→ AI-POWERED</span>
    </div>
  </div>
</section>

<!-- HOW IT WORKS -->
<section class="how-section">
  <div class="section-eyebrow">como funciona</div>
  <h2 class="section-title">Simples de começar.</h2>
  <div class="steps" id="steps">
    <div class="step">
      <div class="step-num">01 —</div>
      <div class="step-title">Crie uma sala</div>
      <p class="step-desc">Configure sua sala de estudo com matéria, objetivo e quem pode entrar.</p>
      <div class="step-connector"></div>
    </div>
    <div class="step">
      <div class="step-num">02 —</div>
      <div class="step-title">Conecte seus apps</div>
      <p class="step-desc">Autorize Spotify, Notion, Discord em segundos. O Sync cuida do resto.</p>
      <div class="step-connector"></div>
    </div>
    <div class="step">
      <div class="step-num">03 —</div>
      <div class="step-title">Chame sua galera</div>
      <p class="step-desc">Compartilhe o link. Qualquer um entra — com conta ou sem.</p>
      <div class="step-connector"></div>
    </div>
    <div class="step">
      <div class="step-num">04 —</div>
      <div class="step-title">Estude em sincronia</div>
      <p class="step-desc">Notas, música, foco e conversa — tudo acontecendo junto, em tempo real.</p>
    </div>
  </div>
</section>

<!-- CTA -->
<section class="cta-section">
  <div class="cta-glow"></div>
  <h2 class="cta-title">Pronto pra<br>estudar diferente?</h2>
  <p class="cta-sub">Entre na lista de espera e ganhe acesso antecipado.</p>
  <div class="cta-input-group">
    <input type="email" class="cta-input" placeholder="seu@email.com" />
    <button class="cta-btn">ENTRAR →</button>
  </div>
</section>

<!-- FOOTER -->
<footer>
  <div class="footer-logo">
    <span class="logo-dot"></span>
    Sync
  </div>
  <div class="footer-copy">© 2025 Sync · Feito com 🧠 e ♥</div>
  <ul class="footer-links">
    <li><a href="#">twitter</a></li>
    <li><a href="#">discord</a></li>
    <li><a href="#">github</a></li>
    <li><a href="#">privacidade</a></li>
  </ul>
</footer>

<script>
  // Cursor
  const cursor = document.getElementById('cursor');
  const ring = document.getElementById('cursorRing');
  let mx = 0, my = 0, rx = 0, ry = 0;
  document.addEventListener('mousemove', e => { mx = e.clientX; my = e.clientY; });
  function animCursor() {
    cursor.style.left = mx + 'px';
    cursor.style.top = my + 'px';
    rx += (mx - rx) * 0.12;
    ry += (my - ry) * 0.12;
    ring.style.left = rx + 'px';
    ring.style.top = ry + 'px';
    requestAnimationFrame(animCursor);
  }
  animCursor();

  document.querySelectorAll('button, a, .si-icon, .cp-channel, .rp-tab, .mh-btn, .ft-ctrl').forEach(el => {
    el.addEventListener('mouseenter', () => {
      cursor.style.transform = 'translate(-50%,-50%) scale(2)';
      ring.style.width = '50px'; ring.style.height = '50px';
      ring.style.borderColor = 'rgba(124,111,255,0.8)';
    });
    el.addEventListener('mouseleave', () => {
      cursor.style.transform = 'translate(-50%,-50%) scale(1)';
      ring.style.width = '36px'; ring.style.height = '36px';
      ring.style.borderColor = 'rgba(124,111,255,0.5)';
    });
  });

  // Nav scroll
  const nav = document.getElementById('nav');
  window.addEventListener('scroll', () => {
    nav.classList.toggle('scrolled', window.scrollY > 30);
  });

  // Intersection observer
  const obs = new IntersectionObserver(entries => {
    entries.forEach(e => { if (e.isIntersecting) e.target.classList.add('visible'); });
  }, { threshold: 0.15 });

  document.getElementById('mockup').style.transition = 'opacity 0.9s, transform 0.9s';
  obs.observe(document.getElementById('mockup'));

  document.querySelectorAll('.feature-card').forEach((card, i) => {
    card.style.transitionDelay = (i * 0.08) + 's';
    obs.observe(card);
  });

  document.querySelectorAll('.step').forEach((step, i) => {
    step.style.transitionDelay = (i * 0.1) + 's';
    obs.observe(step);
  });

  // Tab switching on mockup
  document.querySelectorAll('.rp-tab').forEach(tab => {
    tab.addEventListener('click', () => {
      document.querySelectorAll('.rp-tab').forEach(t => t.classList.remove('active'));
      tab.classList.add('active');
    });
  });

  // Channel switching
  document.querySelectorAll('.cp-channel').forEach(ch => {
    ch.addEventListener('click', () => {
      document.querySelectorAll('.cp-channel').forEach(c => c.classList.remove('active'));
      ch.classList.add('active');
    });
  });

  // CTA enter key
  document.querySelector('.cta-input').addEventListener('keydown', e => {
    if (e.key === 'Enter') {
      document.querySelector('.cta-btn').style.background = '#6fffd4';
      document.querySelector('.cta-btn').textContent = '✓ NA LISTA!';
    }
  });
</script>
</body>
</html>
