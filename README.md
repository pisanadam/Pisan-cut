# Pisan Cut 🎬

CapCut benzeri, **tek HTML dosyasında çalışan** mobil video editörü. Sunucu yok, kurulum yok, hesap yok — her şey tarayıcıda çalışır ve videolar cihazından dışarı çıkmaz.

## Kullanım

`index.html` dosyasını bir tarayıcıda aç, hepsi bu. GitHub Pages ile de yayınlayabilirsin:
Ayarlar → Pages → dalı seç → yayınla.

> En iyi deneyim için mobil Chrome / Safari önerilir. Masaüstünde de çalışır.

## Özellikler

- 📹 **Çoklu klip**: Video ve fotoğraf ekle, sırala
- ✂️ **Kırp & Böl**: Klip uçlarını tutamaçlarla kırp, oynatma çubuğundan ikiye böl
- ⏩ **Hız**: 0.25x – 3x arası hız (yavaş çekim / hızlandırma)
- 🔊 **Ses**: Klip başına ses seviyesi
- 🎨 **Filtreler**: Canlı, Sıcak, Soğuk, Siyah-Beyaz, Sepya, Retro, Dramatik
- 🎛️ **Ayarla**: Parlaklık, kontrast, doygunluk
- 🅣 **Metin**: Renk, boyut, arka plan; önizlemede sürükleyerek konumlandır
- 🎵 **Müzik**: Cihazından ses dosyası ekle, seviyesini ayarla
- ⬛ **En-boy oranı**: 9:16, 16:9, 1:1, 4:5
- 📤 **Dışa aktarma**: Ses miksajıyla birlikte WebM/MP4 (MediaRecorder) — sunucusuz, tamamen tarayıcıda

## Nasıl çalışıyor?

- Önizleme ve dışa aktarma tek bir `<canvas>` üzerinden çizilir; filtreler CSS filter, metinler canvas metni olarak işlenir.
- Dışa aktarma `canvas.captureStream()` + Web Audio miksajı + `MediaRecorder` ile gerçek zamanlı kayıttır; süre, proje süresi kadardır.
- Tarayıcının `MediaRecorder` desteğine göre WebM (VP9/VP8) ya da MP4 üretilir.

## Sınırlamalar

- Dışa aktarma gerçek zamanlıdır (5 dakikalık video ≈ 5 dakika sürer).
- Kodek desteği tarayıcıya bağlıdır; iOS Safari MP4, Chrome/Android WebM üretir.
- Proje kaydetme yoktur; sekme kapanınca kurgu sıfırlanır.
