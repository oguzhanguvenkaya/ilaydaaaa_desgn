# Higgsfield özellik envanteri (26 Ekim 2026)

Kaynak listesi: Higgsfield üst menüsü, Image ve Video açılır menülerinin ekran görüntüleri (higgsfield.ai, 26 Ekim 2026) ve kullanıcının saydığı özellikler. Her satırın ayrıntısı, kaynak linkleri ve `[doğrulanacak]` notları "Detay" sütunundaki araştırma dosyasında.

**Sütunlar**
- **Eski rehber:** `higgsfield_test/docs/higgsfield-arastirma-2026-09-16.md` bu özelliği kapsıyor mu? ✗ yok · ◐ adı geçiyor / yüzeysel · ✓ anlatılmış.
- **Etiket riski:** Ürün etiketi, logo ve ambalajın bozulma riski. Düşük = ürün piksellerine dokunmuyor ya da çok az dokunuyor; Yüksek = ürünü AI yeniden çiziyor. Bu bizim yorumumuz, test edilmedi.
- **Öncelik:** Bizim iş akışımız için öneri. Y = önce dene · O = uygun işte dene · D = şimdilik gerek yok.

Kısaltmalar: A = [A-ajan-otomasyon](../research/2026-10-26/A-ajan-otomasyon.md), B = [B-studyolar-reklam](../research/2026-10-26/B-studyolar-reklam.md), C = [C-eklentiler-canvas](../research/2026-10-26/C-eklentiler-canvas.md), D = [D-gorsel](../research/2026-10-26/D-gorsel.md), E = [E-video](../research/2026-10-26/E-video.md), F = [F-canli-mcp-katalog](../research/2026-10-26/F-canli-mcp-katalog.md).

## 1. Yeni ve üst menü özellikleri

