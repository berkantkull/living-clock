# LIVING CLOCK

**“Zaman durağan değildir. Bu saat de öyle.”**

LIVING CLOCK, zamanı nefes alan ve dokunmaya tepki veren yaşam biçimleriyle görünür kılan, bağımlılıksız bir Canvas 2D enstalasyonu. Varsayılan dil Türkçedir ve arayüzden İngilizceye geçilebilir.

[Living Clock’u canlı aç](https://berkantkull.github.io/living-clock/)

## Özellikler

- Cihazın gerçek yerel zamanını kullanan hassas saat ve tarih
- Yerel saate göre değişen ışık, nefes ritmi, dakika dalgaları ve gece yarısı geçişi
- Farklı anatomileri ve hareketleri olan altı aile. **Peçe**, **Kök**, **Spor**, **Kıvrım**, **Koloni** ve **Lif**
- Her basışta farklı bir örnek. **Yeni yaşam**, iki aileyi birleştirerek yeni bir melez üretir.
- Seçili örnek ve dil tercihi `localStorage` ile korunur.
- Türkçe ve İngilizce arayüz
- Zen Modu, tarayıcı tam ekranı ve tam kompozisyon PNG dışa aktarma
- Klavye erişimi, görünür odak durumları ve azaltılmış hareket desteği
- Masaüstü, tablet ve mobil ekranlar için duyarlı tasarım
- Harici bağımlılık, çerçeve, API, arka uç veya derleme adımı yok

## Çalıştırma

`index.html` dosyasını doğrudan açabilirsiniz. Yerel sunucu kullanmak için klasörde aşağıdaki komutu çalıştırın.

```bash
python -m http.server 8080
```

Sonra `http://localhost:8080` adresini açın.

## Kontroller

- İşaretçiyi hareket ettirin veya sahneye dokunarak formu etkileyin.
- Aynı aileye tekrar basarak yeni bir örnek oluşturun.
- `Z` ile Zen Moduna girin. `Escape` ya da sahneye dokunarak çıkın.
- Üstteki araçlar tam ekranı, Zen Modunu ve PNG kaydını açar. `TR / EN` arayüz dilini değiştirir.

## GitHub Pages

GitHub Pages, siteyi `main` dalının kök dizininden yayınlar.

## Teknik notlar

Uygulamanın tamamı tek bir `index.html` dosyasındadır. Canvas çözünürlüğü en fazla `2x` piksel oranında çalışır. Sekme görünmediğinde animasyon durur. `prefers-reduced-motion` açıkken nefes animasyonu ve dalgalar devre dışı kalır.
