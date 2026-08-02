```aura width=860 height=190
<div style={{
  width: '100%', height: '100%', background: '#12060d',
  display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center',
  fontFamily: 'Inter', position: 'relative', overflow: 'hidden', borderRadius: 16,
  border: '1px solid rgba(255,77,166,0.25)'
}}>
  <svg width="860" height="190" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="p1" cx="30%" cy="40%" r="60%">
        <stop offset="0%" stopColor="rgba(255,77,166,0.55)" />
        <stop offset="45%" stopColor="rgba(200,30,120,0.22)" />
        <stop offset="70%" stopColor="rgba(200,30,120,0)" />
      </radialGradient>
      <radialGradient id="p2" cx="75%" cy="60%" r="55%">
        <stop offset="0%" stopColor="rgba(180,50,255,0.40)" />
        <stop offset="50%" stopColor="rgba(140,30,220,0.16)" />
        <stop offset="70%" stopColor="rgba(140,30,220,0)" />
      </radialGradient>
    </defs>
    <ellipse cx="220" cy="90" rx="260" ry="180" fill="url(#p1)" />
    <ellipse cx="650" cy="110" rx="240" ry="170" fill="url(#p2)" />
  </svg>

  <div style={{ display: 'flex', fontSize: 44, fontWeight: 800, color: '#ffffff', letterSpacing: '2px', zIndex: 10 }}>
    ANANYA
  </div>
  <div style={{ display: 'flex', fontSize: 15, fontWeight: 600, color: '#ff8fc7', letterSpacing: '3px', marginTop: 6, zIndex: 10 }}>
    SOFTWARE ENGINEER (IN THE MAKING)
  </div>
  <div style={{ display: 'flex', fontSize: 12, fontWeight: 400, color: 'rgba(255,220,240,0.55)', letterSpacing: '2px', marginTop: 10, zIndex: 10 }}>
    DTU · SE'28 · NEW DELHI
  </div>
</div>
```

```aura width=170 height=48 link="https://linkedin.com/in/ananyamonga" inline align=center
<div style={{
  width: '100%', height: '100%', display: 'flex', alignItems: 'center', justifyContent: 'center',
  background: '#ff4da6', borderRadius: 10, fontFamily: 'Inter', fontSize: 13, fontWeight: 700,
  color: '#12060d', letterSpacing: '1px'
}}>LINKEDIN</div>
```
```aura width=170 height=48 link="https://leetcode.com/u/ananyarchive" inline align=center
<div style={{
  width: '100%', height: '100%', display: 'flex', alignItems: 'center', justifyContent: 'center',
  background: '#ff4da6', borderRadius: 10, fontFamily: 'Inter', fontSize: 13, fontWeight: 700,
  color: '#12060d', letterSpacing: '1px'
}}>LEETCODE</div>
```
```aura width=170 height=48 link="https://codeforces.com/profile/ananyarchiv3" inline align=center
<div style={{
  width: '100%', height: '100%', display: 'flex', alignItems: 'center', justifyContent: 'center',
  background: '#ff4da6', borderRadius: 10, fontFamily: 'Inter', fontSize: 13, fontWeight: 700,
  color: '#12060d', letterSpacing: '1px'
}}>CODEFORCES</div>
```

