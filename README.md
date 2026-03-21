# LSaat

Modern flip-clock arayuzu sunan, tek dosya ile calisan bir web projesi.

Repository: https://github.com/LynXMaSTeR/LSaat

## TR

### Proje Ozeti
LSaat, saat deneyimini kart-cevirme (flip) animasyon mantigi ile sunan bir arayuzdur.
Tek bir HTML dosyasi uzerinden calisir ve responsive hesaplamalar ile farkli ekran
boyutlarina otomatik uyum saglar.

### Neler Yapar?
- Saat, dakika ve saniye kartlarini flip animasyonu ile gunceller.
- Saniye grubunu acip kapatabilir.
- 12 saat / 24 saat bicimi arasinda gecis yapabilir.
- Tam ekran moduna gecebilir.
- Renkleri ters cevirme (invert) modu sunar.
- Tarih bilgisini alt bolumde gosterir.

### Klavye Kisayollari
- `D`: Invert ac/kapat
- `F`: Tam ekran ac/kapat
- `G`: Saniye goster/gizle
- `T`: 12/24 saat bicimi degistir

### Teknik Detaylar
- Dosya: `LSaat.html`
- Teknolojiler: HTML, CSS, JavaScript
- Layout yaklasimi:
	- Grup bosluklari (`group-gap`) viewport genisligine gore hesaplanir.
	- Kart genisligi (`card-width`) gorunen grup sayisina gore dinamik belirlenir.
	- Yazi boyutlari (`digit-size`, `date-size`) kart boyutlari ile orantili olur.
- Animasyon:
	- Ust yari ve alt yari kartlar ayri katmanlar ile cevrilir.
	- `top-flip` ve `bottom-flip` katmanlari zamanlamali calisir.

### Yerelde Calistirma
1. Depoyu klonla veya indir.
2. `LSaat.html` dosyasini tarayicida ac.
3. Istersen basit bir local server ile de calistirabilirsin:

```bash
python3 -m http.server 8080
```

Sonra tarayicida `http://localhost:8080/LSaat.html` adresini ac.

### GIF Onizleme (Kendi Dosyalarimiz)
Dis kaynaktan GIF kullanmiyoruz. Onizlemeler projede yerel dosya olarak tutulur:
- `assets/preview-dark.gif`
- `assets/preview-light.gif`

![LSaat Dark Preview](assets/preview-dark.gif)
![LSaat Light Preview](assets/preview-light.gif)

### GitHub'a Yukleme
Asagidaki adimlar sadece gerekli dosyalari gondermek icin yeterlidir:

```bash
git init
git add LSaat.html README.md assets/preview-dark.gif assets/preview-light.gif
git commit -m "Initial commit: LSaat HTML flip clock"
git branch -M main
git remote add origin https://github.com/LynXMaSTeR/LSaat.git
git push -u origin main
```

Not:
- Kimlik dogrulama sorunu olursa GitHub PAT kullan.
- GIF onizlemeleri README ile birlikte ayni committe gonderilebilir.

---

## EN

### Project Summary
LSaat is a flip-clock style web interface that runs from a single HTML file.
It uses responsive calculations to adapt card sizing, spacing, and typography
to different viewport sizes.

### Features
- Flip animation for hours, minutes, and seconds
- Toggle seconds group on/off
- Switch between 12h and 24h formats
- Fullscreen toggle
- Invert color mode
- Date display

### Keyboard Shortcuts
- `D`: Toggle invert mode
- `F`: Toggle fullscreen
- `G`: Toggle seconds visibility
- `T`: Toggle 12h / 24h mode

### Technical Notes
- File: `LSaat.html`
- Stack: HTML, CSS, JavaScript
- Responsive behavior:
	- Group spacing is viewport-based.
	- Card width is recalculated based on visible groups.
	- Digit and date typography scales with layout constraints.
- Animation model:
	- Separate top and bottom card halves.
	- Coordinated `top-flip` and `bottom-flip` layers.

### Run Locally
1. Clone or download the repository.
2. Open `LSaat.html` in your browser.
3. Optional local server:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080/LSaat.html`.

### GIF Preview (Our Own Assets)
No external GIF links are used. Previews are stored as local project assets:
- `assets/preview-dark.gif`
- `assets/preview-light.gif`

![LSaat Dark Preview](assets/preview-dark.gif)
![LSaat Light Preview](assets/preview-light.gif)

### Push to GitHub

```bash
git init
git add LSaat.html README.md assets/preview-dark.gif assets/preview-light.gif
git commit -m "Initial commit: LSaat HTML flip clock"
git branch -M main
git remote add origin https://github.com/LynXMaSTeR/LSaat.git
git push -u origin main
```

## Project Structure

```text
LSaat/
	LSaat.html
	README.md
	assets/
		preview-dark.gif
		preview-light.gif
```
