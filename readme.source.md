```aura width=860 height=200
<div style={{ width: '100%', height: '100%', background: '#080808', display: 'flex', alignItems: 'center', fontFamily: 'Inter, sans-serif', position: 'relative', overflow: 'hidden', borderRadius: 16, border: '1px solid rgba(255,255,255,0.12)' }}>
  <style>{`
    @keyframes float-slow { 0%, 100% { transform: translateX(0px); opacity: 0.6; } 50% { transform: translateX(350px); opacity: 0.9; } }
    @keyframes float-medium { 0%, 100% { transform: translateX(0px); opacity: 0.5; } 50% { transform: translateX(-250px); opacity: 0.8; } }
    @keyframes float-fast { 0%, 100% { transform: translateX(0px); opacity: 0.7; } 50% { transform: translateX(200px); opacity: 0.4; } }
    @keyframes float-wave { 0%, 100% { transform: translateX(0px); opacity: 0.5; } 33% { transform: translateX(-160px); opacity: 0.7; } 66% { transform: translateX(80px); opacity: 0.8; } }
    @keyframes float-pulse { 0%, 100% { transform: scale(1); opacity: 0.6; } 50% { transform: scale(1.3); opacity: 0.2; } }
    #glow-1 { animation: float-slow 8s ease-in-out infinite; }
    #glow-2 { animation: float-medium 12s ease-in-out infinite; }
    #glow-3 { animation: float-fast 9s ease-in-out infinite; }
    #glow-4 { animation: float-slow 11s ease-in-out infinite reverse; }
    #glow-5 { animation: float-medium 14s ease-in-out infinite reverse; }
    #glow-6 { animation: float-wave 13s ease-in-out infinite; }
    #glow-7 { animation: float-pulse 7s ease-in-out infinite; }
  `}</style>
  <svg width="860" height="200" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="g1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(255,255,255,0.12)" /><stop offset="70%" stopColor="rgba(255,255,255,0)" /></radialGradient>
      <radialGradient id="g2" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(255,255,255,0.09)" /><stop offset="70%" stopColor="rgba(255,255,255,0)" /></radialGradient>
      <radialGradient id="g3" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(255,255,255,0.07)" /><stop offset="70%" stopColor="rgba(255,255,255,0)" /></radialGradient>
      <radialGradient id="g4" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(255,255,255,0.06)" /><stop offset="70%" stopColor="rgba(255,255,255,0)" /></radialGradient>
      <radialGradient id="g5" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(255,255,255,0.08)" /><stop offset="70%" stopColor="rgba(255,255,255,0)" /></radialGradient>
      <radialGradient id="g6" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(255,255,255,0.05)" /><stop offset="70%" stopColor="rgba(255,255,255,0)" /></radialGradient>
      <radialGradient id="g7" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(255,255,255,0.07)" /><stop offset="70%" stopColor="rgba(255,255,255,0)" /></radialGradient>
    </defs>
    <ellipse id="glow-1" cx="180" cy="230" rx="260" ry="190" fill="url(#g1)" />
    <ellipse id="glow-2" cx="300" cy="240" rx="220" ry="160" fill="url(#g2)" />
    <ellipse id="glow-3" cx="420" cy="240" rx="180" ry="140" fill="url(#g3)" />
    <ellipse id="glow-4" cx="550" cy="250" rx="150" ry="120" fill="url(#g4)" />
    <ellipse id="glow-5" cx="750" cy="250" rx="130" ry="110" fill="url(#g5)" />
    <ellipse id="glow-6" cx="490" cy="230" rx="220" ry="170" fill="url(#g6)" />
    <ellipse id="glow-7" cx="590" cy="250" rx="150" ry="130" fill="url(#g7)" />
  </svg>
  <div style={{ position: 'absolute', left: 48, top: 52, width: 96, height: 96, borderRadius: 48, background: 'linear-gradient(135deg, #ffffff, #555555)', display: 'flex', alignItems: 'center', justifyContent: 'center' }}>
    <img src={(github && github.user && github.user.avatar_url) || 'https://github.com/0xpdev.png'} width={88} height={88} style={{ borderRadius: 44 }} />
  </div>
  <div style={{ display: 'flex', flexDirection: 'column', marginLeft: 168, gap: 8, zIndex: 10 }}>
    <div style={{ fontSize: 38, fontWeight: 800, color: '#ffffff', letterSpacing: '-1px', lineHeight: 1 }}>Priyanshu Dev</div>
    <div style={{ fontSize: 15, color: 'rgba(255,255,255,0.5)', fontWeight: 400 }}>Full Stack Engineer · Gen AI · Machine Learning</div>
    <div style={{ display: 'flex', gap: 8, marginTop: 6, flexWrap: 'wrap' }}>
      {['JavaScript', 'Python', 'C++', 'Java', 'React', 'Next.js'].map(function(tag) {
        return <div key={tag} style={{ padding: '4px 12px', borderRadius: 20, background: 'rgba(255,255,255,0.06)', border: '1px solid rgba(255,255,255,0.15)', color: 'rgba(255,255,255,0.75)', fontSize: 12, fontWeight: 600 }}>{tag}</div>;
      })}
    </div>
  </div>
</div>
```

