# LSaat

Modern bir flip-clock arayüzü sunan, tek bir HTML dosyasıyla çalışan web projesi.

Repository: https://github.com/LynXMaSTeR/LSaat

## TR

### Proje Özeti
LSaat, kart çevirme (flip) animasyonlarıyla çalışan modern bir dijital saat arayüzüdür.
Tek bir HTML dosyası üzerinden çalışır ve duyarlı yerleşim hesaplamaları sayesinde
farklı ekran boyutlarına otomatik olarak uyum sağlar.

### Özellikler
- Saat, dakika ve saniye kartlarını flip animasyonuyla günceller.
- Saniye grubunu gösterip gizleyebilirsiniz.
- 12 saat ve 24 saat biçimleri arasında geçiş yapabilirsiniz.
- Tam ekran modunu açıp kapatabilirsiniz.
- Renkleri ters çevirme (invert) modunu etkinleştirebilirsiniz.
- Tarih bilgisini alt bölümde görüntüler.

### Klavye Kısayolları
- `D`: İnvert modunu aç/kapat
- `F`: Tam ekran modunu aç/kapat
- `G`: Saniye grubunu göster/gizle
- `T`: 12/24 saat biçimi arasında geçiş yap

### Teknik Detaylar
- Dosya: `LSaat.html`
- Teknolojiler: HTML, CSS, JavaScript
- Yerleşim yaklaşımı:
	- Grup boşlukları (`group-gap`) ekran genişliğine göre hesaplanır.
	- Kart genişliği (`card-width`), görünür grup sayısına göre dinamik olarak belirlenir.
	- Yazı boyutları (`digit-size`, `date-size`), kart ölçülerine orantılı şekilde ölçeklenir.
- Animasyon yapısı:
	- Kartların üst ve alt yarımları ayrı katmanlarda işlenir.
	- `top-flip` ve `bottom-flip` katmanları zamanlamalı olarak birlikte çalışır.

### Yerelde Çalıştırma
1. Depoyu klonlayın veya indirin.
2. `LSaat.html` dosyasını tarayıcıda açın.
3. İsterseniz basit bir yerel sunucu ile de çalıştırabilirsiniz:

```bash
python3 -m http.server 8080
```

Daha sonra tarayıcıda `http://localhost:8080/LSaat.html` adresini açın.

### GIF Önizleme (Kendi Dosyalarımız)
Harici GIF bağlantısı kullanılmaz. Önizlemeler, proje içinde yerel dosya olarak tutulur:
- `assets/preview-dark.gif`
- `assets/preview-light.gif`

![LSaat Dark Preview](assets/preview-dark.gif)
![LSaat Light Preview](assets/preview-light.gif)

### GitHub'a Yükleme
Aşağıdaki adımlar, yalnızca gerekli dosyaları göndermek için yeterlidir:

```bash
git init
git add LSaat.html README.md assets/preview-dark.gif assets/preview-light.gif
git commit -m "Initial commit: LSaat HTML flip clock"
git branch -M main
git remote add origin https://github.com/LynXMaSTeR/LSaat.git
git push -u origin main
```

Not:
- Kimlik doğrulama sorunu yaşarsanız GitHub PAT kullanın.
- GIF önizlemelerini README ile birlikte aynı commit içinde gönderebilirsiniz.

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
