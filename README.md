# LIVING CLOCK

**“Zaman durağan değildir. Bu saat de öyle.”**

LIVING CLOCK, yerel zamanı sürekli dönüşen organik bir form üzerinden görünür kılan, bağımlılıksız bir Canvas 2D dijital sanat deneyimidir. Varsayılan dil Türkçedir; arayüzden İngilizceye geçilebilir.

[Living Clock’u canlı aç](https://berkantkull.github.io/living-clock/)

## Özellikler

- Cihazın gerçek yerel zamanını kullanan hassas saat ve tarih
- Zamanla, işaretçiyle ve dokunmayla yaşayan prosedürel Canvas 2D formu
- Dakika değişimlerinde genişleyen dalga ve gece yarısında özel geçiş
- **Otomatik, Sıvı, Güneş, Nebula ve Monokrom** atmosferler
- Tema ve dil tercihlerinin `localStorage` ile saklanması
- Türkçe ve İngilizce arayüz
- Zen Modu, tarayıcı tam ekranı ve tam kompozisyon PNG dışa aktarma
- Klavye erişimi, görünür odak durumları ve azaltılmış hareket desteği
- Masaüstü, tablet ve mobil ekranlar için duyarlı tasarım
- Harici bağımlılık, çerçeve, API, arka uç veya derleme adımı yok

## Çalıştırma

`index.html` dosyasını doğrudan açabilir veya klasörde basit bir yerel sunucu başlatabilirsiniz:

```bash
npx serve .
```

Python yüklüyse:

```bash
python -m http.server 8080
```

Sonra `http://localhost:8080` adresini açın.

## Kontroller

- Organik forma tıklama/dokunma: geçici dalga
- `Z`: Zen Modu
- `Escape`: Zen Modundan çıkış
- Alt sağ kontroller: tam ekran, Zen Modu ve PNG kaydı
- Üst sağ `TR / EN`: arayüz dili

## GitHub Pages

GitHub Pages, siteyi `main` dalının kök dizininden yayınlar.

## Teknik notlar

Uygulamanın tamamı tek bir `index.html` dosyasındadır. Canvas çözünürlüğü performans için en fazla `2x` piksel oranında çalışır; sekme görünmediğinde animasyon durur ve `prefers-reduced-motion` açıkken hareket belirgin biçimde azaltılır.

---

Designed and built as an experimental living timepiece.