```aura width=860 height=140
<div style={{
  width: '100%', height: '100%', background: '#12060d', borderRadius: 16,
  border: '1px solid rgba(255,77,166,0.2)', display: 'flex', alignItems: 'center', justifyContent: 'space-around',
  fontFamily: 'Inter'
}}>
  <div style={{ display: 'flex', flexDirection: 'column', alignItems: 'center' }}>
    <div style={{ display: 'flex', fontSize: 34, fontWeight: 800, color: '#ffffff' }}>{(github && github.stats && github.stats.totalStars) || 0}</div>
    <div style={{ display: 'flex', fontSize: 12, fontWeight: 600, color: '#ff8fc7', letterSpacing: '1px', marginTop: 4 }}>STARS</div>
  </div>
  <div style={{ display: 'flex', flexDirection: 'column', alignItems: 'center' }}>
    <div style={{ display: 'flex', fontSize: 34, fontWeight: 800, color: '#ffffff' }}>{(github && github.stats && github.stats.totalForks) || 0}</div>
    <div style={{ display: 'flex', fontSize: 12, fontWeight: 600, color: '#ff8fc7', letterSpacing: '1px', marginTop: 4 }}>FORKS</div>
  </div>
  <div style={{ display: 'flex', flexDirection: 'column', alignItems: 'center' }}>
    <div style={{ display: 'flex', fontSize: 34, fontWeight: 800, color: '#ffffff' }}>{(github && github.stats && github.stats.totalRepos) || 0}</div>
    <div style={{ display: 'flex', fontSize: 12, fontWeight: 600, color: '#ff8fc7', letterSpacing: '1px', marginTop: 4 }}>REPOS</div>
  </div>
  <div style={{ display: 'flex', flexDirection: 'column', alignItems: 'center' }}>
    <div style={{ display: 'flex', fontSize: 34, fontWeight: 800, color: '#ffffff' }}>{(github && github.stats && github.stats.totalCommits) || 0}</div>
    <div style={{ display: 'flex', fontSize: 12, fontWeight: 600, color: '#ff8fc7', letterSpacing: '1px', marginTop: 4 }}>COMMITS</div>
  </div>
</div>
```

```aura width=860 height=200
<div style={{
  width: '100%', height: '100%', background: '#12060d', borderRadius: 16,
  border: '1px solid rgba(255,77,166,0.2)', display: 'flex', flexDirection: 'column',
  padding: 28, fontFamily: 'Inter'
}}>
  <div style={{ display: 'flex', fontSize: 13, fontWeight: 700, color: '#ff8fc7', letterSpacing: '2px', marginBottom: 16 }}>
    STACK ANALYTICS
  </div>
  <div style={{ display: 'flex', width: '100%', height: 10, borderRadius: 6, overflow: 'hidden', marginBottom: 20 }}>
    {((github && github.languages) || []).slice(0, 8).map(function(l, i) {
      var pct = (l && l.percentage) || 0;
      return <div key={(l.name || 'lang') + i} style={{ display: 'flex', width: (pct * 8) + 'px', height: '100%', background: (l && l.color) || '#ff4da6' }} />;
    })}
  </div>
  <div style={{ display: 'flex', flexWrap: 'wrap', gap: 20 }}>
    {((github && github.languages) || []).slice(0, 8).map(function(l, i) {
      var pct = (l && l.percentage) || 0;
      return (
        <div key={(l.name || 'lang') + '-label-' + i} style={{ display: 'flex', alignItems: 'center', gap: 8, width: '22%' }}>
          <div style={{ display: 'flex', width: 8, height: 8, borderRadius: 4, background: (l && l.color) || '#ff4da6' }} />
          <div style={{ display: 'flex', fontSize: 12, color: 'rgba(255,220,240,0.8)' }}>{l.name} {Math.round(pct)}%</div>
        </div>
      );
    })}
  </div>
</div>
```

## 🛠️ Tech Stack

**Languages**
[![My Skills](https://skillicons.dev/icons?i=cpp,py,js,ts,java&theme=dark)](https://skillicons.dev)

**AI & Machine Learning**
[![My Skills](https://skillicons.dev/icons?i=pytorch,tensorflow,sklearn,opencv&theme=dark)](https://skillicons.dev)

**Backend**
[![My Skills](https://skillicons.dev/icons?i=fastapi,nodejs,redis,postgres,mongodb&theme=dark)](https://skillicons.dev)

**Cloud & DevOps**
[![My Skills](https://skillicons.dev/icons?i=docker,kubernetes,githubactions,aws&theme=dark)](https://skillicons.dev)

## 🐍 Contribution Snake

<div align="center">
  <img src="https://raw.githubusercontent.com/ananyarchive/ananyarchive/output/github-contribution-grid-snake-dark.svg" alt="Snake animation" />
</div>
