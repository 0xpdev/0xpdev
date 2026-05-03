```aura width=860 height=200
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
    <div style={{ fontSize: 15, color: 'rgba(196,181,253,0.8)', fontWeight: 400 }}>Full Stack Engineer · Gen AI · Machine Learning</div>
    <div style={{ display: 'flex', gap: 8, marginTop: 6, flexWrap: 'wrap' }}>
      {['JavaScript', 'Python', 'C++', 'Java', 'React', 'Next.js'].map(function(tag) {
        return <div key={tag} style={{ padding: '4px 12px', borderRadius: 20, background: 'rgba(139,92,246,0.15)', border: '1px solid rgba(139,92,246,0.35)', color: 'rgba(221,214,254,0.9)', fontSize: 12, fontWeight: 600 }}>{tag}</div>;
      })}
    </div>
  </div>
</div>
```

```aura width=860 height=100
<div style={{ display: 'flex', flexDirection: 'row', gap: 12, width: '100%', height: '100%', fontFamily: 'Inter, sans-serif' }}>
  <style>{`
    @keyframes stat-glow { 0%, 100% { box-shadow: 0 0 0px rgba(139,92,246,0); } 50% { box-shadow: 0 0 20px rgba(139,92,246,0.4); } }
    .stat-card { animation: stat-glow 4s ease-in-out infinite; }
  `}</style>
  {[
    { label: 'REPOS', value: (github && github.user && github.user.public_repos) || '8' },
    { label: 'STARS', value: (github && github.totalStars) || '4', color: '#c4b5fd' },
    { label: 'COMMITS', value: (github && github.totalCommits) || '100+', color: '#93c5fd' },
  ].map((stat, i) => (
    <div key={i} className="stat-card" style={{ flex: 1, display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center', background: '#07050f', borderRadius: 14, border: '1px solid rgba(139,92,246,0.2)', position: 'relative', overflow: 'hidden' }}>
      <svg width="100%" height="100" style={{ position: 'absolute', top: 0, left: 0 }}>
        <defs><radialGradient id={`sg${i}`} cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(139,92,246,0.3)" /><stop offset="70%" stopColor="rgba(139,92,246,0)" /></radialGradient></defs>
        <ellipse cx="50%" cy="120" rx="120" ry="90" fill={`url(#sg${i})`} />
      </svg>
      <span style={{ fontSize: 28, fontWeight: 700, color: stat.color || '#ffffff', position: 'relative', zIndex: 1 }}>{stat.value}</span>
      <span style={{ fontSize: 10, color: 'rgba(196,181,253,0.4)', letterSpacing: 3, marginTop: 4, position: 'relative', zIndex: 1 }}>{stat.label}</span>
    </div>
  ))}