```aura width=860 height=100
<div style={{ display: 'flex', flexDirection: 'row', gap: 12, width: '100%', height: '100%', fontFamily: 'Inter, sans-serif' }}>
  <style>{`
    @keyframes stat-glow { 0%, 100% { box-shadow: 0 0 0px rgba(255,255,255,0); } 50% { box-shadow: 0 0 18px rgba(255,255,255,0.08); } }
    .stat-card { animation: stat-glow 4s ease-in-out infinite; }
  `}</style>
  {[
    { label: 'REPOS', value: (github && github.user && github.user.public_repos) || '8' },
    { label: 'STARS', value: (github && github.totalStars) || '4' },
    { label: 'COMMITS', value: (github && github.totalCommits) || '100+' },
  ].map((stat, i) => (
    <div key={i} className="stat-card" style={{ flex: 1, display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center', background: '#080808', borderRadius: 14, border: '1px solid rgba(255,255,255,0.1)', position: 'relative', overflow: 'hidden' }}>
      <svg width="100%" height="100" style={{ position: 'absolute', top: 0, left: 0 }}>
        <defs><radialGradient id={`sg${i}`} cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(255,255,255,0.06)" /><stop offset="70%" stopColor="rgba(255,255,255,0)" /></radialGradient></defs>
        <ellipse cx="50%" cy="120" rx="120" ry="90" fill={`url(#sg${i})`} />
      </svg>
      <span style={{ fontSize: 28, fontWeight: 700, color: '#ffffff', position: 'relative', zIndex: 1 }}>{stat.value}</span>
      <span style={{ fontSize: 10, color: 'rgba(255,255,255,0.3)', letterSpacing: 3, marginTop: 4, position: 'relative', zIndex: 1 }}>{stat.label}</span>
    </div>
  ))}
</div>
```

```aura width=860 height=160
<div style={{ position: 'relative', width: '100%', height: '100%', background: '#080808', borderRadius: 14, overflow: 'hidden', fontFamily: 'Inter, sans-serif', border: '1px solid rgba(255,255,255,0.1)', display: 'flex', alignItems: 'center', padding: '0 28px', boxSizing: 'border-box' }}>
  <style>{`
    @keyframes t-float-slow { 0%, 100% { transform: translateX(0px); opacity: 0.6; } 50% { transform: translateX(300px); opacity: 0.9; } }
    @keyframes t-float-med { 0%, 100% { transform: translateX(0px); opacity: 0.5; } 50% { transform: translateX(-220px); opacity: 0.8; } }
    #t-orb1 { animation: t-float-slow 9s ease-in-out infinite; }
    #t-orb2 { animation: t-float-med 12s ease-in-out infinite; }
  `}</style>
  <svg width="860" height="160" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="tg1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(255,255,255,0.08)" /><stop offset="70%" stopColor="rgba(255,255,255,0)" /></radialGradient>
      <radialGradient id="tg2" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(255,255,255,0.06)" /><stop offset="70%" stopColor="rgba(255,255,255,0)" /></radialGradient>
    </defs>
    <ellipse id="t-orb1" cx="100" cy="80" rx="200" ry="120" fill="url(#tg1)" />
    <ellipse id="t-orb2" cx="700" cy="80" rx="200" ry="120" fill="url(#tg2)" />
  </svg>
  <div style={{ display: 'flex', flexDirection: 'row', alignItems: 'center', gap: 24, zIndex: 10, width: '100%' }}>
    <div style={{ display: 'flex', flexDirection: 'column', gap: 8, flex: 1 }}>
      <span style={{ fontSize: 9, color: 'rgba(255,255,255,0.4)', letterSpacing: 3, textTransform: 'uppercase' }}>LANGUAGES</span>
      <div style={{ display: 'flex', gap: 6, flexWrap: 'wrap' }}>
        {['JavaScript', 'Python', 'C++', 'Java'].map((t, i) => (
          <span key={i} style={{ padding: '4px 14px', background: 'rgba(255,255,255,0.05)', color: 'rgba(255,255,255,0.8)', borderRadius: 100, fontSize: 12, border: '1px solid rgba(255,255,255,0.12)', fontWeight: 500 }}>{t}</span>
        ))}
      </div>
    </div>
    <div style={{ width: 1, height: 60, background: 'rgba(255,255,255,0.1)', flexShrink: 0 }} />
    <div style={{ display: 'flex', flexDirection: 'column', gap: 8, flex: 1 }}>
      <span style={{ fontSize: 9, color: 'rgba(255,255,255,0.4)', letterSpacing: 3, textTransform: 'uppercase' }}>FRAMEWORKS</span>
      <div style={{ display: 'flex', gap: 6, flexWrap: 'wrap' }}>
        {['React', 'Next.js', 'Node.js', 'Docker'].map((t, i) => (
          <span key={i} style={{ padding: '4px 14px', background: 'rgba(255,255,255,0.05)', color: 'rgba(255,255,255,0.8)', borderRadius: 100, fontSize: 12, border: '1px solid rgba(255,255,255,0.12)', fontWeight: 500 }}>{t}</span>
        ))}
      </div>
    </div>
    <div style={{ width: 1, height: 60, background: 'rgba(255,255,255,0.1)', flexShrink: 0 }} />
    <div style={{ display: 'flex', flexDirection: 'column', gap: 8, flex: 1 }}>
      <span style={{ fontSize: 9, color: 'rgba(255,255,255,0.4)', letterSpacing: 3, textTransform: 'uppercase' }}>FOCUS</span>
      <div style={{ display: 'flex', gap: 6, flexWrap: 'wrap' }}>
        {['DSA', 'System Design', 'Gen AI', 'ML'].map((t, i) => (
          <span key={i} style={{ padding: '4px 14px', background: 'rgba(255,255,255,0.05)', color: 'rgba(255,255,255,0.8)', borderRadius: 100, fontSize: 12, border: '1px solid rgba(255,255,255,0.12)', fontWeight: 500 }}>{t}</span>
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
  backgroundColor="#080808"
  width={110}
  height={44}
  gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '25%', color: '#333333' }, { offset: '50%', color: '#ffffff' }, { offset: '75%', color: '#333333' }, { offset: '100%', color: '#ffffff' }]}