| Özellik | Ne yapıyor (kısa) | Eski rehber | Etiket riski | Öncelik | Detay |
|---|---|---|---|---|---|
| **Content Factory** (22 Eki) | "Ya … olsaydı?" sorusundan 9:16, yüzsüz kısa video veya 1–4 bölümlük seri. 15 sn–5 dk. Ürün/logo girdisi yok | ✗ | Uygulanmaz (ürün koymuyoruz) | O | A, B, F |
| **Playable** (25 Eki) | Playable Ads (oynanabilir reklam, yalnızca Enterprise, ≤5 MB HTML, 9 reklam ağı) + Playable Games (mobil mini oyun, tüm planlar) | ✗ | Orta | D | A |
| **Genjutsu** | Videodaki hareketi yeni özneye aktarma (Motion transfer) veya videodaki ürünü/kişiyi değiştirme (Objects swap). 4–30 sn, ≤30 referans, ≤1080p | ◐ | Yüksek (değişen ürün yeniden çizilir) | Y | A, E, F |
| **Genjutsu Lite** (menüde FREE) | Genjutsu'nun yaklaşık üçte bir fiyatlı hızlı sürümü, ≤10 referans, mod seçimi yok | ✗ | Yüksek | Y (ucuz test) | A |
| **Genjutsu Styles** | Kendi videonu hareket ve kamerayı koruyarak bir görsel dünyada yeniden çizer (kil, örgü, 2D…) | ✗ | Yüksek | O | F |
| **Katana** | Beğendiğin bir referans kurguyu (edit) kendi ürününle sahne sahne yeniden kurar; ≤5 foto. Claude/ChatGPT üzerinden `/katana` | ✗ | Orta–yüksek | O | A, F |
| **AI Influencer** (3 Eki yenilendi) | Menülerle (19 ayar) AI karakter yaratır, 1,12 kredi; Genjutsu ile hareketlendirir | ✗ | Karakter iyi, ürün yeniden çizilir | O | A |
| **Ads Studio** (1 Eki) | Web sitesinden marka kiti → ürün → bir çalıştırmada ≤20 statik reklam (1:1, 4:5, 9:16), reklam başına 4 kredi | ✗ | Bilinmiyor [doğrulanacak] | Y | B |
| **Ad Multiplier** (6 Eki) | 4–30 sn bir reklamın kurgusunu koruyup hook, CTA, ürün, oyuncu, mekân değiştirir | ✗ | Yalnız CTA: düşük · ürün değişimi: yüksek | Y | B, F |
| **Effects / Viral Presets** | Tek fotoğraftan hazır efektli kısa video (60+ efekt), 720p'de 27,5–67,5 kredi | ✗ | Yüksek (insan odaklı efektler) | D–O | B |
| **Marketing Studio** | Ürün çekimi, reklam, pazaryeri, poster, UGC, motion, TikTok; webde 1.500+ şablon, MCP/CLI'de daha küçük set | ✓ (CLI kataloğu) | Orta | Y | B, F |
| **ChatGPT Plugin** | ChatGPT içinden Higgsfield; `/product`, `/genjutsu`, `/katana` vb. Ses üretimi ve web sitesi yok, ≤20 MiB referans | ✗ | Araca bağlı | O (ekip için) | A |
| **MCP** | Claude vb. ajanların Higgsfield kullanması (`mcp.higgsfield.ai/mcp`). Her üretim kredi düşer; ücretli abonelik gerekir | ◐ | Araca bağlı | O | A, F |
| **API** (16 Eyl) | Plandan ayrı, USD bakiyeyle kullandıkça öde; ≥$5, 20 eşzamanlı istek, çıktılar ≥7 gün | ✗ | Modele bağlı | D (ileride toplu SKU) | A |
| **Supercomputer** | Sohbetle görev planlayan ajan çalışma alanı; Games, Faceless channel, skill'ler | ✓ | Araca bağlı | O | A |
| **Academy** | Eğitim içerikleri | ✗ | — | Bakılmadı (üretim aracı değil) | — |
| **Audio** (üst menü) | Ses üretimi, ses değiştirme, 18 dilde çeviri, ses klonlama (izinli) | ✗ | — | **Ayrıntılı araştırılmadı** [doğrulanacak] | E (Lipsync bölümü), F |

## 2. Image menüsü — özellikler

| Özellik | Ne yapıyor (kısa) | Eski rehber | Etiket riski | Öncelik | Detay |
|---|---|---|---|---|---|
| Create Image | Çok modelli metinden/referanstan görsel ekranı | ◐ | Modele bağlı | Y | D |
| Cinematic Cameras | Kamera gövdesi, lens, odak (8–50 mm), diyafram seçerek görsel. Cinema Studio'nun görsel modu olduğu varsayıldı; CLI kataloğunda "Cinematic Studio Image" var [eşleşme doğrulanacak] | ✗ | Orta–yüksek | O | D |
| Canvas | Node (kutucuk) tabanlı pano: modelleri zincirle, yan yana karşılaştır, şablon kaydet, ekipçe çalış. Unlimited burada geçerli değil | ✗ | Orta | Y (model karşılaştırma) | C, E |
| Soul Moodboard | 10–80 referanstan marka estetiği öğrenir; yalnızca Soul 2.0 | ✗ | Uygulanmaz (ürünsüz sahne) | O | D |
| Soul ID Character | 20–80 fotodan kişi yüzü öğrenir | ✗ | — | D | D |
| AI Influencer | Bkz. 1. bölüm | ✗ | | O | A |
| Photodump | Soul ID karakterinden 15 karelik sosyal set | ✗ | — | D | D |
| **Relight** (görsel) | Işık yönü, sertlik, parlaklık, renk; ürün fotoğrafçılığı kullanım alanı olarak sayılıyor | ◐ | Orta (yeniden render; test) | Y | D |
| **Inpaint** | Maskelenen bölgeyi değiştirir, dışını korur (Nano Banana Pro Inpaint) | ◐ | Düşük (etiketi maskelemezsen) | Y | D |
| **Image Upscale** | ByteDance (2K/4K) veya Topaz. Etiket için yalnızca Standard modlar; canlı katalogda Topaz **Text Refine** seçeneği var | ◐ | Standard: düşük · generative: yüksek | Y | D |
| Face Swap | Yüz değiştirme; günde 5 ücretsiz (free plan) | ✗ | — | D (KVKK riski) | D |
| Character Swap | Karakter kimliğini başka sahneye aktarır | ✗ | — | D | D |

