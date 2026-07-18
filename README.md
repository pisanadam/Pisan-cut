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
- ✨ **Efektler**: Ken Burns, Nabız, Sarsıntı, VHS, Glitch, Film Greni, Vinyet, Kar, Yağmur, Parıltı
- ⏩ **Hız**: 0.25x – 3x arası hız (yavaş çekim / hızlandırma)
- 🔊 **Ses**: Klip başına ses seviyesi
- 🎨 **Filtreler**: Canlı, Sıcak, Soğuk, Siyah-Beyaz, Sepya, Retro, Dramatik
- 🎛️ **Ayarla**: Parlaklık, kontrast, doygunluk
- 🅣 **Animasyonlu metin**: Giriş animasyonları (Pop, Solma, Kayma, Zıplama, Dönme, Daktilo) + döngü hareketleri (Dalga, Gökkuşağı, Nabız, Süzülme, Titreme); sürükleyerek konumlandır
- 😀 **Bindirme objeler**: Emoji çıkartmaları, giriş animasyonu + sürekli hareket (süzülme, dönme, nabız…), boyut/süre ayarı, sürükleyerek taşıma
- 🎵 **Müzik**: Cihazından ses dosyası ekle, seviyesini ayarla
- ⬛ **En-boy oranı**: 9:16, 16:9, 1:1, 4:5
- 📤 **Dışa aktarma**: Ses miksajıyla birlikte WebM/MP4 (MediaRecorder) — geçişler, efektler ve animasyonlar dahil, sunucusuz

## Nasıl çalışıyor?

- Önizleme ve dışa aktarma tek bir `<canvas>` üzerinden çizilir; filtreler CSS filter, metinler canvas metni olarak işlenir.
- Dışa aktarma `canvas.captureStream()` + Web Audio miksajı + `MediaRecorder` ile gerçek zamanlı kayıttır; süre, proje süresi kadardır.
- Tarayıcının `MediaRecorder` desteğine göre WebM (VP9/VP8) ya da MP4 üretilir.

## Sınırlamalar

- Dışa aktarma gerçek zamanlıdır (5 dakikalık video ≈ 5 dakika sürer).
- Kodek desteği tarayıcıya bağlıdır; iOS Safari MP4, Chrome/Android WebM üretir.
- Projeler tarayıcının IndexedDB deposunda tutulur; tarayıcı verilerini/site verilerini silersen projeler de silinir ve başka cihazdan erişilemez.
