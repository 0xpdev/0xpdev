```aura width=860 height=200
<div style={{ width: '100%', height: '100%', background: '#08080c', display: 'flex', alignItems: 'center', fontFamily: 'Inter, sans-serif', position: 'relative', overflow: 'hidden', borderRadius: 16, border: '1px solid rgba(220,30,30,0.18)' }}>
  <style>{`
    @keyframes float-slow { 0%, 100% { transform: translateX(0px); opacity: 0.8; } 50% { transform: translateX(350px); opacity: 1.2; } }
    @keyframes float-medium { 0%, 100% { transform: translateX(0px); opacity: 0.7; } 50% { transform: translateX(-250px); opacity: 1.1; } }
    @keyframes float-fast { 0%, 100% { transform: translateX(0px); opacity: 0.9; } 50% { transform: translateX(200px); opacity: 0.6; } }
    @keyframes float-diagonal { 0%, 100% { transform: translateX(0px); opacity: 0.75; } 50% { transform: translateX(300px); opacity: 1.0; } }
    @keyframes float-wave { 0%, 100% { transform: translateX(0px); opacity: 0.65; } 33% { transform: translateX(-160px); opacity: 0.9; } 66% { transform: translateX(80px); opacity: 1.0; } }
    @keyframes float-pulse { 0%, 100% { transform: scale(1); opacity: 0.8; } 50% { transform: scale(1.3); opacity: 0.4; } }
    #glow-1 { animation: float-slow 8s ease-in-out infinite; }
    #glow-2 { animation: float-medium 12s ease-in-out infinite; }
    #glow-3 { animation: float-fast 9s ease-in-out infinite; }
    #glow-4 { animation: float-slow 11s ease-in-out infinite reverse; }
    #glow-5 { animation: float-medium 14s ease-in-out infinite reverse; }
    #glow-6 { animation: float-diagonal 10s ease-in-out infinite; }
    #glow-7 { animation: float-wave 13s ease-in-out infinite; }
    #glow-8 { animation: float-pulse 7s ease-in-out infinite; }
  `}</style>
  <svg width="860" height="200" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="g1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(200,20,20,0.72)" /><stop offset="40%" stopColor="rgba(160,10,10,0.35)" /><stop offset="70%" stopColor="rgba(160,10,10,0)" /></radialGradient>
      <radialGradient id="g2" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(220,40,40,0.6)" /><stop offset="45%" stopColor="rgba(180,20,20,0.25)" /><stop offset="70%" stopColor="rgba(180,20,20,0)" /></radialGradient>
      <radialGradient id="g3" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(180,0,0,0.45)" /><stop offset="50%" stopColor="rgba(140,0,0,0.18)" /><stop offset="70%" stopColor="rgba(140,0,0,0)" /></radialGradient>
      <radialGradient id="g4" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(255,40,40,0.32)" /><stop offset="70%" stopColor="rgba(255,40,40,0)" /></radialGradient>
      <radialGradient id="g5" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(150,10,10,0.38)" /><stop offset="70%" stopColor="rgba(150,10,10,0)" /></radialGradient>
      <radialGradient id="g6" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(230,20,20,0.55)" /><stop offset="45%" stopColor="rgba(190,10,10,0.22)" /><stop offset="70%" stopColor="rgba(190,10,10,0)" /></radialGradient>
      <radialGradient id="g7" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(200,30,30,0.42)" /><stop offset="50%" stopColor="rgba(160,10,10,0.16)" /><stop offset="70%" stopColor="rgba(160,10,10,0)" /></radialGradient>
      <radialGradient id="g8" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(255,20,20,0.40)" /><stop offset="50%" stopColor="rgba(200,10,10,0.15)" /><stop offset="70%" stopColor="rgba(200,10,10,0)" /></radialGradient>
    </defs>
    <ellipse id="glow-1" cx="180" cy="230" rx="260" ry="190" fill="url(#g1)" />
    <ellipse id="glow-2" cx="300" cy="240" rx="220" ry="160" fill="url(#g2)" />
    <ellipse id="glow-3" cx="420" cy="240" rx="180" ry="140" fill="url(#g3)" />
    <ellipse id="glow-4" cx="550" cy="250" rx="150" ry="120" fill="url(#g4)" />
    <ellipse id="glow-5" cx="750" cy="250" rx="130" ry="110" fill="url(#g5)" />
    <ellipse id="glow-6" cx="300" cy="240" rx="180" ry="140" fill="url(#g6)" />
    <ellipse id="glow-7" cx="490" cy="230" rx="220" ry="170" fill="url(#g7)" />
    <ellipse id="glow-8" cx="590" cy="250" rx="150" ry="130" fill="url(#g8)" />
  </svg>
  <div style={{ position: 'absolute', left: 48, top: 52, width: 96, height: 96, borderRadius: 48, background: 'linear-gradient(135deg, #ee2222, #880000)', display: 'flex', alignItems: 'center', justifyContent: 'center' }}>
    <img src={(github && github.user && github.user.avatar_url) || 'https://github.com/0xpdev.png'} width={88} height={88} style={{ borderRadius: 44 }} />
  </div>
  <div style={{ display: 'flex', flexDirection: 'column', marginLeft: 168, gap: 8, zIndex: 10 }}>
    <div style={{ fontSize: 38, fontWeight: 800, color: '#ffffff', letterSpacing: '-1px', lineHeight: 1 }}>Priyanshu Dev</div>
    <div style={{ fontSize: 15, color: 'rgba(255,180,180,0.8)', fontWeight: 400 }}>Full Stack Engineer · Gen AI · Machine Learning</div>
    <div style={{ display: 'flex', gap: 8, marginTop: 6, flexWrap: 'wrap' }}>
      {['JavaScript', 'Python', 'C++', 'Java', 'React', 'Next.js'].map(function(tag) {
        return <div key={tag} style={{ padding: '4px 12px', borderRadius: 20, background: 'rgba(220,30,30,0.18)', border: '1px solid rgba(220,50,50,0.32)', color: 'rgba(255,200,200,0.85)', fontSize: 12, fontWeight: 600 }}>{tag}</div>;
      })}
    </div>
  </div>
</div>
```

