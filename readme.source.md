```aura width=800 height=120
<div style={{ position: 'relative', display: 'flex', flexDirection: 'row', alignItems: 'center', width: '100%', height: '100%', background: 'linear-gradient(135deg, #020817 0%, #0a1628 50%, #020817 100%)', borderRadius: 20, overflow: 'hidden', fontFamily: 'Inter, sans-serif', padding: '0 32px', boxSizing: 'border-box' }}>
  <style>{`
    @keyframes blue-orb-a { 0%, 100% { transform: translate(0,0); opacity: 0.5; } 50% { transform: translate(20px,-15px); opacity: 0.8; } }
    @keyframes blue-orb-b { 0%, 100% { transform: translate(0,0); opacity: 0.4; } 50% { transform: translate(-15px,10px); opacity: 0.7; } }
    #bo1 { animation: blue-orb-a 9s ease-in-out infinite; }
    #bo2 { animation: blue-orb-b 11s ease-in-out infinite 1s; }
    #bo3 { animation: blue-orb-a 8s ease-in-out infinite 2s; }
  `}</style>
  <svg width="800" height="120" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="bg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(59,130,246,0.5)" />
        <stop offset="100%" stopColor="rgba(59,130,246,0)" />
      </radialGradient>
      <radialGradient id="bg2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(99,102,241,0.4)" />
        <stop offset="100%" stopColor="rgba(99,102,241,0)" />
      </radialGradient>
      <radialGradient id="bg3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(14,165,233,0.35)" />
        <stop offset="100%" stopColor="rgba(14,165,233,0)" />
      </radialGradient>
    </defs>
    <ellipse id="bo1" cx="700" cy="60" rx="200" ry="100" fill="url(#bg1)" />
    <ellipse id="bo2" cx="100" cy="30" rx="180" ry="90" fill="url(#bg2)" />
    <ellipse id="bo3" cx="400" cy="100" rx="160" ry="80" fill="url(#bg3)" />
  </svg>
  <img src={(github && github.user && github.user.avatar_url) || 'https://github.com/0xpdev.png'} style={{ width: 64, height: 64, borderRadius: '50%', border: '2px solid rgba(59,130,246,0.5)', zIndex: 10, flexShrink: 0 }} />
  <div style={{ display: 'flex', flexDirection: 'column', marginLeft: 20, zIndex: 10 }}>
    <span style={{ fontSize: 28, fontWeight: 700, color: '#ffffff', letterSpacing: -0.5 }}>{(github && github.user && (github.user.name || github.user.login)) || 'Priyanshu Dev'}</span>
    <span style={{ fontSize: 12, color: 'rgba(148,163,184,0.8)', marginTop: 4, letterSpacing: 2, textTransform: 'uppercase' }}>Full Stack · Gen AI · Machine Learning</span>
    <div style={{ display: 'flex', gap: 6, marginTop: 10 }}>
      {['React', 'Next.js', 'Python', 'TypeScript', 'C++'].map((t, i) => (
        <span key={i} style={{ padding: '3px 10px', background: 'rgba(59,130,246,0.12)', color: 'rgba(148,163,184,0.9)', borderRadius: 100, fontSize: 10, border: '1px solid rgba(59,130,246,0.25)', letterSpacing: 0.5 }}>{t}</span>
      ))}
    </div>
  </div>
</div>
```

```aura width=800 height=100
<div style={{ display: 'flex', flexDirection: 'row', gap: 12, width: '100%', height: '100%', fontFamily: 'Inter, sans-serif' }}>
  {[
    { label: 'REPOS', value: (github && github.user && github.user.public_repos) || '8' },
    { label: 'STARS', value: (github && github.totalStars) || '4', color: '#f59e0b' },
    { label: 'COMMITS', value: (github && github.totalCommits) || '100+', color: '#3b82f6' },
  ].map((stat, i) => (
    <div key={i} style={{ flex: 1, display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center', background: 'linear-gradient(135deg, #020817 0%, #0a1628 100%)', borderRadius: 14, border: '1px solid rgba(59,130,246,0.15)' }}>
      <span style={{ fontSize: 28, fontWeight: 700, color: stat.color || '#e2e8f0' }}>{stat.value}</span>
      <span style={{ fontSize: 10, color: 'rgba(148,163,184,0.5)', letterSpacing: 3, marginTop: 4 }}>{stat.label}</span>
    </div>
  ))}
</div>
```