</div>
```

```aura width=860 height=160
<div style={{ position: 'relative', width: '100%', height: '100%', background: '#07050f', borderRadius: 14, overflow: 'hidden', fontFamily: 'Inter, sans-serif', border: '1px solid rgba(139,92,246,0.2)', display: 'flex', alignItems: 'center', padding: '0 28px', boxSizing: 'border-box' }}>
  <style>{`
    @keyframes t-float-slow { 0%, 100% { transform: translateX(0px); opacity: 0.7; } 50% { transform: translateX(300px); opacity: 1.0; } }
    @keyframes t-float-med { 0%, 100% { transform: translateX(0px); opacity: 0.6; } 50% { transform: translateX(-220px); opacity: 0.9; } }
    @keyframes t-float-fast { 0%, 100% { transform: translateX(0px); opacity: 0.5; } 50% { transform: translateX(180px); opacity: 0.8; } }
    #t-orb1 { animation: t-float-slow 9s ease-in-out infinite; }
    #t-orb2 { animation: t-float-med 12s ease-in-out infinite; }
    #t-orb3 { animation: t-float-fast 8s ease-in-out infinite reverse; }
  `}</style>
  <svg width="860" height="160" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <filter id="tgrain"><feTurbulence type="fractalNoise" baseFrequency="0.65" numOctaves="3" stitchTiles="stitch"/><feColorMatrix type="saturate" values="0"/><feBlend in="SourceGraphic" mode="overlay" result="blend"/><feComposite in="blend" in2="SourceGraphic" operator="in"/></filter>
      <radialGradient id="tg1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(139,92,246,0.45)" /><stop offset="70%" stopColor="rgba(139,92,246,0)" /></radialGradient>
      <radialGradient id="tg2" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(59,130,246,0.35)" /><stop offset="70%" stopColor="rgba(59,130,246,0)" /></radialGradient>
      <radialGradient id="tg3" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(147,51,234,0.3)" /><stop offset="70%" stopColor="rgba(147,51,234,0)" /></radialGradient>
    </defs>
    <ellipse id="t-orb1" cx="100" cy="80" rx="200" ry="120" fill="url(#tg1)" />
    <ellipse id="t-orb2" cx="700" cy="80" rx="200" ry="120" fill="url(#tg2)" />
    <ellipse id="t-orb3" cx="430" cy="160" rx="180" ry="100" fill="url(#tg3)" />
    <rect width="860" height="160" fill="transparent" filter="url(#tgrain)" opacity="0.15" />
  </svg>
  <div style={{ display: 'flex', flexDirection: 'row', alignItems: 'center', gap: 24, zIndex: 10, width: '100%' }}>
    <div style={{ display: 'flex', flexDirection: 'column', gap: 8, flex: 1 }}>
      <span style={{ fontSize: 9, color: 'rgba(167,139,250,0.7)', letterSpacing: 3, textTransform: 'uppercase' }}>LANGUAGES</span>
      <div style={{ display: 'flex', gap: 6, flexWrap: 'wrap' }}>
        {['JavaScript', 'Python', 'C++', 'Java'].map((t, i) => (
          <span key={i} style={{ padding: '4px 14px', background: 'rgba(139,92,246,0.12)', color: 'rgba(221,214,254,0.9)', borderRadius: 100, fontSize: 12, border: '1px solid rgba(139,92,246,0.25)', fontWeight: 500 }}>{t}</span>
        ))}
      </div>
    </div>
    <div style={{ width: 1, height: 60, background: 'rgba(139,92,246,0.2)', flexShrink: 0 }} />
    <div style={{ display: 'flex', flexDirection: 'column', gap: 8, flex: 1 }}>
      <span style={{ fontSize: 9, color: 'rgba(167,139,250,0.7)', letterSpacing: 3, textTransform: 'uppercase' }}>FRAMEWORKS</span>
      <div style={{ display: 'flex', gap: 6, flexWrap: 'wrap' }}>
        {['React', 'Next.js', 'Node.js', 'Docker'].map((t, i) => (
          <span key={i} style={{ padding: '4px 14px', background: 'rgba(59,130,246,0.12)', color: 'rgba(191,219,254,0.9)', borderRadius: 100, fontSize: 12, border: '1px solid rgba(59,130,246,0.25)', fontWeight: 500 }}>{t}</span>
        ))}
      </div>
    </div>
    <div style={{ width: 1, height: 60, background: 'rgba(139,92,246,0.2)', flexShrink: 0 }} />
    <div style={{ display: 'flex', flexDirection: 'column', gap: 8, flex: 1 }}>
      <span style={{ fontSize: 9, color: 'rgba(167,139,250,0.7)', letterSpacing: 3, textTransform: 'uppercase' }}>FOCUS</span>
      <div style={{ display: 'flex', gap: 6, flexWrap: 'wrap' }}>
        {['DSA', 'System Design', 'Gen AI', 'ML'].map((t, i) => (
          <span key={i} style={{ padding: '4px 14px', background: 'rgba(147,51,234,0.12)', color: 'rgba(233,213,255,0.9)', borderRadius: 100, fontSize: 12, border: '1px solid rgba(147,51,234,0.25)', fontWeight: 500 }}>{t}</span>
        ))}
      </div>
    </div>
  </div>