## 3. Image menüsü — modeller

| Model | Kaynağın öne çıkardığı | Etiket metni iddiası (test edilmedi) | Detay |
|---|---|---|---|
| Soul 2.0 | Moda/kültür estetiği, Moodboard, Soul ID; 2K'da 0,125 kredi | Metin güçlü yanı **değil** | D |
| Soul Cinema | Sinematik film karesi; video başlangıç karesi | Yok | D |
| GPT Image 2.5 Sunburst / Flare | Hassas düzenleme / hızlı varyasyon; 16 referans; 1,5–26,5 kredi | "text rendering better than most" | D |
| Nano Banana 2.1 | Bir referanstan 40 görsel tutarlılığı | "label text" tutarlılığı | D |
| Seedream 5.0 Pro | Maskesiz nokta düzenleme, infografik | "fix a label", 10–14 dil (Türkçe açık değil). Canlı katalog: **en fazla 2K** | D |
| **Nano Banana Pro** | Adet, metin, perspektifte en yüksek hassasiyet; HEX renk; 2K 2 / 4K 4 kredi | **En güçlü iddia** ("packaging text… perfect spelling") | D |
| FLUX 3 Image / FLUX.2 | Prompt sadakati; FLUX.2'de JSON prompt ve HEX | Çok dilli metin | D |
| Recraft V4.1 | Tasarım, vektör çıktı | Zayıf | D |
| Grok Imagine 2.0 | Canlı MCP kataloğunda `grok_image_2_0` olarak var (1k/2k; 26 Eki). Webde ayrı tanıtım sayfası bulunamadı | Kaynakta iddia yok | D, [katalog](../bilgi/canli-katalog-2026-10-26/README.md) |
| Z-Image | 1–3 sn hızlı taslak | Kendi blogu tipografide NB Pro'yu üstün sayıyor | D |
| Topaz | Upscaler | Standard modda kaynağa yakın | D |

## 4. Video menüsü — özellikler