```aura width=860 height=100
<div style={{ display: 'flex', flexDirection: 'row', gap: 12, width: '100%', height: '100%', fontFamily: 'Inter, sans-serif' }}>
  <style>{`
    @keyframes s-float-slow { 0%, 100% { transform: translateX(0px); opacity: 0.7; } 50% { transform: translateX(120px); opacity: 1.0; } }
    @keyframes s-float-med { 0%, 100% { transform: translateX(0px); opacity: 0.6; } 50% { transform: translateX(-100px); opacity: 0.9; } }
    @keyframes stat-glow { 0%, 100% { box-shadow: 0 0 0px rgba(220,30,30,0); } 50% { box-shadow: 0 0 18px rgba(220,30,30,0.35); } }
    .stat-card { animation: stat-glow 4s ease-in-out infinite; }
    #s-orb1 { animation: s-float-slow 8s ease-in-out infinite; }
    #s-orb2 { animation: s-float-med 11s ease-in-out infinite; }
    #s-orb3 { animation: s-float-slow 9s ease-in-out infinite reverse; }
  `}</style>
  {[
    { label: 'REPOS', value: (github && github.user && github.user.public_repos) || '8', delay: '0s' },
    { label: 'STARS', value: (github && github.totalStars) || '4', color: '#f87171', delay: '1.3s' },
    { label: 'COMMITS', value: (github && github.totalCommits) || '100+', color: '#fca5a5', delay: '2.6s' },
  ].map((stat, i) => (
    <div key={i} className="stat-card" style={{ flex: 1, display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center', background: '#08080c', borderRadius: 14, border: '1px solid rgba(220,30,30,0.2)', position: 'relative', overflow: 'hidden' }}>
      <svg width="100%" height="100" style={{ position: 'absolute', top: 0, left: 0 }}>
        <defs>
          <radialGradient id={`sg${i}`} cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(200,20,20,0.35)" /><stop offset="70%" stopColor="rgba(200,20,20,0)" /></radialGradient>
        </defs>
        <ellipse cx="50%" cy="120" rx="120" ry="90" fill={`url(#sg${i})`} />
      </svg>
      <span style={{ fontSize: 28, fontWeight: 700, color: stat.color || '#e2e8f0', position: 'relative', zIndex: 1 }}>{stat.value}</span>
      <span style={{ fontSize: 10, color: 'rgba(255,180,180,0.45)', letterSpacing: 3, marginTop: 4, position: 'relative', zIndex: 1 }}>{stat.label}</span>
    </div>
  ))}
