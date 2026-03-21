# LSaat - Flip Clock (HTML)

## TR
### Proje Ozeti
LSaat, tek bir HTML dosyasi icinde calisan modern gorunumlu bir flip clock (kart cevirme saat) arayuzudur. Responsive yerlesim mantigi sayesinde ekran boyutu degistikce kartlar, bosluklar ve yazi boyutlari dinamik olarak uyarlanir.

### Ozellikler
- Tek dosya mimarisi: Sadece `LSaat.html`
- Flip kart animasyonu (saat, dakika, saniye)
- Saniye gosterimini ac/kapat
- 12/24 saat bicimi gecisi
- Tam ekran modu
- Renkleri ters cevirme modu
- Tarih gosterimi
- Ekran genisligine gore responsive hesaplama

### Klavye Kisayollari
- `D`: Renkleri ters cevir
- `F`: Tam ekran ac/kapat
- `G`: Saniyeyi goster/gizle
- `T`: 12 saat / 24 saat gecisi

### Yerelde Calistirma
1. Bu depoyu indir.
2. `LSaat.html` dosyasini tarayicida ac.
3. Alternatif olarak terminalden bulundugu klasorde su komutu calistir:

```bash
python3 -m http.server 8080
```

Sonra tarayicida `http://localhost:8080/LSaat.html` adresini ac.

### GitHub'a Yukleme (Yeni Repo)
1. GitHub'da yeni bir repo olustur (bos repo tercih edilir).
2. Terminalde proje klasorune gir:

```bash
cd "/Users/samed/Desktop/Projeler/Antigravity Projeler/LSaat/LSaat"
```

3. Git baslat ve dosyalari ekle:

```bash
git init
git add LSaat.html README.md PROJECT_OVERVIEW.md
git commit -m "Initial commit: LSaat HTML flip clock"
```

4. Ana branch'i ayarla, remote bagla ve push et:

```bash
git branch -M main
git remote add origin https://github.com/<kullanici-adi>/<repo-adi>.git
git push -u origin main
```

Not: Kimlik dogrulama sorunu olursa GitHub Personal Access Token (PAT) kullan.

---

## EN
### Project Summary
LSaat is a modern flip-clock interface implemented in a single HTML file. Its responsive layout logic dynamically adjusts card sizes, spacing, and typography based on viewport size.

### Features
- Single-file architecture: only `LSaat.html`
- Flip-card animation (hours, minutes, seconds)
- Toggle seconds visibility
- Switch between 12h and 24h formats
- Fullscreen mode
- Invert-colors mode
- Date display
- Responsive sizing and spacing calculations

### Keyboard Shortcuts
- `D`: Toggle invert colors
- `F`: Toggle fullscreen
- `G`: Toggle seconds visibility
- `T`: Toggle 12h / 24h format

### Run Locally
1. Clone or download the repository.
2. Open `LSaat.html` in your browser.
3. Optional local server:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080/LSaat.html`.

### Upload to GitHub (New Repository)
1. Create a new repository on GitHub (preferably empty).
2. Open terminal in the project folder:

```bash
cd "/Users/samed/Desktop/Projeler/Antigravity Projeler/LSaat/LSaat"
```

3. Initialize git and add files:

```bash
git init
git add LSaat.html README.md PROJECT_OVERVIEW.md
git commit -m "Initial commit: LSaat HTML flip clock"
```

4. Set branch, add remote, and push:

```bash
git branch -M main
git remote add origin https://github.com/<username>/<repo-name>.git
git push -u origin main
```

If authentication fails, use a GitHub Personal Access Token (PAT).

---

## Project Structure
```text
LSaat/
  LSaat.html
  README.md
  PROJECT_OVERVIEW.md
```