/>
```

```aura width=125 height=44 link="https://t.me/priyannnsh" inline align=center
<SocialMediaButton
  icon="https://raw.githubusercontent.com/0xpdev/0xpdev/main/icons/telegram.png"
  text="Telegram"
  backgroundColor="#080808"
  width={125}
  height={44}
  gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '25%', color: '#333333' }, { offset: '50%', color: '#ffffff' }, { offset: '75%', color: '#333333' }, { offset: '100%', color: '#ffffff' }]}
/>
```

```aura width=120 height=44 link="https://discord.gg/9TJ9Uywhky" inline align=center
<SocialMediaButton
  icon="https://raw.githubusercontent.com/0xpdev/0xpdev/main/icons/discord.png"
  text="Discord"
  backgroundColor="#080808"
  width={120}
  height={44}
  gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '25%', color: '#333333' }, { offset: '50%', color: '#ffffff' }, { offset: '75%', color: '#333333' }, { offset: '100%', color: '#ffffff' }]}
/>
```

```aura width=105 height=44 link="mailto:priyanshudev037@gmail.com" inline align=center
<SocialMediaButton
  icon="https://raw.githubusercontent.com/0xpdev/0xpdev/main/icons/gmail.png"
  text="Email"
  backgroundColor="#080808"
  width={105}
  height={44}
  gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '25%', color: '#333333' }, { offset: '50%', color: '#ffffff' }, { offset: '75%', color: '#333333' }, { offset: '100%', color: '#ffffff' }]}
/>
```

```aura width=120 height=44 link="https://leetcode.com/u/priyanshudev/" inline align=center
<SocialMediaButton
  icon="https://raw.githubusercontent.com/0xpdev/0xpdev/main/icons/leetcode.png"
  text="LeetCode"
  backgroundColor="#080808"
  width={120}
  height={44}
  gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '25%', color: '#333333' }, { offset: '50%', color: '#ffffff' }, { offset: '75%', color: '#333333' }, { offset: '100%', color: '#ffffff' }]}
/>
```

<div align="center">
<br/>

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=0xpdev&show_icons=true&theme=dark&bg_color=080808&title_color=ffffff&text_color=888888&icon_color=ffffff&border_color=222222&hide_border=false)
![Streak](https://streak-stats.demolab.com?user=0xpdev&theme=dark&background=080808&ring=ffffff&fire=ffffff&currStreakLabel=ffffff&sideLabels=888888&dates=555555&border=222222)

<br/>

![Profile Views](https://komarev.com/ghpvc/?username=0xpdev&color=ffffff&labelColor=000000&style=flat-square&label=PROFILE+VIEWS)

<br/>

**Open to collaborations, freelance work, and interesting ideas.**
<br/>
<sub>If you're building something ambitious — let's talk.</sub>

</div>