</div>
```

```aura width=860 height=160
<div style={{ position: 'relative', width: '100%', height: '100%', background: '#08080c', borderRadius: 14, overflow: 'hidden', fontFamily: 'Inter, sans-serif', border: '1px solid rgba(220,30,30,0.2)', display: 'flex', alignItems: 'center', padding: '0 28px', boxSizing: 'border-box' }}>
  <style>{`
    @keyframes t-float-slow { 0%, 100% { transform: translateX(0px); opacity: 0.8; } 50% { transform: translateX(300px); opacity: 1.1; } }
    @keyframes t-float-med { 0%, 100% { transform: translateX(0px); opacity: 0.7; } 50% { transform: translateX(-220px); opacity: 1.0; } }
    @keyframes t-float-fast { 0%, 100% { transform: translateX(0px); opacity: 0.6; } 50% { transform: translateX(180px); opacity: 0.9; } }
    @keyframes t-float-pulse { 0%, 100% { transform: scale(1); opacity: 0.7; } 50% { transform: scale(1.4); opacity: 0.3; } }
    #t-orb1 { animation: t-float-slow 9s ease-in-out infinite; }
    #t-orb2 { animation: t-float-med 12s ease-in-out infinite; }
    #t-orb3 { animation: t-float-fast 8s ease-in-out infinite reverse; }
    #t-orb4 { animation: t-float-pulse 7s ease-in-out infinite; }
  `}</style>
  <svg width="860" height="160" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="tg1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(200,20,20,0.5)" /><stop offset="40%" stopColor="rgba(160,10,10,0.2)" /><stop offset="70%" stopColor="rgba(160,10,10,0)" /></radialGradient>
      <radialGradient id="tg2" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(220,40,40,0.45)" /><stop offset="45%" stopColor="rgba(180,20,20,0.18)" /><stop offset="70%" stopColor="rgba(180,20,20,0)" /></radialGradient>
      <radialGradient id="tg3" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(180,0,0,0.4)" /><stop offset="50%" stopColor="rgba(140,0,0,0.15)" /><stop offset="70%" stopColor="rgba(140,0,0,0)" /></radialGradient>
      <radialGradient id="tg4" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(255,30,30,0.35)" /><stop offset="70%" stopColor="rgba(255,30,30,0)" /></radialGradient>
    </defs>
    <ellipse id="t-orb1" cx="100" cy="80" rx="200" ry="120" fill="url(#tg1)" />
    <ellipse id="t-orb2" cx="700" cy="80" rx="200" ry="120" fill="url(#tg2)" />
    <ellipse id="t-orb3" cx="430" cy="160" rx="180" ry="100" fill="url(#tg3)" />
    <ellipse id="t-orb4" cx="500" cy="20" rx="150" ry="90" fill="url(#tg4)" />
  </svg>
  <div style={{ display: 'flex', flexDirection: 'row', alignItems: 'center', gap: 24, zIndex: 10, width: '100%' }}>
    <div style={{ display: 'flex', flexDirection: 'column', gap: 8, flex: 1 }}>
      <span style={{ fontSize: 9, color: 'rgba(220,50,50,0.8)', letterSpacing: 3, textTransform: 'uppercase' }}>LANGUAGES</span>
      <div style={{ display: 'flex', gap: 6, flexWrap: 'wrap' }}>
        {['JavaScript', 'Python', 'C++', 'Java'].map((t, i) => (
          <span key={i} style={{ padding: '4px 14px', background: 'rgba(200,20,20,0.15)', color: 'rgba(255,200,200,0.9)', borderRadius: 100, fontSize: 12, border: '1px solid rgba(220,40,40,0.28)', fontWeight: 500 }}>{t}</span>
        ))}
      </div>
    </div>
    <div style={{ width: 1, height: 60, background: 'rgba(220,30,30,0.25)', flexShrink: 0 }} />
    <div style={{ display: 'flex', flexDirection: 'column', gap: 8, flex: 1 }}>
      <span style={{ fontSize: 9, color: 'rgba(220,50,50,0.8)', letterSpacing: 3, textTransform: 'uppercase' }}>FRAMEWORKS</span>
      <div style={{ display: 'flex', gap: 6, flexWrap: 'wrap' }}>
        {['React', 'Next.js', 'Node.js', 'Docker'].map((t, i) => (
          <span key={i} style={{ padding: '4px 14px', background: 'rgba(200,20,20,0.15)', color: 'rgba(255,200,200,0.9)', borderRadius: 100, fontSize: 12, border: '1px solid rgba(220,40,40,0.28)', fontWeight: 500 }}>{t}</span>
        ))}
      </div>
    </div>
    <div style={{ width: 1, height: 60, background: 'rgba(220,30,30,0.25)', flexShrink: 0 }} />
    <div style={{ display: 'flex', flexDirection: 'column', gap: 8, flex: 1 }}>
      <span style={{ fontSize: 9, color: 'rgba(220,50,50,0.8)', letterSpacing: 3, textTransform: 'uppercase' }}>FOCUS</span>
      <div style={{ display: 'flex', gap: 6, flexWrap: 'wrap' }}>
        {['DSA', 'System Design', 'Gen AI', 'ML'].map((t, i) => (
          <span key={i} style={{ padding: '4px 14px', background: 'rgba(200,20,20,0.15)', color: 'rgba(255,200,200,0.9)', borderRadius: 100, fontSize: 12, border: '1px solid rgba(220,40,40,0.28)', fontWeight: 500 }}>{t}</span>
        ))}
      </div>
    </div>
  </div>
