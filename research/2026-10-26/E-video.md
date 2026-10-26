# E — Higgsfield Video Menüsü: Özellikler ve Modeller

**Araştırma tarihi:** 26 Ekim 2026
**Bağlam:** Türkiye'de çok markalı bir oto bakım/detailing ürünleri distribütörü. Instagram Reels, ürün tanıtım ve reklam videosu üretiliyor. En önemli kriter ürün etiketinin, logonun ve ambalajın doğru görünmesi.
**Yöntem:** higgsfield.ai sayfaları, /blog, /creator-hub/help-center ve site haritası (sitemap) okundu. Higgsfield MCP araçları çağrılmadı, ücretli üretim yapılmadı.

## İşaretler

| İşaret | Anlamı |
|---|---|
| **[doğrulanacak]** | Resmî kaynakta bulunamadı ya da kaynaklar birbiriyle çelişiyor. |
| **[üçüncü taraf]** | Bilgi Higgsfield dışı bir kaynaktan geliyor. |
| **[ön yüz kodu]** | higgsfield.ai'nin herkese açık JavaScript dosyalarından çıkarıldı. Resmî doküman değil, arayüz ayarlarını gösteriyor ve değişebilir. |
| **Öneri** | Bizim iş akışımız için yorum. Kaynakta geçmiyor. |

## Kredi bilgisi hakkında genel not