| Özellik | Ne yapıyor (kısa) | Eski rehber | Etiket riski | Öncelik | Detay |
|---|---|---|---|---|---|
| Create Video | Model seç + prompt/referans; **ilk/son kare kilitleme** | ◐ | Orta (ara karelerde risk) | Y | B |
| **Cinema Studio 4.0** | Tür, kamera, lens, ışık, renk, duygu; Seedance 2.5 tabanlı, ≤30 sn, ≤50 referans; AI Director | ◐ | Yüksek | O | B |
| Faceless Studio | Konudan 1–5 dk animasyonlu anlatımlı bölüm; 1 dk = 246 kredi | ✗ | Uygulanmaz | D–O | B |
| **3D Jutsu** | Prompt'tan düzenlenebilir 3D sahne; kamera yolu; GLB içe/dışa aktarma; videoya gönderme | ✗ | Geometri iyi, finalde etiket yeniden çizilir | O | E, F |
| **Shorts Studio** | **Kendi videonu** 40+ stil presetiyle 9:16 kısa formata çevirir; ≤2 dk girdi, 720p | ✗ | **Düşük** | Y | B |
| Higgsfield Explainer | Konu/URL/dosyadan 20 sn–10 dk açıklama videosu | ✗ | Yüksek (stilize çizer) | O | B |
| Mixed Media | Videoya 40+ stil (neon, doodle…) ve otomatik rotoskop | ◐ | Yüksek | D–O | E |
| Edit Video | Videodaki bir öğeyi değiştir (Kling Video Edit / Seedance 2.5 Edit) | ◐ | Yüksek (değişen bölge) | O | E |
| **Video Upscale** | ByteDance, Topaz, FLUX.3 Upscale. Help center ürün/metin videosunda Topaz'ı önermiyor | ◐ | ByteDance / FLUX.3 precise: düşük | Y | E |
| **Reframe** | Videoyu yeni orana çevirir, eksik alanı AI üretir; ≤1 dk; 15 sn 720p = 71 kredi | ◐ | Orta (kenardaki ürün) | Y | E |
| Click to Ad | Ürün URL'sinden ad, açıklama, ≤8 foto, logo çekip video reklam (Marketing Studio Product Link) | ✗ | Yüksek + marka karışması | O | B |
| **Change Color Palette** | Videoya renk derecelemesi; 50+ preset veya görselden palet | ✗ | Düşük (marka rengi kayabilir) | Y | E |
| **Relight** (video) | Videonun ışığını değiştirir, hareket/kadraj korunur; 15 sn 720p = 42 kredi (eski blog 135) | ✗ | Düşük–orta | Y | E |
| Lipsync Studio | Görsel/videodan konuşan klip; 8–10 model | ✗ | Ürün eldeyse yüksek | O | E |
| Draw to Video | Görsel üzerine ok/etiket çizerek hareketi yönetme | ◐ | Orta | O | E |
| Draw to Edit | Bölge işaretleyip değiştirme (görsel: Nano Banana; video: Seedance 2.5 Edit) | ✗ | Etiketi işaretlemezsen düşük | O | E |

## 5. Video menüsü — modeller

| Model | Kaynağın öne çıkardığı | Süre / çözünürlük / ses | Kredi örneği | Detay |
|---|---|---|---|---|
| Seedance 2.5 | ≤50 referans, bölgesel edit, Cinema Studio altyapısı | ≤30 sn · 480p–1080p · ses var | 8 sn: 24 (480p) / 128 (1080p) | E |
| Kling 4.0 | Hızlı hareket, ≤10 keyframe, ekranda metin ve **logo** | 3–30 sn · 720p/1080p (canlı katalog; tanıtım sayfasındaki 4K katalogda yok) · stereo | 5 sn 720p 25 · 30 sn 1080p 225 | E |
| Kling Motion Control | Referans videodaki hareketi karakter görseline aktarma | ≤30 sn · 720p/1080p | [doğrulanacak] | E |
| Kling 3.0 Omni Edit | Videoyu ≤4 görselle düzenleme | [doğrulanacak] | [doğrulanacak] | E |
| Gemini Omni Flash 1.1 | Sohbetle çok turlu edit, 10'ar sn uzatma, SynthID/C2PA damgası | 8–10 sn (uzatmayla ≤60) · 720p · ses | ~$0,15/sn | E |
| FLUX.3 Video | Hareket hâlinde okunur tipografi | 5–20 sn · 720p/1080p · opsiyonel ses | 5 sn 720p 27,5 | E |
| FLUX.3 Upscale | "precise" mod kaynağa sadık | 1080p/2K/4K | 15 sn 720p 14 | E |
| MiniMax H3 | **"Packaging labels and brand marks render cleanly"** iddiası | ≤15 sn · 2K · stereo | 5 sn 20 · 15 sn 60 | E |
| Hailuo 2.3 | Fizik, dönüşüm efektleri; logolar keskin iddiası | 6/10 sn · 768p/1080p · **sessiz** | [doğrulanacak] | E |
| Wan 3.0 | Tek prompt'tan ≤6 çekimlik, sesli, ≤30 sn kurgu; ≤12 referans | ≤30 sn · [doğrulanacak] | [doğrulanacak] | E |
| Grok Imagine 1.5 / 1.5 Lite | Başlangıç karesinin detayını sadık koruma / ucuz hızlı | 2–15 sn · 480p/720p | [doğrulanacak] | E |
| Google Veo 3.1 | Yüksek sadakat, diyalog; Fast modda ilk/son kare | 4/6/8 sn · 720p/1080p | ~$0,35/sn | E |
| HappyHorse | Alibaba modeli; resmî Higgsfield sayfası yok | [doğrulanacak] | [doğrulanacak] | E |
| Higgsfield DOP | Higgsfield'in kendi i2v'si, kamera ve VFX presetleri | 3/5 sn | [doğrulanacak] | E |

