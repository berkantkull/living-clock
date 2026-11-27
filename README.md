# LIVING CLOCK

**“Zaman durağan değildir. Bu saat de öyle.”**

LIVING CLOCK, zamanı nefes alan ve dokunmaya tepki veren yaşam biçimleriyle görünür kılan, bağımlılıksız bir Canvas 2D enstalasyonu. Varsayılan dil Türkçedir ve arayüzden İngilizceye geçilebilir.

[Living Clock’u canlı aç](https://berkantkull.github.io/living-clock/)

## Özellikler

- Cihazın gerçek yerel zamanını kullanan hassas saat ve tarih
- Yerel saate göre değişen ışık, nefes ritmi, dakika dalgaları ve gece yarısı geçişi
- Nefes alışverişi formun hacmini ve ışığını değiştirir. Yakınında beklemek, yavaş gezinmek veya sahne odaktayken boşluk tuşuna basmak büyümeyi besler.
- Aynı bölgeye art arda tıklamak veya dokunmak stresi artırır. Yakındaki bir uzantı kopabilir ve zamanla yeniden büyür.
- Formun gelişimi, enerji durumu ve yaraları bu tarayıcıda kalır. Sayfa tekrar açıldığında arada geçen süre gelişime yansır.
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

- Yavaşça gezinin veya formun yakınında durun. Hızlı ve tekrarlı dokunuşların formu nasıl değiştirdiğini gözlemleyin.
- Aynı aileye tekrar basarak yeni bir örnek oluşturun.
- `Z` ile Zen Moduna girin. `Escape` ya da sahneye dokunarak çıkın.
- Üstteki araçlar tam ekranı, Zen Modunu ve PNG kaydını açar. `TR / EN` arayüz dilini değiştirir.

## GitHub Pages

GitHub Pages, siteyi `main` dalının kök dizininden yayınlar.

## Teknik notlar

Uygulamanın tamamı tek bir `index.html` dosyasındadır. Canvas çözünürlüğü en fazla `2x` piksel oranında çalışır. Sekme görünmediğinde animasyon durur. `prefers-reduced-motion` açıkken nefes animasyonu ve dalgalar devre dışı kalır.

**Güneş ışığını eşle** etkinleştirilirse ışık, yaklaşık konum ile günün tarih ve saatine göre hesaplanır. Konum yalnızca bu oturum boyunca tarayıcı belleğinde tutulur. Konum eşlemesi kapalıyken ışık yerel saatten tahmin edilir. [NOAA güneş konumu denklemleri](https://www.gml.noaa.gov/grad/solcalc/solareqns.PDF)

## Telif hakları

© 2026 Berkant Kul. Tüm hakları saklıdır. [Hak bildirimi](LICENSE)