- Fiyatlar blog yazılarında verilen örnek fiyatlardır. Yazıların hepsi tarihlidir ve bazı araçlarda aynı iş için iki farklı fiyat geçiyor (ilgili bölümlerde ayrıca belirtildi).
- Blog yazıları dolar karşılığını genelde Plus planına göre hesaplıyor: $49 / 1.000 kredi, yani kredi başına yaklaşık $0,049.
- Help center'a göre kesin fiyat her üretimde Generate düğmesinin üzerinde yazıyor.
- Canvas, MCP, CLI, Supercomputer ve eklentilerden yapılan üretimler, Unlimited hakkı olsa bile krediden düşüyor. Kaynak: [ai-video-credits-explained](https://higgsfield.ai/blog/ai-video-credits-explained), [Canvas help](https://higgsfield.ai/creator-hub/help-center/tools/how-do-i-use-canvas).

---

# BÖLÜM 1 — Özellikler (Features)

## 1.1 3D Jutsu (3D sahne → video)

**URL:**
- Uygulama: https://higgsfield.ai/3d-jutsu (sayfa istemci tarafında yükleniyor, metin içeriği yok)
- Resmî tanıtım: https://higgsfield.ai/blog/higgsfield-3d-jutsu (5 Eyl 2026)

**Ne yapıyor:**
- Higgsfield'in yapay zekâ tabanlı 3D çalışma alanı.
- Bir prompt ya da referanstan düzenlenebilir bir 3D sahne kuruyor: nesneler, yerleşim, ışık, kameralar ve animasyon.
- Bu sahneden video üretiyor.
- Sahneyi Supercomputer üzerinde çalışan bir AI ajanı kuruyor.
- Amaç sahne blocking ve previz (ön görselleştirme). Sahneler hesapta "My Scenes" altında saklanıyor.

**Nasıl kullanılır:**
1. Sahneyi tarif eden bir metin prompt yaz. Varsa referans ekle (kendi yüklemelerin ya da önceki Higgsfield üretimleri).
2. Parametreleri seç:
   - **Model:** Ajanı yöneten LLM. "Auto" ücretsiz varsayılan.
   - **Duration:** Sahne süresi 1–60 sn, varsayılan 15 sn.
   - **Aspect ratio:** 16:9, 9:16, 1:1, 4:3, 3:4 veya 21:9.
3. Generate'e bas. Taslak sahne etkileşimli 3D görüntü alanına (viewport) gelir: sürükleyerek döndür, kaydırarak yakınlaştır, sağ tıkla sürükleyerek kaydır.
4. Sahneyi düzenle:
   - Primitifler: küre, küp, piramit.
   - 3 ışık tipi: sun, point, spot.
   - Kameralar, hazır kamera ayarları ve kamera yolu (trajectory) düzenleme.
   - Varlık kütüphanesi: hazır GLB modeller ve Mixamo karakterleri.
   - Sahne özellikleri: arka plan rengi, sahne çözünürlüğü, ışık yoğunluğu.
   - Playhead'li zaman çizelgesi.
   - Nesneleri taşı, döndür, ölçekle, çoğalt. Undo/redo ve revizyon geçmişi var.
5. Sohbet panelinden doğal dille talimat ver. Ajan için üç mod var:
   - "generate without asking": onay sormadan üretir.
   - "ask before generating": her üretimden önce sorar.
   - Ayrı bir "ask" modu: sahneye dokunmadan soruları yanıtlar.
6. Sahneyi dışa aktar ya da videoya gönder:
   - Export seçenekleri: animasyonlu MP4, tek kare (statik) ya da GLB. Boyut ve dosya büyüklüğü render öncesinde ayarlanıyor.
   - Video üretimi doğrudan aynı sohbetten isteniyor.
   - Blogdaki örnek iş akışı: gri proxy'lerle previz kur → previz'i video olarak render et → Soul 2.0 / Soul Cinema ile karakter ve mekân referansı üret → previz videosu ile referansları aynı sohbette birleştir.

**Ek özellikler:**
- GLB içe aktarılabiliyor ve animasyonu korunuyor.
- Ekip paylaşımı var: admin, collaborator ve viewer rolleri, ayrıca "link'e sahip herkes" erişimi.
- Aynı sahne katmanı Higgsfield Blender eklentisinde de çalışıyor.

**Ses:** Final video üretimindeki ses davranışı kaynakta tanımlanmamış **[doğrulanacak]**. Örnek prompt bir ses bölümü içeriyor, ama hangi modelin render ettiği belirtilmemiş.

**Kredi:**
- Ajan mesajları LLM'e göre ücretlendiriliyor. Auto ücretsiz.
- Örnek mesaj başı maliyetler: DeepSeek V4 Flash ~0,4 · Seed 2.1 Turbo ~1 · Gemini 3.5 Flash ~2 · Gemini 3.1 Pro ~3 · GPT 5.6 Sol ~7 · Claude Opus 5 ~8 · Claude Fable 5.1 ~11 · GPT 6 Astra ~17 kredi.
- Final video render maliyeti belirtilmemiş **[doğrulanacak]** (büyük olasılıkla seçilen video modelinin ücretiyle).

**Sınırlar:**
- Manuel düzenleme sınırlı: nesne taşıma, primitif/ışık ekleme, kamera kadrajı.
- Final görünüm yine bir üretken video modelinden geliyor. Previz'deki gri geometri yalnızca kamera ve davranış referansı olarak kullanılıyor.

**Öneri:**
- Ürünün doğru geometrisi (şişe, sprey başlığı, kova vb.) için elinizde GLB varsa, ya da ürün fotoğrafından GLB üretilebiliyorsa **[doğrulanacak]**, 3D Jutsu'ya import edip kamera yolunu (orbit, push-in, makro geçiş) burada kilitleyin.
- Previz MP4'ünü Seedance 2.5 veya Kling 4.0'a video referansı olarak, gerçek ürün fotoğraflarını da görsel referans olarak verin.
- Dikkat: final renderda etiketi model yeniden çizer. Geometri doğru kalsa bile etiket metni bozulabilir. Etiket kritik karelerde gerçek packshot'ı postta bindirmeyi (overlay) planlayın.
- En güvenli kullanım: 3D Jutsu'yu "kamera hareketi ve kompozisyon kilitleme" aracı olarak düşünün. Etiket doğruluğunu bundan beklemeyin.

---

## 1.2 Mixed Media

**URL:**
- Tanıtım: https://higgsfield.ai/mixed-media-intro
- Uygulama: https://higgsfield.ai/flow/mixed-media (ön yüz kodundaki katalog: "Transform videos with AI presets")

**Ne yapıyor:**
- Yüklenen videoya hazır görsel stiller (preset) uyguluyor: neon, doodle, kâğıt eskiz vb. 40+ estetik.
- "Otomatik rotoskop" ile kare kare maskeleme yapıyor.
- Sayfa başlığı: "Create complete 10-sec scenes".

**Nasıl kullanılır (sayfadaki adımlar):**
1. Videoyu yükle.
2. Preset seç.
3. Kare hızı (frame rate) ve çözünürlüğü seç.
4. Advanced settings (opsiyonel).
5. Sonucu al.

**Süre ve ses:**
- Sayfa "10 saniyelik sahne" diyor. Kesin girdi süresi limiti **[doğrulanacak]**.
- Ses davranışı **[doğrulanacak]**.

**Kredi:** Kaynakta yok **[doğrulanacak]**.

**Sınırlar:** Stilize bir efekt aracı; ürünün görünümü preset'e göre değişir.

**Öneri:**
- Ürün tanıtımında yalnızca arka plan ya da geçiş efektleri için kullanın. Hook ve trend Reels formatına uygun.
- Etiketin göründüğü karelerde stil, ürün yüzeyini de boyayabilir. Ürünün net göründüğü "packshot" anlarını bu efektin dışında tutun.

---

## 1.3 Edit Video (sahne / çekim / eleman düzenleme)

**URL'ler:**
- Ön yüz kodundaki keşif menüsünde "Edit Video" kartı → Kling Video Edit modeli (`kling-video-edit`), `/video-edit` rotası **[ön yüz kodu]**.
- Genel rehberler:
  - https://higgsfield.ai/blog/how-to-edit-videos-with-ai (24 Eki 2026)
  - https://higgsfield.ai/blog/edit-ai-video-without-regenerating (16 Eyl 2026)

**Ne yapıyor:**
- Var olan klibin (gerçek çekim veya AI üretimi) belirli bir öğesini değiştiriyor: karakter, ürün, kıyafet, arka plan, ışık. Geri kalanını korumayı hedefliyor.
- Ön yüz kodundaki asset düzenleme panelinde şu video seçenekleri görünüyor **[ön yüz kodu]**: "Change scene", "Relight", "Edit Color Palette", "Upscale".

**Higgsfield'in "hangi iş için hangi araç" tablosu (blog):**

| Değişecek şey | Önerilen araç |
|---|---|
| Ürün, kıyafet, aksesuar, karakter | Genjutsu Object Swap |
| Hareketi koruyup oyuncu/mekân değiştirme | Genjutsu Motion Transfer |
| İşaretlenmiş bir bölge ya da prompt'la lokal değişiklik | Seedance 2.5 Edit (prompt veya Draw to Edit; "Smart Clean Up" ile toz, kablo, nesne silme) |
| Işık yönü, rengi, yoğunluğu | Video Relight |

**Diğer düzenleme araçları (24 Eki 2026 blog):** Extend Video (Cinema Studio 4.0, sahneyi en fazla 30 sn'ye kadar uzatır), Reframe, Remove Background (MP4/MOV), SDR→HDR, FPS Boost, Depth Map, FLUX.3 Upscale.

**Girdi limitleri:**
- Genjutsu: referans video 4–30 sn, en fazla 30 referans görsel, çıktı en fazla 1080p.
- Genjutsu Lite (20 Eki 2026): 4–30 sn video, en fazla 10 referans görsel, 720p veya 1080p, standart Genjutsu fiyatının yaklaşık üçte biri.
- Seedance 2.5 Edit: en fazla 50 referans, en fazla 30 sn video, en fazla 1080p.
- Kling 4.0 Edit video: en fazla 5 klip (1 ana klip), her biri 3–30 sn, toplam en fazla 30 sn (bkz. Bölüm 2).

**Kredi (blog örnekleri):**

| Tarih | Araç | Ayar | Kredi |
|---|---|---|---|
| Eyl 2026 | Genjutsu Object Swap | 10 sn 1080p | 99 |
| Eyl 2026 | Genjutsu Motion Transfer | 10 sn 1080p | 99 |
| Eyl 2026 | Seedance 2.5 Edit | 10 sn 1080p | 90 |
| 24 Eki 2026 | Genjutsu | 15 sn 720p | 105 |
| 24 Eki 2026 | Genjutsu Lite | 15 sn 720p | 32 |
| 24 Eki 2026 | Extend | +5 sn 720p | 35 |
| 24 Eki 2026 | Reframe | 15 sn 720p | 71 |
| 24 Eki 2026 | Remove Background | 15 sn 720p | 3,94 |
| 24 Eki 2026 | Relight | 15 sn 720p | 42 |
| 24 Eki 2026 | SDR→HDR | 15 sn 720p | 43 |
| 24 Eki 2026 | FPS Boost | 15 sn 720p | 58 |
| 24 Eki 2026 | Depth Map | 15 sn 720p | 21 |
| 24 Eki 2026 | FLUX.3 Upscale | 15 sn 720p | 14 |

Kling Video Edit'in kredisi kaynakta yok **[doğrulanacak]**.

**Sınırlar (blogun kendi listesi):**
- Karakterin aksiyonunu veya performansını değiştirmek yerel düzenlemeyle olmaz.
- Süre, tempo ya da çekim yapısını değiştirmek de olmaz.
- Boyutu veya şekli çok farklı bir nesneyle değiştirmek uyumu bozar.
- Yeni temas veya örtüşme (oklüzyon) gerektiren etkileşimler (ör. elin olmayan bir şeyi alması) eklenemez.
- Aynı anda çok sayıda bağlantılı öğe değişiyorsa tam yeniden üretim daha iyi sonuç verir.
- FAQ uyarıları: Ürün eldeyse veya hızlı hareket ediyorsa değiştirilen ürün bozulabilir. Bulanık videoda yüz, metin ve ince doku yanlış yeniden kurulabilir.

**Öneri:**
- Gerçek çekimdeki ürünü başka bir SKU ile değiştirmek (aynı şişe formu, farklı etiket) için Genjutsu Object Swap / Lite veya Seedance 2.5 Edit uygun.
- Referans görseli, kaynak videodaki ürünle aynı açıdan çekin. Ürün boyutu ve şekli aynı olsun. Blog da açı uyumunu öneriyor.
- Etiket metni yine modelce yeniden çiziliyor. Her sonucu yavaş oynatıp etiketi kare kare kontrol edin.
- En sağlam yol: **gerçek ürün çekimini düzenlemeden koruyup** yalnızca arka planı, ışığı veya rengi değiştirmek (Relight, Color Palette, Remove Background). Ürün pikselleri ne kadar az değişirse etiket o kadar güvende kalır.

---

## 1.4 Video Upscale (ve FLUX.3 Upscale)

**URL:**
- Uygulama: https://higgsfield.ai/upscale
- Tanıtım: https://higgsfield.ai/ai-video-upscaler
- Help: https://higgsfield.ai/creator-hub/help-center/troubleshooting/my-video-upscale-is-stuck-or-failed-what-should-i-do (1 Ağu 2026)

**Ne yapıyor:**
- Videoyu 1080p, 2K veya 4K'ya çıkarıyor.
- Ek seçenekler: preset'ler (AI clip, UGC/telefon, series, old film), en fazla 60 fps, kare enterpolasyonu (FPS Boost / Topaz), Video Deflicker.

**Motorlar (kaynaklara göre değişiyor):**
- **Help (1 Ağu 2026), video için iki model:**
  - ByteDance Upscale: "yüksek sadakat, 8K'ya kadar", standard/pro sürümleri var.
  - Topaz Video: difüzyon tabanlı, "yaratıcı detay ekler".
- **Landing sayfası:** ByteDance ve Topaz, "4K'ya kadar".
- **FLUX.3 Upscale (24 Eki 2026 blog):**
  - 1080p, 2K veya 4K. Hareketi ve sesi senkron tutacak şekilde tasarlanmış.
  - "precise" modu kaynağa yakın kalıyor.
  - "creative" modu detay ekliyor ve opsiyonel prompt alıyor.
  - Katalogdaki adı: "Flux 3.0 Video Upscale — Up to 4K".
- Kaynaklar arasındaki 8K / 4K farkı **[doğrulanacak]**.

**Nasıl kullanılır:**
- Explore → Video → Upscale yolunu izle, ya da Assets'te herhangi bir videoyu açıp Upscale'i seç.
- Model ve Scale factor'u seç. Advanced settings'te ek seçenekler var. Kredi, Upscale düğmesinin üzerinde güncelleniyor.
- Süre: genelde 1–5 dakika. 5 dakikayı geçerse iptal edip yeniden dene. Başarısız upscale'in kredisi otomatik iade ediliyor.
- Format önerisi: MP4 (H.264).

**Kredi:** FLUX.3 Upscale 15 sn 720p kaynak için 14 kredi (24 Eki blog). Diğer motorlar için tablo yok **[doğrulanacak]**.

**Sınırlar (help):**
- Çok düşük çözünürlüklü ya da aşırı sıkıştırılmış kaynak başarısız olabilir.
- Help açıkça uyarıyor: difüzyon tabanlı Topaz Video'yu **ürün çekimlerinde, metin ağırlıklı görsellerde ve onaylanmış işlerde kullanmayın**.

**Öneri:**
- Etiket ve logo içeren ürün videolarında **ByteDance Upscale** veya **FLUX.3 Upscale "precise"** kullanın.
- Topaz Video ve FLUX.3 "creative" kullanmayın; etikete hayalî detay ekleyebilir.
- Upscale her zaman en son adım olsun (blog önerisi).

---

## 1.5 Higgsfield Reframe

**URL:**
- Tanıtım: https://higgsfield.ai/ai-video-reframer
- Help'teki yol: higgsfield.ai → Edit → Reframe. Ön yüz kodunda mobil rotası `/mobile/video/reframe`.

**Ne yapıyor:**
- Videoyu yeni bir en-boy oranına uyarlıyor. Kırpmak yerine eksik alanı AI ile **yeniden üretiyor** (generatif genişletme), böylece kenardaki kişiler kadraj dışında kalmıyor.

**Nasıl kullanılır:**
1. Klibi yükle. Opsiyonel olarak 4 referans görsel ekle.
2. Oran seç: 9:16, 16:9, 4:3, 3:4, 21:9 veya 1:1. Model özneleri otomatik kilitliyor.
3. Generate et ve indir.

**Limitler:** FAQ'ya göre en fazla 1 dakikalık video, her çözünürlük kabul ediliyor, çıktıda filigran yok.

**Ses:** Belirtilmemiş **[doğrulanacak]**.

**Kredi:** 15 sn 720p için 71 kredi (24 Eki 2026 blog).

**Eklenti versiyonu:** Adobe ve DaVinci eklenti sayfaları Reframe'i "smart subject tracking ile kırpma" olarak tarif ediyor **[üçüncü taraf özetinden; eklenti sayfaları ayrıca okunmadı — doğrulanacak]**.

**Öneri:**
- Yatay çekimi Reels'e (9:16) çevirmek için ideal.
- Risk: genişletilen alanlar üretiliyor. Ürün kadrajın kenarındaysa, ürünün bir kısmı (etiketin yarısı vb.) AI tarafından "tamamlanabilir".
- Ürünü merkezde çekin ya da sonuçta etiketin kenara düşen kısmını kontrol edin. Mümkünse ürünün tamamının zaten kadrajda olduğu çekimleri reframe edin.

---

## 1.6 Change Color Palette (video)

**URL:**
- Tanıtım: https://higgsfield.ai/blog/video-relight-color-palette-higgsfield (20 Ağu 2026)
- Uygulama: ön yüz kodundaki uygulama kimliği `video-rehex`, adı "Color Palette", açıklaması "Apply cinematic color palettes or create your own from any image". Olası URL `/apps/video-rehex` **[doğrulanacak]**.
- Asset panelindeki adı "Edit Color Palette" **[ön yüz kodu]**.

**Ne yapıyor:**
- Var olan videoya renk düzenlemesi (color grading) uyguluyor. Çekimin kendisine dokunmuyor.
- 50+ preset var: Film Colors, Black Gloss, Candy Pink, Lime Jam, Nostalgic Blue, Soft Palette, Overtime, Crimson Vigi vb.
- Bir referans görselden palet çıkarılabiliyor. Özel (custom) grade da yapılabiliyor.

**Nasıl kullanılır:** Color Palette'i aç → klibi yükle → preset seç ya da custom grade/referans görsel ver → Generate → sonucu incele.

**Kredi:** 15 sn klip için 135 kredi ($6,75) (20 Ağu 2026 blog).

**Sınırlar:** Süre ve çözünürlük limitleri belirtilmemiş **[doğrulanacak]**.

**Not:** Ayrıca ücretsiz bir "Color grading" uygulaması var, ama bu yalnızca **görsel** için (PNG/JPG/WebP): https://higgsfield.ai/apps/color-grading

**Öneri:**
- Farklı günlerde çekilmiş ürün videolarını aynı marka görünümünde birleştirmek için kullanın.
- Dikkat: etiketteki marka renkleri (ör. kırmızı/sarı logo) de renklendirmeden etkilenir. Güçlü stilize preset'ler marka rengini kaydırabilir.
- Hafif preset'ler (Film Colors, Soft Palette) tercih edin. Marka renk kodlarını referans görselden vermek **[doğrulanacak]** daha güvenli olabilir.

---

## 1.7 Relight (video)

**URL:**
- Blog: https://higgsfield.ai/blog/video-relight-color-palette-higgsfield
- Uygulama kimliği `video-relight`, açıklaması "Change the lighting in any video while keeping every detail natural" **[ön yüz kodu]**.
- Not: https://higgsfield.ai/apps/relight **görsel** relight sayfası.

**Ne yapıyor:**
- Var olan videonun ışığını değiştiriyor. Kompozisyon ve hareketi koruyor.
- FAQ: "Işığı mevcut görüntünün üzerine yeniden render eder; hareket, kadraj ve kompozisyon kaynaktaki gibi kalır."

**Nasıl kullanılır:**
1. Klibi yükle.
2. Preset seç: Practicals, Silhouette, Contre-jour, Soft Cross, Window, Overhead Fall ya da Auto.
3. Ya da custom ışık kur: renk, parlaklık, diffuse ve açı. Tek geçişte en fazla 2 özel ışık. Işık prompt'la da tarif edilebiliyor.
4. Generate → incele → gerekirse ayarları değiştirip tekrar çalıştır.

**Kredi (çelişkili):**
- 20 Ağu 2026 blog: 15 sn klip için 135 kredi ($6,75).
- 24 Eki 2026 blog: 15 sn 720p için 42 kredi ($2,06).
- Fark muhtemelen çözünürlükten ya da fiyat güncellemesinden kaynaklanıyor **[doğrulanacak]**.

**Sınırlar:** Süre ve çözünürlük limitleri belirtilmemiş **[doğrulanacak]**.

**Öneri:**
- Atölye ya da garaj çekimlerini "stüdyo" ışığına çekmek, parlak boya veya cila yansımalarını dramatize etmek (Contre-jour, Soft Cross) için uygun.
- Ürünü yeniden çizmediği iddia edildiği için etiket riski düşük. Yine de yansıma ve parlama etiketi okunmaz hâle getirebilir; kontrol edin.

---

## 1.8 Lipsync Studio

**URL:**
- Uygulama: https://higgsfield.ai/lipsync-studio
- Help: https://higgsfield.ai/creator-hub/help-center/ai-models/how-do-i-use-lipsync-voiceover-and-aspect-ratios
- Blog: https://higgsfield.ai/blog/make-ai-lipsync-videos (7 Tem 2026)

**Ne yapıyor:** Bir görselden ya da videodan konuşan klip ("Create Talking Clips") üretiyor.

**Nasıl kullanılır:**
1. Video → Lipsync Studio'yu aç.
2. Karakter görseli ya da videosu yükle.
3. "Audio text" alanına metni yaz ya da sesi üret.
4. Model seç. Sahne şablonu seç: General, Selfie, Podcast, Car Talking vb.
5. Generate.

**Modeller (help tablosu):**

| Model | Girdi | Not |
|---|---|---|
| Google Veo 3.1 | görsel → video | |
| Kling 2.6 Lipsync | görsel → video | en fazla 1080p, sesli |
| Wan 2.5 Speak | görsel → video | 480p–1080p |
| Kling Avatars 2.0 | görsel → video | |
| Higgsfield Speak 2.0 | görsel → video | |
| Infinite Talk | görsel → video | uzun form |
| Kling Lipsync | video → video | |
| Sync Lipsync 3 | video → video | en fazla 4K |

Blog "10 model" diyor; help tablosunda 8 model var.

**Ses ve dil:**
- Ses üretimi, ses değiştirme ve çeviri (18 dil) Audio bölümünde.
- Ses klonlama (MP3/WAV) yalnızca kendi sesiniz ya da izinli bir ses için.

**Kredi:**
- Blog: "Veo 3 — 1080p klip başına 58 kredi".
- Starter yaklaşık $9 / 120 kredi ≈ 20 kısa Kling 2.6 LipSync klibi.
- Plus $49 / 1.000 kredi ≈ 100 Kling 2.6 klibi ya da 15–20 Veo 3 klibi.

**Sınırlar (blog):**
- Aynı karede çok konuşmacı hatalı oluyor.
- 30 sn üzerinde jest tekrarı görülüyor.
- Profilden ya da yüzü kapalı kaynakta kalite düşüyor.
- Blog "video-to-video dublaj yok" diyor, help tablosunda ise video→video modeller var. Bu çelişki **[doğrulanacak]**.

**Öneri:**
- Marka sözcüsü veya ustanın kısa ürün anlatımı (Türkçe) için kullanılabilir.
- Türkçe destek model bazında **[doğrulanacak]**. Audio Translate'in 18 dili arasında Türkçe olup olmadığı listelenmemiş.
- Ürünü konuşan kişinin elinde göstermek etiket bozulma riskini artırır. Ürünü sabit packshot olarak ayrı keserek kullanın.

---

## 1.9 Draw to Video

**URL:**
- Ön yüz kodu: `/draw?type=video` (flow rotası `/flow/draw`), kart açıklaması "Sketch turns into a cinema", "top choice" rozetli **[ön yüz kodu]**.
- Eski genel sayfa: https://higgsfield.ai/create/draw-to-video (istemci tarafında yükleniyor, başlığı "Draw-to-Video: Animate Your Sketches with AI").

**Ne yapıyor:** Görselin üzerine çizilen oklar, kısa etiketler ve kutularla hareketi yönetiyor. Prompt yazmadan videoyu yönlendirmeye yarıyor.

**Nasıl kullanılır [üçüncü taraf]** (Higgsfield'in Ağu 2025 tarihli rehberinin özetleri; o tarihli resmî blog bağlantısı artık 404):
1. Görsel yükle ya da Soul ile üret.
2. Kısa eylem etiketleri ("Man walks"), yön okları, opsiyonel sıra numaraları ve odak kutusu ekle. 2–3 eylemle sınırla.
3. Opsiyonel "Add Image" ile ürün ya da nesne ekle (1–2 önerilir, en fazla 3–4).
4. Modeli seç (o tarihte: Veo 3 / Hailuo 02 / Seedance; Seedance görsel eklemeyi desteklemiyordu). Generate.

**Güncel model listesi:**
- Ön yüz kodunda `veo3_draw`, `seedance_draw`, `minimax_hailuo_draw` iş tipleri görünüyor **[ön yüz kodu]**.
- Veo 3.1 rehberi (14 Eki 2025) "Draw-to-Video" modunu Veo 3.1 ile anıyor.
- Güncel liste **[doğrulanacak]**.

**Süre, çözünürlük, ses, kredi:** Seçilen modele bağlı **[doğrulanacak]**.

**Öneri:**
- Ürün kompozisyonu (şişe sabit, köpük soldan sağa akar, mikrofiber bez yukarı kalkar gibi) basit yön okuyla verilebilir.
- "Add Image" ile ürün yerleştirme etiket doğruluğu açısından risklidir. Ürün görselini yüksek çözünürlükte ve doğru ölçekte koyun, sonucu kontrol edin.

---

## 1.10 Draw to Edit

**URL:** Ön yüz kodu: `/draw?type=image`, kart açıklaması "From sketch to picture", model Nano Banana **[ön yüz kodu]**. Bu sürüm **görsel** düzenleme.

**Video bağlamında:**
- Seedance 2.5 Edit içinde "Draw to Edit" var: karede değişecek bölge işaretlenip içine ne olacağı yazılıyor ([edit-ai-video-without-regenerating](https://higgsfield.ai/blog/edit-ai-video-without-regenerating)).
- Adobe eklentilerinde de "Draw to Edit" (bölge işaretleme) ve "Edit Video" (prompt'la değişiklik) var: After Effects ve Premiere Pro.

**Limitler:** Seedance 2.5 Edit için video en fazla 30 sn, en fazla 50 referans, en fazla 1080p.

**Kredi:** Seedance 2.5 Edit 10 sn 1080p = 90 kredi (Eyl 2026).

**Öneri:**
- Video içindeki küçük bir hatayı (arka plandaki yabancı marka, kablo, toz) bölge işaretleyip temizlemek için ideal. Smart Clean Up da bu işe yarıyor.
- Etiketin olduğu bölgeyi işaretlemeyin. İşaretlenen alan yeniden çiziliyor.

---

## 1.11 Canvas (video bağlamı, kısa)

**URL:**
- https://higgsfield.ai/canvas
- Tanıtım: https://higgsfield.ai/canvas-intro
- Help: https://higgsfield.ai/creator-hub/help-center/tools/how-do-i-use-canvas

**Ne yapıyor:** Düğüm (node) tabanlı sonsuz bir pano. Prompt → görsel → video → edit zinciri kuruluyor, modeller paralel çalıştırılıp karşılaştırılıyor, şablon olarak kaydediliyor ve ekipçe canlı düzenleniyor.

**Video için önemli notlar:**
- Seedance düğümleri bağlı referans görselle çalışıyor, ama referansın rolü prompt'un başında açıkça yazılmalı.
- Kling düğümleri bağlı görseli **başlangıç karesi** olarak alıyor. Karakter ya da eleman referansı için önce element oluşturulup prompt'ta `@element-name` ile çağrılmalı.

**Kredi:** Düğüm kurmak ücretsiz, yalnızca üretimde kredi düşüyor. **Unlimited Canvas'ta geçerli değil.**

**Öneri:**
- Her ürün için "ürün fotoğrafı → ürün packshot görseli → 3 farklı video modeli" şablonu kurup modelleri yan yana karşılaştırın; etiket doğruluğunda en iyi modeli seçin.
- Unlimited planınız varsa üretimi web uygulamasında yapın, Canvas'ta değil.

---

# BÖLÜM 2 — Modeller

Video menüsündeki modeller "Video → Create Video → Model" yolundan seçiliyor (Kling 4.0 blogunda böyle tarif ediliyor).

## 2.1 Karşılaştırma tablosu

Kısaltmalar: t2v = metinden video, i2v = görselden video, ref = referans girdileri, ilk/son kare = start/end frame, edit = var olan videoyu düzenleme.

| Model | Güçlü yanı (kaynağa göre) | Max süre | Çözünürlük | Ses | Girdi türleri | URL |
|---|---|---|---|---|---|---|
| **Seedance 2.5** | Bölge düzeyinde düzenleme, 50 referansla karakter/ürün/mekân kilidi, Seedance 2.0'a göre ~%20 daha iyi prompt uyumu; era/genre/ışık/lens seçicileri | 30 sn | Model 480p / 720p / 1080p üretiyor; 4K "upscale" ile. Tanıtım sayfasında hem "native 1080p" hem "native 4K" geçiyor **[doğrulanacak]** | Var (ambiyans, foley, müzik aynı geçişte) | t2v, i2v (opsiyonel görsel), en fazla 50 görsel/klip referansı, motion control, edit (Seedance 2.5 Edit / Draw to Edit / Smart Clean Up). Ön yüz kodunda draft ve extend modları da görünüyor **[ön yüz kodu]**. Oran 9:16 ile 21:9 arası | https://higgsfield.ai/seedance/2.5 · [blog](https://higgsfield.ai/blog/seedance-2-5-on-higgsfield-2026) |
| **Kling 4.0** | Hızlı aksiyonda (spor, dövüş) daha stabil hareket ve kamera; karakter tutarlılığı; ekranda 9 dilde metin, emoji ve **logo** | 3–30 sn | Blog: 720p / 1080p. Tanıtım sayfası: "4K, 10-bit HDR (1080p ve 4K'da)" **[doğrulanacak]**. Kling 4.0 Flash: 720p taslak | Var (stereo, iki kanal; çok dilli konuşma) | t2v, i2v, ilk/son kare, en fazla 10 keyframe, Omni Reference (en fazla 15: 10 görsel + 5 video, 7 subject), edit (en fazla 5 klip, her biri 3–30 sn, toplam ≤30 sn), Creative Recreation. Oran Auto / 21:9 / 16:9 / 9:16 / 1:1. Prompt en fazla 8.000 token | [blog](https://higgsfield.ai/blog/kling-4-0-on-higgsfield) · https://higgsfield.ai/kling-4-0-intro |
| **Kling Motion Control** (3.0 ve 2.6) | Referans videodaki hareket, mimik ve temponun karakter görseline kare kare aktarımı; 3.0'da daha iyi yüz tutarlılığı | 3.0: "30 saniyeye kadar" (katalog açıklaması) **[ön yüz kodu]** | 720p / 1080p | **[doğrulanacak]** | 1 karakter görseli (zorunlu) + 1 hareket videosu (zorunlu) + opsiyonel prompt; "scene source" (arka plan videodan mı görselden mi); yön (orientation) ayarı | [blog](https://higgsfield.ai/blog/kling-motion-control-3) · `/video-edit?model=kling-3-motion-control` |
| **Kling 3.0 Omni Edit** | Var olan videoyu referans görsellerle düzenleme | **[doğrulanacak]** | **[doğrulanacak]** | **[doğrulanacak]** | 1 video (zorunlu) + en fazla 4 görsel; oran 1:1 / 16:9 / 9:16 **[ön yüz kodu]** | Resmî sayfa bulunamadı **[doğrulanacak]** |
| **Gemini Omni Flash 1.1** | Sohbet tarzı çok turlu düzenleme; görsel + metin + video + ses aynı prompt'ta; 1.1 önceki 10 sn'yi okuyup 10'ar saniyelik adımlarla uzatıyor; başlangıç ve bitiş karesi | Blog: 10 sn / üretim. Sayfa: varsayılan 8 sn, devam (continuation) ile 60 sn'ye kadar **[doğrulanacak]** | Sayfa ve blog: native 720p, 24 fps; 1080p upscale son işlem olarak. Sayfada "4K master" ibaresi de var **[doğrulanacak]** | Var (senkron ses; 11 dilde konuşma, lipsync) | t2v, i2v, en fazla 7 referans görsel, video girdi (sayfada hem "30 sn'ye kadar gerçek çekim" hem "60 sn'ye kadar" geçiyor **[doğrulanacak]**), ses girdisi (MP3/WAV ≤30 sn), eskiz, ilk/son kare, extend, edit. Çıktı oranları 16:9 / 9:16 / 1:1 / 4:5. Her çıktıda SynthID ve C2PA damgası var | https://higgsfield.ai/gemini-omni-flash · [blog](https://higgsfield.ai/blog/gemini-omni-flash-vfx-video-editing) |
| **FLUX.3 Video** | Black Forest Labs'in ilk video modeli (erken erişim); hareket hâlindeki tipografi okunur kalıyor; çok dilli diyalog ve lipsync | 5–20 sn | 720p / 1080p | Opsiyonel (açılıp kapatılabiliyor) | t2v, i2v, video devamı (continuation), en fazla 10 referans kare, ilk/son kare, görsel/video/ses referansları | [blog](https://higgsfield.ai/blog/flux-3-higgsfield) · https://higgsfield.ai/flux-3 |
| **FLUX.3 Upscale** | Kaynağa sadık "precise" mod ya da detay ekleyen "creative" mod (prompt alıyor); hareket ve ses senkronu korunuyor | Kaynak süresi (limit **[doğrulanacak]**) | 1080p / 2K / 4K | Sesi koruyor | Video (upscale) | https://higgsfield.ai/upscale · [blog](https://higgsfield.ai/blog/how-to-edit-videos-with-ai) |
| **MiniMax H3** (Hailuo 3.0) | Çok tür referansı tek üretimde birleştirme; **okunur ambalaj etiketi, altyazı ve marka işaretleri** (sayfa iddiası); talimatla düzenleme; fiziğe duyarlı hareket | 15 sn | 2K, 24 fps | Var (native stereo: diyalog, efekt, ambiyans) | t2v, i2v, en fazla 9 görsel + 3 video + 3 ses referansı, ilk/son kare, talimatla düzenleme. Oran 21:9 / 16:9 / 4:3 / 1:1 / 3:4 / 9:16 / adaptive. Ön yüz kodunda ayrıca "MiniMax H3 Max" var (480p / 768p) **[ön yüz kodu]** | https://higgsfield.ai/minimax/h3 · [blog](https://higgsfield.ai/blog/minimax-h3-higgsfield) |
| **Minimax Hailuo 2.3** | Fizik, dönüşüm (transformation) efektleri, anime; blog "logo ve ekrandaki metin hareket boyunca keskin kalır" diyor; 70+ preset; Fast ve Standard modları | 6 veya 10 sn (H3 bloguna göre 1080p'de en fazla 6 sn) | 768p / 1080p | Yok (H3 bloguna göre sessiz) | i2v (görsel zorunlu) + opsiyonel prompt + preset; oran girdi görseliyle aynı | [blog](https://higgsfield.ai/blog/Minimax-Hailuo-2.3-A-Creative-Guide) · https://higgsfield.ai/minimax |
| **Wan 3.0** | Tek prompt'tan en fazla 6 bağlantılı çekim (kesmeler hazır); kesmeler arasında kimlik kilidi; "markalı çekim detaylarını doğru tutan" en fazla 12 referans | 30 sn | **[doğrulanacak]** (ön yüz kodunda 480p / 720p seçenekleri ve "Wan 3.0 Prime" varyantı görünüyor **[ön yüz kodu]**) | Var (diyalog, ambiyans, efekt aynı geçişte) | t2v, en fazla 12 referans (karakter, ürün, mekân, stil). Katalog: "All-in-one reference video with sound, up to 30s" | https://higgsfield.ai/wan-3-0 |
| **Grok Imagine 1.5** | Tek başlangıç karesini sadık biçimde canlandırma (detay ve ışık korunuyor); kamera, atmosfer, fizik | 2–15 sn | 480p / 720p | Var (katalog: "synchronized audio"; FAQ "sound direction" diyor) | i2v (1 başlangıç karesi + prompt; prompt en fazla 2.500 karakter **[ön yüz kodu]**). Oran 16:9 / 9:16 / 4:3 / 3:4 / 1:1 / 3:2 / 2:3 **[ön yüz kodu]** | https://higgsfield.ai/grok-imagine-1.5 |
| **Grok Imagine 1.5 Lite** | "Fast, affordable videos from text or an image" (katalog) | **[doğrulanacak]** | **[doğrulanacak]** | **[doğrulanacak]** | t2v, i2v (katalog); oranlar 1.5 ile aynı **[ön yüz kodu]** | Resmî sayfa bulunamadı |
| **Google Veo 3.1** | Yüksek sadakat, native ses, diyalog ve lipsync (Standard); 1–3 görselle özne tutarlılığı | 4 / 6 / 8 sn | 720p / 1080p, 24 fps. Gemini Omni blogundaki karşılaştırma tablosu "4K" diyor **[doğrulanacak]** | Var | Standard: t2v + 1–3 referans görsel. Fast: t2v + ilk/son kare. Oran 16:9 / 9:16. Ön yüz kodunda ayrıca "Veo 3.1 Lite" var (oran auto / 16:9 / 9:16) **[ön yüz kodu]** | https://higgsfield.ai/veo3.1 |
| **HappyHorse** | Resmî Higgsfield açıklaması bulunamadı. [üçüncü taraf]: Alibaba modeli; 1.0 sürümü 1080p, sesli t2v/i2v, 3–15 sn (fal.ai) | [üçüncü taraf] 3–15 sn (1.0) **[doğrulanacak]** | **[doğrulanacak]** | [üçüncü taraf] var **[doğrulanacak]** | Ön yüz kodu: opsiyonel 1 başlangıç karesi, prompt en fazla 4.000 karakter, oran 16:9 / 9:16 / 1:1 / 4:3 / 3:4; resolution ve duration parametreleri var **[ön yüz kodu]** | Resmî sayfa yok; Video model listesinde görünüyor |
| **Higgsfield DOP** | Higgsfield'in kendi i2v modeli; sinematografiye duyarlı; preset sistemi (kamera hareketleri, VFX efektleri, Mix ile preset birleştirme) | 3 veya 5 sn | **[doğrulanacak]** | **[doğrulanacak]** | Yalnızca i2v: keyframe görsel zorunlu (PNG/JPG), preset, prompt (Enhance açılabiliyor), seed, steps. Model seçicide "Higgsfield Standard" olarak görünüyor | [help](https://higgsfield.ai/creator-hub/help-center/ai-models/how-do-i-use-dop) |

## 2.2 Model kredi bilgileri (yalnızca kaynakta olanlar)

**Seedance 2.5** (iki farklı fiyat geçiyor, fark **[doğrulanacak]**):
- 6 Ağu 2026 blogu, 10 sn: 480p 30 kredi · 720p 70 kredi · 1080p 120 kredi.
- 20 Eki 2026 fiyat blogu, 8 sn: 480p 24 kredi · 720p 56 kredi · 1080p 128 kredi.
- 20 Eki blogu: Seedance 2.5 Starter planda yok, Plus ($49) ve üstünde var.
- [Fiyat blogu](https://higgsfield.ai/blog/seedance-2-5-pricing-2026)

**Kling 4.0:**
- 720p: 5 sn 25 kredi · 30 sn 150 kredi.
- 1080p: 5 sn 37,5 kredi · 30 sn 225 kredi.

**FLUX.3 Video:**
- 5 sn: 720p 27,5 kredi · 1080p 45 kredi.
- 20 sn: 720p 110 kredi · 1080p 180 kredi.

**MiniMax H3 (2K):** 5 sn 20 kredi · 10 sn 40 kredi · 15 sn 60 kredi.

**Gemini Omni Flash:** Blogda yalnızca dolar cinsinden yaklaşık "~$0,15/sn (720p)" geçiyor. Kredi tablosu yok.

**Veo 3.1:**
- Gemini blogunun karşılaştırmasında "~$0,35/sn".
- Lipsync blogunda "Veo 3 — 1080p klip başına 58 kredi" (Veo 3, 3.1 değil).
- Doğrudan kredi tablosu yok **[doğrulanacak]**.

**Kredisi kaynakta olmayanlar [doğrulanacak]:** Kling Motion Control, Kling 3.0 Omni Edit, Grok 1.5 / 1.5 Lite, Hailuo 2.3, Wan 3.0, HappyHorse, DOP. DOP help'i yalnızca "standart oranlar, Generate düğmesinde gösterilir" diyor.

## 2.3 Model notları ve sınırlar

**Seedance 2.5**
- Görünüm seçicileri: era (1960'lar–2020'ler), genre, Soul Hex Engine (hex kodla palet kilidi), lighting, lens/gövde, emotional control.
- Higgsfield içinde Cinema Studio ve Soul ID ile birlikte kullanılabiliyor.
- Unlimited kampanyası: 33 gün Seedance 2.5 (Ağu). Ekim'de "Scale planında 720p'de unlimited" ilan ediliyor. Unlimited anahtarı model menüsünde açık olmalı.

**Kling 4.0**
- Mod sekmeleri: References / Frames / Edit video.
- Ekim 2026'dan önceki bir karşılaştırma blogu ([higgsfield-vs-kling-2026](https://higgsfield.ai/blog/higgsfield-vs-kling-2026)) "Kling 4.0 henüz Higgsfield'de değil" diyordu. 20 Eki 2026 tarihli blog ve tanıtım sayfası artık mevcut olduğunu söylüyor. Güncel olan ikincisi.

**Gemini Omni Flash**
- Blog: düzenleme tek öğe değişikliğinde en güçlü. Birden çok öğenin etkileştiği düzenlemeler zorlanıyor.
- Her sohbet turu ayrı bir üretim olarak ücretleniyor (API tarafındaki not).

**MiniMax H3:** Kling ile karşılaştırma FAQ'sında "H3 en fazla 2K; daha yüksek çözünürlük ya da storyboard'lu sekans için başka model" deniyor.

**Hailuo 2.3:** Sabit oran (girdi görseli), sessiz.

**DOP**
- Metinden video yapamıyor; keyframe şart.
- Preset kategorileri: Effects, Basic/Epic Camera Control, Catch the Pulse, New/Trending, Top Choice, Mix.
- Help'e göre DOP preset kataloğu MCP üzerinden de kullanılabiliyor.

**Veo 3.1:** Standard modu = referans ile özne tutarlılığı ve konuşma. Fast modu = ilk/son kare ve hız.

## 2.4 Modeller için entegrasyon önerileri (etiket ve logo doğruluğu odaklı)

**Öneri 1 — Ürün etiketi kritikse.** Modeli yazıdan değil, **gerçek ürün fotoğrafından** başlatın: i2v ya da başlangıç karesi. Aday modeller:
- **Grok Imagine 1.5:** Sayfası "giriş karesinin detayını ve ışığını korur" diyor.
- **Veo 3.1 Fast:** İlk ve son kareyi aynı packshot yaparak ürünü sabit tutar.
- **MiniMax H3:** "Packaging labels and brand marks render cleanly" iddiası var.
- **Kling 4.0:** Ekrandaki metin ve logo desteği; keyframe ile belli saniyede "ürün açısını pinleme".

Bu modelleri Canvas'ta aynı ürünle yan yana test edin.

**Öneri 2 — Hareketli kadrajda etiket bozulma riski.**
- Hızlı orbit, makro geçiş, ürünün elde dönmesi ve köpük/su altında kalması etiket metnini en çok bozan durumlar. Blog da "eller ürünü örttüğünde ya da ürün hızlı hareket ettiğinde" bozulma uyarısı yapıyor.
- Etiketin okunması gereken anı kısa ve yavaş bir "hero" kareye ayırın.
- Kling 4.0 keyframe, Veo/FLUX/H3 son kare ile o anı gerçek packshot'a sabitleyin. Kritik karelerde gerçek etiketi postta overlay edin.

**Öneri 3 — Çok ürünlü (multi-brand) seri.**
- **Seedance 2.5**'in 50 referansı ve **Wan 3.0**'ın 12 referansıyla aynı mekân, aynı usta karakteri ve farklı ürün SKU'ları kilitlenebilir.
- Wan 3.0 tek prompt'tan 6 çekimlik, sesli, en fazla 30 sn'lik bir Reels kurgusu çıkarıyor. Bu, hızlı varyasyon için uygun.
- Etiket okunurluğu yine her SKU'da ayrı kontrol edilmeli.

**Öneri 4 — Gerçek çekimi bozmadan zenginleştirme.**
- Önce gerçek telefon veya kamera çekimi yapın.
- Sonra şu sırayı izleyin: Relight → Color Palette → (gerekirse) Reframe → ByteDance Upscale / FLUX.3 precise.
- Ürünün piksel içeriğini değiştiren araçları (Object Swap, Seedance Edit, Gemini Omni edit) yalnızca etiketin görünmediği bölgelerde kullanın.

**Öneri 5 — Kling Motion Control.** Usta hareketi (cila sürme, pasta makinesi kullanma) bir referans videodan alıp farklı karaktere aktarmak için kullanılabilir. Ürün etiketi burada da yeniden üretileceğinden ürünün yakın planı ayrı çekilmeli.

**Öneri 6 — DOP / Hailuo 2.3 / Mixed Media.** Hook, geçiş ve efekt amaçlı kısa (3–10 sn) parçalar için uygun. Hailuo 2.3 sessiz olduğundan müzik/ses postta eklenmeli.

**Öneri 7 — Bütçe.** Taslakları 480p/720p'de çekin (Seedance 2.5 8 sn: 24 kredi vs 1080p: 128 kredi). Finali 1080p'de üretip en son upscale edin.

---

# Kaynaklar (okunan sayfalar)

**Resmî Higgsfield blog yazıları:**
- https://higgsfield.ai/blog/higgsfield-3d-jutsu
- https://higgsfield.ai/blog/video-relight-color-palette-higgsfield
- https://higgsfield.ai/blog/edit-ai-video-without-regenerating
- https://higgsfield.ai/blog/how-to-edit-videos-with-ai
- https://higgsfield.ai/blog/kling-4-0-on-higgsfield
- https://higgsfield.ai/blog/minimax-h3-higgsfield
- https://higgsfield.ai/blog/flux-3-higgsfield
- https://higgsfield.ai/blog/gemini-omni-flash-vfx-video-editing
- https://higgsfield.ai/blog/Higgsfield-Omni-VFX
- https://higgsfield.ai/blog/kling-motion-control-3
- https://higgsfield.ai/blog/Grok-Imagine-AI-Video-Best-Use-Cases (Ocak 2026, Grok Imagine 1.5 öncesi)
- https://higgsfield.ai/blog/How-to-Use-Google-Veo-3.1-Complete-Guide-for-the-New-Model
- https://higgsfield.ai/blog/Minimax-Hailuo-2.3-A-Creative-Guide
- https://higgsfield.ai/blog/make-ai-lipsync-videos
- https://higgsfield.ai/blog/Restore-Your-Old-Video-With-Higgsfield-Upscale
- https://higgsfield.ai/blog/seedance-2-5-on-higgsfield-2026
- https://higgsfield.ai/blog/seedance-2-5-pricing-2026
- https://higgsfield.ai/blog/ai-video-credits-explained
- https://higgsfield.ai/blog/higgsfield-vs-kling-2026

**Resmî ürün sayfaları:**
- https://higgsfield.ai/seedance/2.5
- https://higgsfield.ai/kling-4-0-intro
- https://higgsfield.ai/minimax/h3
- https://higgsfield.ai/wan-3-0
- https://higgsfield.ai/grok-imagine-1.5
- https://higgsfield.ai/gemini-omni-flash
- https://higgsfield.ai/veo3.1
- https://higgsfield.ai/mixed-media-intro
- https://higgsfield.ai/canvas-intro
- https://higgsfield.ai/ai-video-reframer
- https://higgsfield.ai/ai-video-upscaler
- https://higgsfield.ai/apps/color-grading

**Help center:**
- https://higgsfield.ai/creator-hub/help-center/ai-models/how-do-i-use-dop
- https://higgsfield.ai/creator-hub/help-center/ai-models/how-do-i-use-lipsync-voiceover-and-aspect-ratios
- https://higgsfield.ai/creator-hub/help-center/ai-models/which-ai-model-should-i-use
- https://higgsfield.ai/creator-hub/help-center/tools/how-do-i-use-canvas
- https://higgsfield.ai/creator-hub/help-center/troubleshooting/my-video-upscale-is-stuck-or-failed-what-should-i-do

**Üçüncü taraf:**
- https://kanjiai.beehiiv.com/p/draw-to-video-is-here-with-higgsfield-ai (Draw to Video, Ağu 2025)
- https://fal.ai/happyhorse ve https://runware.ai/docs/models/alibaba-happyhorse-1-1/guides (HappyHorse; arama özeti üzerinden)
- https://hackernoon.com/how-to-reframe-ai-generated-video-for-any-aspect-ratio-without-regenerating-it (Reframe; arama özeti üzerinden)

**Ön yüz kodu:** higgsfield.ai ana sayfasının ve /ai/video sayfasının yüklediği `assets.higgsfield.ai/tanstack/assets/*.js` dosyaları. Kullanıldığı yerler: menü ve katalog açıklamaları, model girdi limitleri, oranlar, uygulama kimlikleri.
