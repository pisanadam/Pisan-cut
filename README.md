# Pisan Cut 🎬

CapCut benzeri, **tek HTML dosyasında çalışan** mobil video editörü. Sunucu yok, kurulum yok, hesap yok — her şey tarayıcıda çalışır ve videolar cihazından dışarı çıkmaz.

## Kullanım

`index.html` dosyasını bir tarayıcıda aç, hepsi bu. GitHub Pages ile de yayınlayabilirsin:
Ayarlar → Pages → dalı seç → yayınla.

> En iyi deneyim için mobil Chrome / Safari önerilir. Masaüstünde de çalışır.

## Özellikler

- 🏠 **Ana ekran**: CapCut benzeri açılış menüsü, araç kısayolları ve proje listesi
- 🖥️ **Profesyonel Mod (aç/kapa)**: Ana menünün üstündeki anahtarla açılan masaüstü düzeni (DaVinci Resolve / Windows CapCut tarzı) — üstte menü çubuğu, solda dikey araç rayı, ortada büyük önizleme, sağda sabit "Özellikler" (inspector) paneli, altta tam genişlik zaman çizelgesi. Geniş ekran / yatay modda devreye girer, tercih kaydedilir
- 💾 **Otomatik kayıt**: Projeler medya dosyalarıyla birlikte IndexedDB'ye kaydedilir; sekmeyi kapatsan bile ana ekrandan geri açabilirsin (yeniden adlandır / sil dahil)
- 📹 **Çoklu klip**: Video ve fotoğraf ekle, sırala
- ✂️ **Kırp & Böl**: Klibi seçince çıkan kenar tutamaçlarını sürükleyerek videoyu kes, fotoğrafın süresini uzat (kesilen uçtaki kare canlı önizlenir); oynatma çubuğundan ikiye böl; ilk klip soldan kırpılınca zaman kaymaz — kesilen süre kadar başta siyah boşluk kalır (müzik/yazı senkronu korunur)
- 🔀 **Sıralama**: Klibe basılı tutup zaman çizelgesinde sürükleyerek kliplerin sırasını değiştir
- 🖼️ **Görünür çerçeve**: Önizlemede tuval kenarları ve boş alanlar gri gösterilir (en-boy oranı net seçilir); dışa aktarmada siyahtır
- ⇄ **Geçişler**: Klipler arasında Solma, Siyah/Beyaz, Kaydırma, Silme, Yakınlaşma — süre ayarlı; zaman çizelgesindeki sınır düğmesinden eklenir
- ✨ **128 Efekt (çoklu seçim)**: Aynı klipte 6 efekte kadar birleştirilebilir (örn. El Kamerası + Gren + Vinyet); dönüşümler birleşir, katmanlar sırayla çizilir. Arama + kategori sekmeli panel; emoji parçacık aileleri (kar, kalp, balon, kelebek, ateş…) × 4 yoğunluk, yağmur, gren, vinyet, sarsıntı, nabız, glitch, parıltı, tarama, konfeti, VHS, negatif, renk döngüsü, kamera hareketi (4 yön), flaşlar, ışık sızıntıları, bokeh, hız çizgileri; 39 hareket efekti: sallanma, el kamerası, deprem, zıplama, salıncak, bas vuruşu zoom'u (BPM'li), yörünge, süzülme, mikro titreme, dönme nabzı (yoğunluk kademeleriyle)
- ⇄ **119 Geçiş**: 17 renge karartma, 8 yönlü kaydırma/silme (+yumuşak sürümleri), bölünme, jaluzi, daire/kare/elmas/kalp/yıldız açılış-kapanışları, zoom/dönme, satranç, piksel çözülme, saat süpürmesi + **Ani ⚡ kategorisi**: editlerdeki vuruşlu kesimler — flaş kesim (4 renk), kamera savurma (4 yön), zoom vuruş, sekmeli zoom, sarsıntılı kesim, glitch kesim, RGB ayrışma, dönme vuruşu, bulanık kesim (seçilince süre otomatik ~0.3s)
- 🎨 **100+ Filtre**: 10 aile × 9 yoğunluk + 12 ton kaydırma; arama ve kategorilerle
- ▦ **108 Şablon**: Popüler edit müziği türleriyle (Phonk, Sigma, Drill, Lofi, Slowed, Synthwave…) hazır kurgu şablonları — seç, videolarını ekle; tempo kesimi, her kesimde dönüşümlü farklı geçişler (geçiş havuzu), filtre, efekt, başlık ve müzik otomatik uygulanır; birden fazla video/fotoğraf seçilebilir. "🎲 Otomatik Şablon Oluştur" ile rastgele yeni kombinasyonlar
- 🧪 **YZ Lab**: Upscale, Kare Üretici ve tek dokunuşla Otomatik Edit
- 🖼 **Bindirme (PiP)**: Video/fotoğrafı katman olarak üstüne ekle — sesi mikslenir, süresi, konumu ve **opaklığı** ayarlanır
- 🤏 **Dokunmatik dönüşüm**: Önce dokunup seç, sonra tek parmakla taşı, iki parmakla yakınlaştır/boyutlandır (yanlışlıkla kaydırmayı önler; ana klip zaman çizelgesinden seçilir); sürüklerken merkez mıknatısı (kılavuz çizgisiyle ortaya yapışma) ve panellerde "Tam Ortala / Yatay / Dikey" düğmeleri
- 🗂 **Katmanlar**: Üst üste binen öğelerde "öne getir / arkaya gönder" ile sıralama; birden çok bindirme ve müzik eklenebilir — zamanda çakışan çubuklar zaman çizelgesinde otomatik olarak ayrı katman satırlarına dizilir
- ↔️ **Çubuk sürükleme**: Zaman çizelgesinde metin/obje/bindirme çubuklarını ortadan taşı, uçlarından uzat/kısalt
- ⏩ **Hız**: 0.01x – 10x sürgüyle (logaritmik) + hazır değerler; "ses perdesini değiştir" aç/kapa
- 🔊 **Ses**: Klip başına ses seviyesi
- 🎨 **Filtreler**: Canlı, Sıcak, Soğuk, Siyah-Beyaz, Sepya, Retro, Dramatik
- 🎛️ **Ayarla**: Parlaklık, kontrast, doygunluk
- 🅣 **Animasyonlu metin**: Giriş animasyonları (Pop, Solma, Kayma, Zıplama, Dönme, Daktilo) + döngü hareketleri (Dalga, Gökkuşağı, Nabız, Süzülme, Titreme); sürükleyerek konumlandır
- 😀 **Bindirme objeler**: Emoji çıkartmaları, giriş animasyonu + sürekli hareket (süzülme, dönme, nabız…), boyut/süre ayarı, sürükleyerek taşıma
- 🌈 **Arka Plan kütüphanesi**: 32 düz renk arka plan — dokun, tüm kareyi kaplayan renk klibi eklenir (her orana uyar, süresi kenardan uzatılır); yazı/obje altına zemin ya da geçiş dolgusu için ideal
- 🎞️ **Stok Video kütüphanesi**: Açık kaynak / kamu malı videoları (Wikimedia Commons, İnternet Arşivi) ara, indir ve **filigransız** klip olarak ekle — indirilen video projeyle birlikte cihazına kaydedilir
- ⛶ **Tam ekran**: Ana menüdeki butonla uygulamayı tam ekrana al
- 🎵 **Müzik**: Birden çok parça ekle (oynatma çubuğundan başlar); çubuğunu sürükleyerek taşı/kırp, böl, sil, hızlandır (0.1x–10x), ses seviyesi, **bas güçlendirme** (low-shelf, 0–15 dB); proje süresi videonun bittiği andır: müzik daha uzunsa video sonunda otomatik kesilir (zaman göstergesi videonun süresini yazar). Kısa müziği video boyunca uzatmak için müzik panelindeki "🔁 Video sonuna kadar döngüle" düğmesini kullan
- 📚 **Müzik kütüphaneleri**: Cihazından eklemenin yanında 5 çevrimiçi kaynakta ara, dinle ve tek dokunuşla projeye ekle — 🎧 Phonk sekmesi hazır kategorilerle (Popüler, Drift, Brazilian, Agresif, Chill, Sigma) sekme açılır açılmaz popüler phonk parçalarını listeler; — İnternet Arşivi (archive.org), Openverse ve Wikimedia Commons tam şarkı verir; iTunes 30 sn önizleme verir (döngüleme ile uzatılabilir); eklenen parçalar projeyle birlikte cihazına kaydedilir
- ⚙️ **Ayarlar**: Ana ekranda sağ üstteki ⚙ düğmesinden (veya her ekranda "Pisan Cut" yanındaki **sürüm rozetine dokunarak**) açılır.
  - 🛠 **Geliştirici Modu**: Açıkken ⚙ üzerinde **hata sayacı rozeti** çıkar, hata oluştuğunda anında uyarı gösterilir (en fazla 4 sn'de bir) ve **cihaz raporu** (sürüm, çekirdek sayısı, ekran, GPU adı, WebCodecs desteği, UA) görüntülenip kopyalanabilir. Ayar tarayıcıda kalıcıdır.
  - 📋 **Logları Görüntüle**: Uygulama açıldığı andan itibaren tüm `console` kayıtları, yakalanmamış hatalar ve işlenmeyen promise hataları toplanır. Seviye süzgeci (**Tümü / Hata / Uyarı / Bilgi**), canlı güncelleme, aynı kaydın tekrarını birleştirme (×N), **Kopyala** (cihaz raporuyla birlikte) ve **Temizle**. Bellek için halka tampon: en fazla 600 kayıt tutulur.
  - ❗ **Sadece Hataları Göster**: Açıkken log ekranı doğrudan hata süzgeciyle açılır (bilgi/uyarı gizlenir).
- ↩️ **Geri al / Yinele**: PC'de Ctrl+Z geri alır, Ctrl+X (veya Ctrl+Y / Ctrl+Shift+Z) yineler; mobilde üst çubuktaki ↩ ↪ düğmeleri — 50 adıma kadar
- ⬛ **En-boy oranı**: 12 ön ayar (9:16, 16:9, 1:1, 4:5, 5:4, 3:4, 4:3, 2:3, 3:2, 21:9, 9:21, 2.35:1) **+ klavyeyle özel oran** — istediğin herhangi bir en:boy değerini girebilirsin (örn. sinema 21:9, klasik 4:3)
- 🎚️ **Dışa aktarma ayarları**: Format (**MP4** / WebM), çözünürlük (480p / 720p / 1080p / 2K β / 4K β **veya klavyeyle 120–4320 px özel kısa kenar**) ve kare hızı (5 / 10 / 15 / 20 / 24 / 30 / 60 / 90 β / 120 β **veya klavyeyle 1–240 özel fps**) seçimi, tahmini dosya boyutuyla; seçimler projeyle birlikte kaydedilir. MP4 varsayılandır (en uyumlu): H.264 + AAC ile paketlenir, cihaz desteklemezse otomatik WebM'e düşer. β işaretli seçenekler beta'dır — bazı telefonlarda stabil çalışmayabilir
- 🎮 **GPU Kullan (aç/kapa)**: Açıkken (varsayılan) ekran kartının **donanım video kodlayıcısı** (NVIDIA NVENC / Intel QuickSync / AMD AMF / Apple VideoToolbox) zorlanır ve her kare **ağır iki geçişli bir WebGL shader hattından** geçirilir: ayrılabilir Gauss bulanıklığı (geçiş başına 13 örnek) + unsharp mask (netlik) + ince detay. Bu, ekran kartının **shader/CUDA çekirdeklerini** gerçekten çalıştırır (yük çözünürlükle büyür) ve görüntüyü netleştirir. Kapalıyken yazılım (CPU) kodlayıcı. **Önemli:** CUDA çekirdekleri tarayıcıdan yalnızca shader ile sürülür; video **çözme (NVDEC)** ve **kodlama (NVENC)** ayrı sabit-işlev motorlarıdır. Görev Yöneticisi'nde kodlayıcı yükü **"Video Encode"**, shader geçişi **"3D"/Compute** motorunda görünür (varsayılan grafik değil). Güçlü kartlar (RTX 4060 gibi) tek video akışında %100'e ulaşmaz — darboğaz genelde video çözme/besleme aşamasıdır; **çözünürlük + fps + upscale artırınca GPU yükü belirgin artar**. Tanı satırında hangi GPU'nun devreye girdiği (ör. "GPU:donanım+WebGL (NVIDIA ...)") gösterilir. Yazılım (donanımsız/SwiftShader) GL algılanırsa geçiş otomatik atlanır. **Kodlayıcı seçimi:** GPU açıkken MP4 için önce **donanım kodlanabilen H.264** aranır (NVENC/QuickSync/AMF; H.264 seviyeleri 5.2/6.2'ye kadar denenir, böylece 4K/yüksek fps'te de donanım kodlayıcı seçilir). NVENC VP9 kodlamadığından, eski sürümlerde yüksek çözünürlükte H.264 yerine **yazılım VP9**'a düşülüp CPU'ya yükleniyordu — artık H.264 donanım yolu önceliklidir.
- 🔍 **Video Upscale (aç/kapa)**: Açıkken çıktı %50 büyütülüp yüksek kaliteli ölçekleme ile kodlanır; yazılar, çıkartmalar ve efektler yüksek çözünürlükte yeniden çizildiği için gerçekten daha keskin çıkar
- 🎞 **Kare Üretici (aç/kapa)**: 60/90/120 fps dışa aktarmada düşük fps'li kaynaklar için ara kareler harmanlanarak üretilir (echo frame blending) — hareket akıcılaşır; yalnızca 60 fps ve üstünde etkilidir
- 📤 **Hızlı render (CapCut tarzı)**: WebCodecs destekleyen tarayıcılarda video kare kare offline kodlanır, ses offline mikslenir — önizleme taksa bile çıktı her zaman akıcıdır ve çoğu cihazda gerçek zamandan hızlı biter. WebCodecs yoksa MediaRecorder ile gerçek zamanlı kayda düşer.
- ⚡ **Hızlı Mod (gerçek zamanlı)**: Dışa aktarma panelinden açılır; kare kare offline render yerine cihazın yerleşik donanım kaydedicisini kullanır (Safari/iPad'de doğrudan MP4). Safari/iPadOS'ta `<video>` kare kare sarma yavaş olduğu için orada çok daha hızlıdır (render ≈ video süresi).
- ⚡ **Akıcı önizleme**: Düzenleme sırasında canvas ekran çözünürlüğünde çalışır (dışa aktarmada tam çözünürlüğe geçer), kare yalnızca gerektiğinde yeniden çizilir

## Nasıl çalışıyor?

- Önizleme ve dışa aktarma tek bir `<canvas>` üzerinden çizilir; filtreler CSS filter, metinler canvas metni olarak işlenir.
- **Hızlı render**: her kare için videolar tam zamana sarılır, kare `VideoEncoder` ile kodlanır; ses `OfflineAudioContext` ile mikslenip `AudioEncoder` (Opus) ile **videoyla paralel** kodlanır ve dosya içindeki minimal Matroska/WebM muxer ile birleştirilir. Kare düşmesi mümkün değildir. Kodlayıcı önce cihazın **donanım kodlayıcısını** dener (telefonlarda en hızlı ve en stabil yol), yoksa yazılım "quality" moduna düşer.
- **Paralel seek hattı**: dışa aktarmada kareler tek tek sarılıp beklenmez; her klip için bir havuz gölge `<video>` elemanı tutulur ve gelecek kareler (çekirdek sayısına göre 3–8 hat) **aynı anda** sarılır. Böylece CPU çözücü çekirdekleri boş kalmaz, kodlayıcı bir kareyi işlerken sonraki kareler arka planda hazırlanır — donanım darboğaza kadar dolu kullanılır (seri sarmaya göre belirgin hızlanma). Geçiş ve PiP içeren kareler kendi elemanlarında seri işlenir (doğruluk için).
- WebCodecs olmayan tarayıcılarda `canvas.captureStream()` + `MediaRecorder` ile gerçek zamanlı kayda düşülür.

## Sınırlamalar

- Hızlı render WebCodecs gerektirir (Chrome/Edge/Android WebView 94+, Safari 16.4+ kısmi); yoksa dışa aktarma gerçek zamanlı sürer.
- MP4 çıktı H.264+AAC destekleyen cihazlarda üretilir (çoğu telefon/masaüstü); yoksa otomatik WebM'e düşer. Dosya içi MP4 muxer sıkıştırılmamış (tek mdat) ISO-BMFF üretir. iOS/iPadOS Opus'u MP4 içinde çalamadığından, bu cihazlarda AAC yoksa sesin gerçekten gelebilmesi için otomatik olarak gerçek zamanlı (native AAC) kayda geçilir.
- **iOS ses düzeltmesi (MP4/MOV demux + WebCodecs)**: Safari/WebKit'in `decodeAudioData`'sı **video kapsayıcısından** (MP4/MOV) ses çıkaramaz — Chrome çıkarır. Bu yüzden iPad/iPhone'da dışa aktarılan videonun sesi kayboluyordu. Artık `decodeAudioData` başarısız olursa, dosyanın ses izi **kendi MP4/MOV demux'umuzla** ayrıştırılıp (moov→trak→stbl: stsd/esds-ASC, stts, stsc, stsz, stco/co64) **WebCodecs `AudioDecoder`** ile çözülüyor ve AudioBuffer'a dönüştürülüyor. Medya IndexedDB'de bulunamazsa eleman kaynağından (`fetch`) çekilir; 48 kHz OfflineAudioContext reddedilirse 44.1 kHz'e düşülür.
- **Dışa aktarma tanısı**: "Hazır!" ekranında küçük bir tanı satırı gösterilir (kullanılan video/ses codec'i + zamanlama dökümü: kare başına seek/çizim/bekleme süresi ve yavaşlamanın kaçıncı karede başladığı). Satıra dokununca panoya kopyalanır — cihaza özel dışa aktarma sorunlarını ayıklamak için.
- Projeler tarayıcının IndexedDB deposunda tutulur; tarayıcı verilerini/site verilerini silersen projeler de silinir ve başka cihazdan erişilemez.