## 6. Eklentiler (Plugins)

Her eklentinin iki biçimi var: **(A)** uygulamanın içinde senin tıkladığın panel, **(B)** Claude Code'un uygulamayı yerel bilgisayarda kumanda ettiği MCP bağlantısı. Kurulum: [yerel-kurulum.md](yerel-kurulum.md#6-isteğe-bağlı-masaüstü-uygulama-eklentileri).

| Eklenti | (A) Panel araçları | Sürüm şartı | Çıktı nereye | Etiket riski (doğru kullanılırsa) | Öncelik | Detay |
|---|---|---|---|---|---|---|
| **Photoshop** | Angles, Mockup Studio, Expand, Remove BG, Relight (help-center'a göre 12 araç: Layer Decompose, Realtime AI…) | 2024+ (UXP) | **Yeni katman** | Düşük: ürün katmanı korunur | **Y** | C |
| **Premiere Pro / After Effects** (tek kurulum) | Generate Video/Image, Reframe, Remove BG, Draw to Edit, Upscale 4K/8K, Edit Video | 2024 veya 2025+ [çelişkili] | Timeline / kompozisyon | Düşük: AI yalnızca B-roll ve arka planda | Y | C |
| **DaVinci Resolve** | Aynı araçlar + **AI LUT Creator** (.cube) | 19+, App Store sürümü değil. (B) MCP bağlantısı **Resolve Studio** ister | Media Pool / Timeline | Düşük (LUT yalnızca renk) | O | C, F |
| **Figma / FigJam** | Görsel/video, Remove BG, Color Grading, Relight, Expand, Angles, Mockup Studio; FigJam'de Canvas Nodes | Figma Community | Kanvasta katman | Düşük: metin ve logo vektör kalır | **Y** | C |
| **Blender** | Scene Builder, 3D Model (fotoğraftan mesh, Meshy 5), Character Animation, Image, Video, Camera, Asset | 5.1+ | .blend sahne | Düşük: **gerçek etiketi UV doku olarak kendin kaplarsan** | O | C, F |

## 7. Kapsam notu

- **Canlı katalog (26 Ekim):** Modellerin güncel parametreleri için [canlı katalog özeti](../bilgi/canli-katalog-2026-10-26/README.md). Çelişkide katalog esas alınır.

- **Ayrıntılı araştırılmayanlar:** Audio menüsü (yalnızca Lipsync içinden dolaylı bilgi var), Academy, Explore, Assets, Enterprise. Nedeni: kullanıcının listesinde değillerdi; Academy, Explore ve Assets üretim aracı değil. Audio bir sonraki turda araştırılmalı (Türkçe seslendirme bizim için önemli).
- **Fiyatlar** blog yazılarındaki tarihli örneklerdir; kesin fiyat her üretimde Generate düğmesinde görünür. Birçok yerde kaynaklar çelişiyor; ilgili dosyada işaretli.
- **Unlimited:** Resmî help-center'a göre web dışındaki kanallarda (MCP, CLI, eklenti, Canvas, Supercomputer, API) geçerli değil. After Effects blogu ve bir Supercomputer yardım sayfası buna aykırı ifade içeriyor [doğrulanacak].
