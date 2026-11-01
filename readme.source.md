<div style={{ width: '100%', height: '100%', background: '#07050f', display: 'flex', alignItems: 'center', fontFamily: 'Inter, sans-serif', position: 'relative', overflow: 'hidden', borderRadius: 16, border: '1px solid rgba(139,92,246,0.25)' }}>
  <style>{`
    @keyframes float-slow { 0%, 100% { transform: translateX(0px); opacity: 0.8; } 50% { transform: translateX(350px); opacity: 1.1; } }
    @keyframes float-medium { 0%, 100% { transform: translateX(0px); opacity: 0.7; } 50% { transform: translateX(-250px); opacity: 1.0; } }
    @keyframes float-fast { 0%, 100% { transform: translateX(0px); opacity: 0.9; } 50% { transform: translateX(200px); opacity: 0.5; } }
    @keyframes float-wave { 0%, 100% { transform: translateX(0px); opacity: 0.6; } 33% { transform: translateX(-160px); opacity: 0.9; } 66% { transform: translateX(80px); opacity: 1.0; } }
    @keyframes float-pulse { 0%, 100% { transform: scale(1); opacity: 0.8; } 50% { transform: scale(1.4); opacity: 0.3; } }
    #glow-1 { animation: float-slow 8s ease-in-out infinite; }
    #glow-2 { animation: float-medium 12s ease-in-out infinite; }
    #glow-3 { animation: float-fast 9s ease-in-out infinite; }
    #glow-4 { animation: float-slow 11s ease-in-out infinite reverse; }
    #glow-5 { animation: float-medium 14s ease-in-out infinite reverse; }
    #glow-6 { animation: float-wave 13s ease-in-out infinite; }
    #glow-7 { animation: float-pulse 7s ease-in-out infinite; }
    #glow-8 { animation: float-slow 10s ease-in-out infinite 2s; }
  `}</style>
  <svg width="860" height="200" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <filter id="grain"><feTurbulence type="fractalNoise" baseFrequency="0.65" numOctaves="3" stitchTiles="stitch"/><feColorMatrix type="saturate" values="0"/><feBlend in="SourceGraphic" mode="overlay" result="blend"/><feComposite in="blend" in2="SourceGraphic" operator="in"/></filter>
      <radialGradient id="g1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(139,92,246,0.75)" /><stop offset="40%" stopColor="rgba(109,40,217,0.35)" /><stop offset="70%" stopColor="rgba(109,40,217,0)" /></radialGradient>
      <radialGradient id="g2" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(59,130,246,0.65)" /><stop offset="45%" stopColor="rgba(37,99,235,0.28)" /><stop offset="70%" stopColor="rgba(37,99,235,0)" /></radialGradient>
      <radialGradient id="g3" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(167,139,250,0.55)" /><stop offset="50%" stopColor="rgba(139,92,246,0.22)" /><stop offset="70%" stopColor="rgba(139,92,246,0)" /></radialGradient>
      <radialGradient id="g4" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(99,102,241,0.45)" /><stop offset="70%" stopColor="rgba(99,102,241,0)" /></radialGradient>
      <radialGradient id="g5" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(79,70,229,0.40)" /><stop offset="70%" stopColor="rgba(79,70,229,0)" /></radialGradient>
      <radialGradient id="g6" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(147,51,234,0.55)" /><stop offset="45%" stopColor="rgba(126,34,206,0.22)" /><stop offset="70%" stopColor="rgba(126,34,206,0)" /></radialGradient>
      <radialGradient id="g7" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(37,99,235,0.45)" /><stop offset="50%" stopColor="rgba(29,78,216,0.18)" /><stop offset="70%" stopColor="rgba(29,78,216,0)" /></radialGradient>
      <radialGradient id="g8" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(196,181,253,0.30)" /><stop offset="70%" stopColor="rgba(196,181,253,0)" /></radialGradient>
    </defs>
    <ellipse id="glow-1" cx="180" cy="230" rx="260" ry="190" fill="url(#g1)" />
    <ellipse id="glow-2" cx="300" cy="240" rx="220" ry="160" fill="url(#g2)" />
    <ellipse id="glow-3" cx="420" cy="240" rx="180" ry="140" fill="url(#g3)" />
    <ellipse id="glow-4" cx="550" cy="250" rx="150" ry="120" fill="url(#g4)" />
    <ellipse id="glow-5" cx="750" cy="250" rx="130" ry="110" fill="url(#g5)" />
    <ellipse id="glow-6" cx="300" cy="240" rx="180" ry="140" fill="url(#g6)" />
    <ellipse id="glow-7" cx="490" cy="230" rx="220" ry="170" fill="url(#g7)" />
    <ellipse id="glow-8" cx="650" cy="100" rx="160" ry="130" fill="url(#g8)" />
    <rect width="860" height="200" fill="transparent" filter="url(#grain)" opacity="0.18" />
  </svg>
  <div style={{ position: 'absolute', left: 48, top: 52, width: 96, height: 96, borderRadius: 48, background: 'linear-gradient(135deg, #8b5cf6, #3b82f6)', display: 'flex', alignItems: 'center', justifyContent: 'center' }}>
    <img src={(github && github.user && github.user.avatar_url) || 'https://github.com/0xpdev.png'} width={88} height={88} style={{ borderRadius: 44 }} />
  </div>
  <div style={{ display: 'flex', flexDirection: 'column', marginLeft: 168, gap: 8, zIndex: 10 }}>
    <div style={{ fontSize: 38, fontWeight: 800, color: '#ffffff', letterSpacing: '-1px', lineHeight: 1 }}>Priyanshu Dev</div>
    <div style={{ fontSize: 15, color: 'rgba(196,181,253,0.8)', fontWeight: 400 }}> Developer // AI // Devops</div>

  </div>
</div>