</div>
```

```aura width=110 height=44 link="https://x.com/priyanshudevx" inline align=center
<SocialMediaButton
  icon="https://raw.githubusercontent.com/0xpdev/0xpdev/main/.github/icons/X.png"
  text="X.com"
  backgroundColor="#07050f"
  width={110}
  height={44}
  gradientStops={[{ offset: '0%', color: '#8b5cf6' }, { offset: '30%', color: '#07050f' }, { offset: '60%', color: '#3b82f6' }, { offset: '80%', color: '#07050f' }, { offset: '100%', color: '#8b5cf6' }]}
/>
```

```aura width=125 height=44 link="https://t.me/priyannnsh" inline align=center
<SocialMediaButton
  icon="https://raw.githubusercontent.com/0xpdev/0xpdev/main/.github/icons/telegram.png"
  text="Telegram"
  backgroundColor="#07050f"
  width={125}
  height={44}
  gradientStops={[{ offset: '0%', color: '#8b5cf6' }, { offset: '30%', color: '#07050f' }, { offset: '60%', color: '#3b82f6' }, { offset: '80%', color: '#07050f' }, { offset: '100%', color: '#8b5cf6' }]}
/>
```

```aura width=120 height=44 link="https://discord.gg/9TJ9Uywhky" inline align=center
<SocialMediaButton
  icon="https://raw.githubusercontent.com/0xpdev/0xpdev/main/.github/icons/discord.png"
  text="Discord"
  backgroundColor="#07050f"
  width={120}
  height={44}
  gradientStops={[{ offset: '0%', color: '#8b5cf6' }, { offset: '30%', color: '#07050f' }, { offset: '60%', color: '#3b82f6' }, { offset: '80%', color: '#07050f' }, { offset: '100%', color: '#8b5cf6' }]}
/>
```

```aura width=105 height=44 link="mailto:priyanshudev037@gmail.com" inline align=center
<SocialMediaButton
  icon="https://raw.githubusercontent.com/0xpdev/0xpdev/main/.github/icons/gmail.png"
  text="Email"
  backgroundColor="#07050f"
  width={105}
  height={44}
  gradientStops={[{ offset: '0%', color: '#8b5cf6' }, { offset: '30%', color: '#07050f' }, { offset: '60%', color: '#3b82f6' }, { offset: '80%', color: '#07050f' }, { offset: '100%', color: '#8b5cf6' }]}
/>
```

```aura width=120 height=44 link="https://leetcode.com/u/priyanshudev/" inline align=center
<SocialMediaButton
  icon="https://raw.githubusercontent.com/0xpdev/0xpdev/main/.github/icons/leetcode.png"
  text="LeetCode"
  backgroundColor="#07050f"
  width={120}
  height={44}
  gradientStops={[{ offset: '0%', color: '#8b5cf6' }, { offset: '30%', color: '#07050f' }, { offset: '60%', color: '#3b82f6' }, { offset: '80%', color: '#07050f' }, { offset: '100%', color: '#8b5cf6' }]}
/>
```

<div align="center">
<br/>

![Streak](https://streak-stats.demolab.com?user=0xpdev&theme=dark&background=07050f&ring=8b5cf6&fire=a78bfa&currStreakLabel=a78bfa&sideLabels=888888&dates=555555&border=2d1b69)

<br/>

![Profile Views](https://komarev.com/ghpvc/?username=0xpdev&color=8b5cf6&labelColor=07050f&style=flat-square&label=PROFILE+VIEWS)

<br/>

**Open to collaborations, freelance work, and interesting ideas.**
<br/>
<sub>If you're building something ambitious — let's talk.</sub>

</div>