```aura width=800 height=130
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', justifyContent: 'center', width: '100%', height: '100%', background: 'linear-gradient(135deg, #020817 0%, #0a1628 100%)', borderRadius: 14, overflow: 'hidden', fontFamily: 'Inter, sans-serif', padding: '0 28px', boxSizing: 'border-box', border: '1px solid rgba(59,130,246,0.15)' }}>
  <svg width="800" height="130" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="tg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(59,130,246,0.2)" />
        <stop offset="100%" stopColor="rgba(59,130,246,0)" />
      </radialGradient>
    </defs>
    <ellipse cx="700" cy="65" rx="200" ry="100" fill="url(#tg1)" />
  </svg>
  <div style={{ display: 'flex', flexDirection: 'row', alignItems: 'center', gap: 24, zIndex: 10 }}>
    <div style={{ display: 'flex', flexDirection: 'column', gap: 4 }}>
      <span style={{ fontSize: 9, color: 'rgba(59,130,246,0.7)', letterSpacing: 3, textTransform: 'uppercase', marginBottom: 6 }}>LANGUAGES</span>
      <div style={{ display: 'flex', gap: 6, flexWrap: 'wrap' }}>
        {['JavaScript', 'TypeScript', 'Python', 'C++', 'Java'].map((t, i) => (
          <span key={i} style={{ padding: '4px 12px', background: 'rgba(59,130,246,0.1)', color: 'rgba(203,213,225,0.9)', borderRadius: 100, fontSize: 11, border: '1px solid rgba(59,130,246,0.2)' }}>{t}</span>
        ))}
      </div>
    </div>
    <div style={{ width: 1, height: 60, background: 'rgba(59,130,246,0.2)' }} />
    <div style={{ display: 'flex', flexDirection: 'column', gap: 4 }}>
      <span style={{ fontSize: 9, color: 'rgba(59,130,246,0.7)', letterSpacing: 3, textTransform: 'uppercase', marginBottom: 6 }}>FRAMEWORKS</span>
      <div style={{ display: 'flex', gap: 6, flexWrap: 'wrap' }}>
        {['React', 'Next.js', 'Node.js', 'TensorFlow', 'Docker'].map((t, i) => (
          <span key={i} style={{ padding: '4px 12px', background: 'rgba(99,102,241,0.1)', color: 'rgba(203,213,225,0.9)', borderRadius: 100, fontSize: 11, border: '1px solid rgba(99,102,241,0.2)' }}>{t}</span>
        ))}
      </div>
    </div>
  </div>
</div>
```

```aura width=120 height=44 link="https://github.com/0xpdev" inline align=center
<SocialMediaButton
  icon="https://cdn.simpleicons.org/github/ffffff"
  text="GitHub"
  backgroundColor="#0a1628"
  width={120}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#3b82f6' },
    { offset: '50%', color: '#1d4ed8' },
    { offset: '100%', color: '#3b82f6' },
  ]}
/>
```

```aura width=110 height=44 link="https://x.com/priyanshudevx" inline align=center
<SocialMediaButton
  icon="https://cdn.simpleicons.org/x/ffffff"
  text="X.com"
  backgroundColor="#0a1628"
  width={110}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#3b82f6' },
    { offset: '50%', color: '#1d4ed8' },
    { offset: '100%', color: '#3b82f6' },
  ]}
/>
```

```aura width=130 height=44 link="https://substack.com/@priyanshudev" inline align=center
<SocialMediaButton
  icon="https://cdn.simpleicons.org/substack/FF6719"
  text="Substack"
  backgroundColor="#0a1628"
  width={130}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#3b82f6' },
    { offset: '50%', color: '#1d4ed8' },
    { offset: '100%', color: '#3b82f6' },
  ]}
/>
```

```aura width=125 height=44 link="https://linkedin.com/in/priyanshudev1" inline align=center
<SocialMediaButton
  icon="https://cdn.simpleicons.org/linkedin/0A66C2"
  text="LinkedIn"
  backgroundColor="#0a1628"
  width={125}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#3b82f6' },
    { offset: '50%', color: '#1d4ed8' },
    { offset: '100%', color: '#3b82f6' },
  ]}
/>
```

```aura width=120 height=44 link="https://discord.com/users/priyanshu.dev." inline align=center
<SocialMediaButton
  icon="https://cdn.simpleicons.org/discord/5865F2"
  text="Discord"
  backgroundColor="#0a1628"
  width={120}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#3b82f6' },
    { offset: '50%', color: '#1d4ed8' },
    { offset: '100%', color: '#3b82f6' },
  ]}
/>
```

```aura width=105 height=44 link="mailto:priyanshudev037@gmail.com" inline align=center
<SocialMediaButton
  icon="https://cdn.simpleicons.org/gmail/EA4335"
  text="Email"
  backgroundColor="#0a1628"
  width={105}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#3b82f6' },
    { offset: '50%', color: '#1d4ed8' },
    { offset: '100%', color: '#3b82f6' },
  ]}
/>
```