# $VINCENT — Vincent Mallory

Site static (un singur `index.html` + folderul `assets/`). Nu are nevoie de build.

## Structura (trebuie să rămână exact așa)
```
index.html
vercel.json
assets/
  vincent.glb          ← personajul 3D
  reel1.mp4 reel2.mp4 reel3.mp4  (+ .jpg = coperțile)
  *.webp               ← afișele
  favicon.png apple-touch-icon.png
```

## Unde completezi CA, X, Instagram
Deschide `index.html`, caută `CONFIG` (aproape de început) și schimbă:
- `CA:` adresa contractului
- `X_URL:` link-ul de X
- `IG_URL:` link-ul de Instagram
- `BUY_URL:` link de cumpărare (opțional)

## GitHub + Vercel
1. Pe GitHub: New repository → „uploading an existing file” → trage TOT conținutul acestui folder (index.html, vercel.json, README.md și folderul assets) → Commit.
2. Verifică pe GitHub că vezi `assets/vincent.glb` și `assets/reel1.mp4`.
3. Pe Vercel: Add New → Project → alege repo-ul → Framework Preset: **Other** → Root Directory: gol (rădăcina) → Build Command: gol → Deploy.
4. Test: deschide `https://<site>.vercel.app/assets/vincent.glb` — trebuie să descarce fișierul (nu 404).