</div>
```

```aura width=110 height=44 link="https://x.com/priyanshudevx" inline align=center
<SocialMediaButton
  icon="https://raw.githubusercontent.com/0xpdev/0xpdev/main/icons/X.png"
  text="X.com"
  backgroundColor="#08080c"
  width={110}
  height={44}
  gradientStops={[{ offset: '0%', color: '#cc2222' }, { offset: '30%', color: '#000000' }, { offset: '60%', color: '#cc2222' }, { offset: '80%', color: '#000000' }, { offset: '100%', color: '#aa1111' }]}
/>
```

```aura width=125 height=44 link="https://t.me/priyannnsh" inline align=center
<SocialMediaButton
  icon="https://raw.githubusercontent.com/0xpdev/0xpdev/main/icons/telegram.png"
  text="Telegram"
  backgroundColor="#08080c"
  width={125}
  height={44}
  gradientStops={[{ offset: '0%', color: '#cc2222' }, { offset: '30%', color: '#000000' }, { offset: '60%', color: '#cc2222' }, { offset: '80%', color: '#000000' }, { offset: '100%', color: '#aa1111' }]}
/>
```

```aura width=120 height=44 link="https://discord.com/users/priyanshu.dev." inline align=center
<SocialMediaButton
  icon="https://raw.githubusercontent.com/0xpdev/0xpdev/main/icons/discord.png"
  text="Discord"
  backgroundColor="#08080c"
  width={120}
  height={44}
  gradientStops={[{ offset: '0%', color: '#cc2222' }, { offset: '30%', color: '#000000' }, { offset: '60%', color: '#cc2222' }, { offset: '80%', color: '#000000' }, { offset: '100%', color: '#aa1111' }]}
/>
```

```aura width=105 height=44 link="mailto:priyanshudev037@gmail.com" inline align=center
<SocialMediaButton
  icon="https://raw.githubusercontent.com/0xpdev/0xpdev/main/icons/gmail.png"
  text="Email"
  backgroundColor="#08080c"
  width={105}
  height={44}
  gradientStops={[{ offset: '0%', color: '#cc2222' }, { offset: '30%', color: '#000000' }, { offset: '60%', color: '#cc2222' }, { offset: '80%', color: '#000000' }, { offset: '100%', color: '#aa1111' }]}
/>
```