# Pisan Cut 🎬

CapCut benzeri, **tek HTML dosyasında çalışan** mobil video editörü. Sunucu yok, kurulum yok, hesap yok — her şey tarayıcıda çalışır ve videolar cihazından dışarı çıkmaz.

## Kullanım

`index.html` dosyasını bir tarayıcıda aç, hepsi bu. GitHub Pages ile de yayınlayabilirsin:
Ayarlar → Pages → dalı seç → yayınla.

> En iyi deneyim için mobil Chrome / Safari önerilir. Masaüstünde de çalışır.

## Özellikler

- 🏠 **Ana ekran**: CapCut benzeri açılış menüsü, araç kısayolları ve proje listesi
- 💾 **Otomatik kayıt**: Projeler medya dosyalarıyla birlikte IndexedDB'ye kaydedilir; sekmeyi kapatsan bile ana ekrandan geri açabilirsin (yeniden adlandır / sil dahil)
- 📹 **Çoklu klip**: Video ve fotoğraf ekle, sırala
- ✂️ **Kırp & Böl**: Klip uçlarını tutamaçlarla kırp, oynatma çubuğundan ikiye böl
- ⇄ **Geçişler**: Klipler arasında Solma, Siyah/Beyaz, Kaydırma, Silme, Yakınlaşma — süre ayarlı; zaman çizelgesindeki sınır düğmesinden eklenir
- ✨ **Efektler (CapCut tarzı panel)**: Arama + kategori sekmeleri (Trend / Atmosfer / Retro / Hareket); Arızalı Sinyal, Konfeti, Parıltı, VHS, Kalpler, Kar, Yağmur, Vinyet, Film Greni, Negatif Renk, Kamera Hareketi, Nabız, Titrek Aksama
- 🖼 **Bindirme (PiP)**: Video/fotoğrafı katman olarak üstüne ekle — sesi mikslenir, süresi ve konumu ayarlanır
- 🤏 **Dokunmatik dönüşüm**: Ana klip, metin, obje ve bindirmeleri tek parmakla taşı, iki parmakla yakınlaştır/boyutlandır; sürüklerken merkez mıknatısı (kılavuz çizgisiyle ortaya yapışma) ve panellerde "Tam Ortala / Yatay / Dikey" düğmeleri
- 🗂 **Katmanlar**: Üst üste binen öğelerde "öne getir / arkaya gönder" ile sıralama
- ↔️ **Çubuk sürükleme**: Zaman çizelgesinde metin/obje/bindirme çubuklarını ortadan taşı, uçlarından uzat/kısalt
- ⏩ **Hız**: 0.01x – 10x sürgüyle (logaritmik) + hazır değerler; "ses perdesini değiştir" aç/kapa
- 🔊 **Ses**: Klip başına ses seviyesi
- 🎨 **Filtreler**: Canlı, Sıcak, Soğuk, Siyah-Beyaz, Sepya, Retro, Dramatik
- 🎛️ **Ayarla**: Parlaklık, kontrast, doygunluk
- 🅣 **Animasyonlu metin**: Giriş animasyonları (Pop, Solma, Kayma, Zıplama, Dönme, Daktilo) + döngü hareketleri (Dalga, Gökkuşağı, Nabız, Süzülme, Titreme); sürükleyerek konumlandır
- 😀 **Bindirme objeler**: Emoji çıkartmaları, giriş animasyonu + sürekli hareket (süzülme, dönme, nabız…), boyut/süre ayarı, sürükleyerek taşıma
- 🎵 **Müzik**: Birden çok parça ekle (oynatma çubuğundan başlar); çubuğunu sürükleyerek taşı/kırp, böl, sil, hızlandır (0.1x–10x), ses seviyesi; müzik videodan uzunsa proje son karede donarak müziğin sonuna kadar uzar
- ⬛ **En-boy oranı**: 9:16, 16:9, 1:1, 4:5
- 🎚️ **Dışa aktarma ayarları**: Çözünürlük (480p / 720p / 1080p) ve kare hızı (24 / 30 / 60 fps) seçimi, tahmini dosya boyutuyla; seçimler projeyle birlikte kaydedilir
- 📤 **Hızlı render (CapCut tarzı)**: WebCodecs destekleyen tarayıcılarda video kare kare offline kodlanır, ses offline mikslenir — önizleme taksa bile çıktı her zaman akıcıdır ve çoğu cihazda gerçek zamandan hızlı biter. WebCodecs yoksa MediaRecorder ile gerçek zamanlı kayda düşer.
- ⚡ **Akıcı önizleme**: Düzenleme sırasında canvas ekran çözünürlüğünde çalışır (dışa aktarmada tam çözünürlüğe geçer), kare yalnızca gerektiğinde yeniden çizilir

## Nasıl çalışıyor?

- Önizleme ve dışa aktarma tek bir `<canvas>` üzerinden çizilir; filtreler CSS filter, metinler canvas metni olarak işlenir.
- **Hızlı render**: her kare için videolar tam zamana sarılır, kare `VideoEncoder` (VP9/VP8) ile kodlanır; ses `OfflineAudioContext` ile mikslenip `AudioEncoder` (Opus) ile kodlanır ve dosya içindeki minimal Matroska/WebM muxer ile birleştirilir. Kare düşmesi mümkün değildir. Her klip için ikinci bir "gölge" video elemanı tutulur: bir kare kodlanırken sıradaki karenin sarması paralel yürür (çift tampon), bu render süresini belirgin kısaltır.
- WebCodecs olmayan tarayıcılarda `canvas.captureStream()` + `MediaRecorder` ile gerçek zamanlı kayda düşülür.

## Sınırlamalar

- Hızlı render WebCodecs gerektirir (Chrome/Edge/Android WebView 94+, Safari 16.4+ kısmi); yoksa dışa aktarma gerçek zamanlı sürer.
- Kodek desteği tarayıcıya bağlıdır; çıktı genellikle WebM'dir (yedek yolda iOS Safari MP4 üretebilir).
- Projeler tarayıcının IndexedDB deposunda tutulur; tarayıcı verilerini/site verilerini silersen projeler de silinir ve başka cihazdan erişilemez.
