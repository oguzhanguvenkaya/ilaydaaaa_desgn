# D — Higgsfield Image menüsü: Özellikler ve Modeller

Araştırma tarihi: 26 Ekim 2026. Kaynaklar higgsfield.ai sayfaları, /blog, /creator-hub/help-center ve /creator-hub/changelog. Hiçbir üretim yapılmadı ve Higgsfield MCP araçları çağrılmadı.

**İşaretler:**
- **[resmî]**: higgsfield.ai kaynağı.
- **[3. taraf]**: Higgsfield dışı kaynak.
- **[doğrulanacak]**: Kaynakta bulunamadı ya da kaynaklar çelişiyor.
- **Öneri**: Bizim (oto bakım/detailing distribütörü, Instagram post/Reels/ürün görseli) için yorum. Kaynak bilgisi değildir.

> **Genel uyarı.** "Metin/etiket doğruluğu" iddiaları satıcının ya da model sağlayıcının pazarlama iddiasıdır. Hiçbiri bizim etiketlerimizde test edilmedi. Ürün etiketi, logo ve ambalaj üretilen görselde **her zaman** gerçek ürünle karşılaştırılmalı. Higgsfield'in kendi ürün fotoğrafçılığı sayfası da bunu söylüyor: "Check every result against your product before listing".

---

## 0. Bizi doğrudan ilgilendiren platform kuralları

| Konu | Kaynakta ne yazıyor | Bizim için anlamı (öneri) |
|---|---|---|
| **Marka/logo IP filtresi** | Prompt veya referans görsel "branded product names or logos" içeriyorsa üretim engellenebilir. Kullanıcıya ait girdilerde "I own the rights for this image" butonu çıkabilir ve uygunsa engeli kaldırır. Engellenen üretimlerde kredi çoğunlukla iade edilir. [resmî] [help: IP block](https://higgsfield.ai/creator-hub/help-center/troubleshooting/my-generation-blocked-for-copyright-or-ip) | Distribütörü olduğumuz yabancı markaların logoları filtreye takılabilir. İlk testlerde bunu ölçmek kritik **[doğrulanacak]**. Marka sahibinden yazılı kullanım izni alınmalı. Rights-holder doğrulaması için Support'a yazılabiliyor. |
| **Ticari kullanım** | Kullanım Koşulları 4.4: çıktılar kullanıcıya aittir ve ticari kullanım kısıtlanmaz. Watermark'sız indirme ücretli planlarda var. IP tazminatı yalnızca Enterprise planda. [resmî] [help: ownership](https://higgsfield.ai/creator-hub/help-center/account/who-owns-my-generations-and-can-i-use-them-commercially) | Face Swap ve Character Swap uygulama sayfaları ise ticari hakkı "all paid Pro plans" ile sınırlıyor. Kaynaklar çelişiyor **[doğrulanacak]**. |
| **Kredi: MCP/CLI/Canvas/Supercomputer** | Bu kanallardan yapılan üretim, Unlimited model olsa bile **her zaman kredi düşer**. Batch 2–4 seçilirse her çıktı ayrı ücretlendirilir. [resmî] [help: credits](https://higgsfield.ai/creator-hub/help-center/credits/what-uses-my-credits), [help: unlimited](https://higgsfield.ai/creator-hub/help-center/credits/what-are-unlimited-models-and-which-plans-include-them) | Toplu üretimde web arayüzü + Unlimited, maliyet açısından ayrıca değerlendirilmeli. |
| **Unlimited** | Modele özel. Liste plan kartında yazıyor ve higher plan daha fazla model içeriyor. Görsel bundle'larında eşzamanlılık 2 üretim. Scale planı (changelog): aylıkta Nano Banana Pro ve Seedream 5.0 Pro. [resmî] | Etiket hassasiyeti yüksek iki model (NB Pro, Seedream 5.0 Pro) Unlimited listesinde geçiyor. Plan seçiminde dikkate alınmalı. |
| **Çözünürlük ve en/boy (genel)** | Create Image sayfası: "up to 4K (4096x4096)" ve "1:1, 9:16, 16:9, 3:4, 4:3, and more". Aynı sayfada "native 2K with intelligent refinement to 4K" ifadesi de geçiyor. [resmî] [ai-image](https://higgsfield.ai/ai-image) | İfadeler birbiriyle çelişiyor. Model bazında aşağıdaki tabloya bakın **[doğrulanacak]**. |

---

## 1. ÖZELLİKLER (Features)

### 1.1 Create Image
- **Ne yapıyor:** Çok modelli metinden görsele (text-to-image) ve referanstan görsele üretim ekranı. Model seçici üzerinden Soul, Nano Banana, GPT Image, Seedream, FLUX, Recraft vb. modellere geçiliyor. [resmî]
- **URL:** https://higgsfield.ai/ai-image (uygulama: `https://higgsfield.ai/ai/image?model=...`, örn. `?model=nano-banana-pro`, `?model=gpt_image_2`)
- **Nasıl kullanılır** (help center ve blog adımları birleştirildi):
  1. Image → model seçici → modeli seç.
  2. Giriş modu seç: Text-to-Image, Multi-reference veya Image-to-Image (NB ailesi için help center).
  3. Prompt yaz. Metin varsa **tırnak içinde** ver; font stilini, boyutu ve yerleşimi açıkça tarif et. Bu, help center'ın NB önerisi.
  4. Referans ekle. Maksimum sayı modele göre değişir: NB Pro/2/2.1 için 14, GPT Image 2.5 için 16.
  5. Çözünürlük, en/boy, kalite ve batch ayarla. Maliyet Generate butonunda gösterilir.
- **Kredi:** Modele, çözünürlüğe ve batch'e göre değişir. Rakamlar model tablosunda. [resmî]
- **Sınırlar:** Free plan günlük ücretsiz kredi verir. Plan bazında model erişimi farklıdır ("Model availability depends on your plan"). [resmî]
- **Öneri:** Ürünlü post için önce **gerçek ürün fotoğrafını referans** verip etiket doğruluğu iddiası taşıyan bir modelle başlayın: NB Pro, NB 2.1, GPT Image 2.5 Sunburst veya Seedream 5.0 Pro. Etiket bozulursa Inpaint ile yalnızca etiket bölgesini düzeltin. Daha güvenli yol: etiket bölgesini gerçek fotoğraftan kompozit edin.

### 1.2 Cinematic Cameras (kamera kontrollü görsel üretimi)
- **Durum:** Image menüsündeki "Cinematic Cameras" adına birebir uyan resmî bir sayfa **bulunamadı**. `higgsfield.ai/cinematic-cameras` 404 döndü. En yakın resmî karşılık, **Cinema Studio**'nun görsel (Hero Frame) üretimi **[menüyle eşleşmesi doğrulanacak]**.
- **Ne yapıyor (Cinema Studio Image):** "Hero Frame First" yaklaşımı. Animasyondan önce durağan kare kamera gövdesi, lens, odak uzaklığı ve diyafram seçilerek üretilir. [resmî] [blog: Cinema Studio 2.0](https://higgsfield.ai/blog/cinema-studio-guide)
  - Rig: kamera sensörü, lens camı (örn. Cooke), **odak 8–50 mm**, diyafram (alan derinliği ve bokeh), kaydedilebilir kamera preset'leri.
  - Görsel tarafında: "Create 3D scene" ile kareye 3B olarak girip kompozisyonu değiştirme; 2x2, 3x3 ve 4x4 grid varyasyon.
  - Cinema Studio 4.0 (varsayılan sürüm): Camera (Modern, DV Camcorder, 35mm Film, 8mm Film), 5–6 lens (Auto, Clean Sharp, Anamorphic, Vintage vb.), aperture, 50+ renk paleti, 6 ışık preset'i, **en fazla 50 referans**. 4.0 bir video odaklı sürüm (Seedance 2.5 tabanlı). [resmî] [help: Cinema Studio](https://higgsfield.ai/creator-hub/help-center/tools/how-do-i-use-cinema-studio), [blog: CS 4.0](https://higgsfield.ai/blog/cinema-studio-4-0)
- **Nasıl:** higgsfield.ai → Cinema Studio → sürüm seç → (görsel) referans/prompt + kamera, lens, odak ve diyafram → Generate.
- **Kredi:** Cinema Studio için sabit fiyat bulunamadı. Plan Unlimited listesine bağlı **[doğrulanacak]**.
- **Sınırlar:** Gerçek yüz ve korumalı IP algılanırsa "May contain protected content" bloğu. Ürün logoları da etkilenebilir **[doğrulanacak]**.
- **Ek (resmî, changelog 19 Eki 2026):** ChatGPT eklentisindeki "3D Angles" fotoğrafı 3B sahneye çeviriyor: 24–300 mm lens, ƒ1.4–ƒ16, 1:1–21:9 arası 8 format. Image menüsünde değil.
- **Öneri:** Orta öncelik. Reels kapak karesi veya "hero shot" (örn. makro lens, sığ alan derinliğiyle cila yüzeyi) için kullanışlı olabilir. Etiketli ürün için çıktıyı Inpaint/kompozit ile doğrulayın. Reels'e geçişte aynı kare video modeline başlangıç karesi olarak verilebilir.

### 1.3 Soul Moodboard
- **Ne yapıyor:** Soul 2.0 için özel stil preset'i. Kendi referans görsellerinizden ışık, doku, kontrast ve renk öğrenir ve sonraki üretimlere tutarlı uygular. İki türü var: **Curated** (20+ hazır; Y2K Studio, Digital Camera, Retro BW…) ve **Personal**. [resmî] [blog: Moodboards](https://higgsfield.ai/blog/create-custom-ai-moodboard-soul-2), [help: Soul](https://higgsfield.ai/creator-hub/help-center/ai-models/how-do-i-use-soul-to-generate-images)
- **Nasıl:** Soul 2.0 → Moodboard ikonu → "Build your moodboard" → cihazdan veya Assets'ten yükle → Soul 2.0 analiz eder → isim ver → prompt ile birlikte uygula.
  - Görsel sayısı: **en fazla 80**. Yaklaşık 10 görsel genelde yeterli; 20–30 (help center: 20+) daha iyi.
  - Görseller tutarlı tek estetikte olmalı. **Yüz içermemesi** önerilir. Bulanık veya düşük kaliteli görsel yüklenmemeli.
  - Soul ID ve Soul HEX ile birlikte kullanılabilir.
- **Kredi:** Moodboard oluşturmanın ücreti kaynakta yok **[doğrulanacak]**. Soul üretimleri "standart oranlarla" ücretlenir.
- **Sınırlar:** **Yalnızca Soul 2.0'da** var; Soul ve Soul Cinema'da yok. Referans görsel eklenince prompt alanı kapanır. Soul 2.0'ın metin render etmesi "core strength" değil. [resmî]
- **Öneri:** **Orta–yüksek öncelik (marka estetiği için).** Mevcut başarılı Instagram görsellerimizden (yüzsüz, ürün/garaj/detay sahneleri) bir "marka Moodboard"u kurulabilir. Arka plan ve sahne üretimi bununla tutarlı tutulur. Ürün etiketi ise Soul'a bırakılmamalı; etiketli ürün sonradan NB Pro/Inpaint/kompozit ile yerleştirilmeli.

### 1.4 Soul ID Character
- **Ne yapıyor:** Bir kişinin yüzünü öğrenip Soul ailesinde (Soul, Soul 2.0, Soul Cinema) tutarlı karakter üretir. Seedance videoda "Element" olarak taşınabilir. [resmî] [help: Soul ID](https://higgsfield.ai/creator-hub/help-center/ai-models/how-do-i-create-and-use-a-soul-id-character)
- **Nasıl:** Soul → "Train new character" → **20+ foto (en fazla 80)** yükle → eğitim birkaç dakika sürer (blog: yaklaşık 3–5 dk) → isim ver → Character sekmesinden seç.
  - Fotoğraflar farklı açılardan, iyi ışıklı ve güncel (son 4–5 ay) olmalı. En az bir boy fotoğrafı bulunmalı. Gözlük/şapka ve grup fotoğrafı olmamalı.
- **Kredi:** Eğitim ücreti kaynakta yok **[doğrulanacak]**. Photodump blogu (Eyl 2025) "ilk karakter ücretsiz" diyor; güncelliği doğrulanmalı.
- **Sınırlar:** Sonuç "piksel-aynı" değil, "açıkça aynı kişi" düzeyinde. Tek kişi tutar. Dışa aktarılamaz. Yalnızca kendi yüzünüz ya da izinli kişiler kullanılabilir. Arka plan kalabalığında yüzü klonlayabilir. [resmî]
- **Öneri:** **Düşük öncelik.** Yalnızca kalıcı bir "marka yüzü" veya detailing ustası kullanılacaksa ve yazılı rıza alınmışsa anlamlı. Asıl ihtiyacımız olan ürün tutarlılığını Soul ID sağlamıyor.

### 1.5 Photodump
- **Ne yapıyor:** Bir Soul ID karakterinden tek seferde sosyal medya "photo dump" seti üretir. [resmî]
  - **Soul Photodump** (Şub 2026, Soul 2.0): 15 foto. 2 preset var: "Male Archive" ve "Cool Girl Dump". [blog](https://higgsfield.ai/blog/how-to-create-ai-photodump-higgsfield-soul)
  - Eski **Photodump Studio** (Eyl 2025): 26 kare, ≥25 fotoğrafla karakter eğitimi. [blog](https://higgsfield.ai/blog/Higgsfield-Photodump-Studio-Your-Viral-Photoshoot)
  - `higgsfield.ai/photodump-studio` bugün `ai/image?model=soul-v2&modal-photo-dump=true` adresine yönleniyor (26.10.2026 gözlemi). Güncel sürüm Soul 2.0 içindeki Photodump.
- **Nasıl:** Preset seç → Soul ID karakteri seç veya oluştur → Generate → 15 görsel → indir ve carousel için seç.
- **Kredi:** Kaynakta yok **[doğrulanacak]**.
- **Sınırlar:** İnsan/karakter odaklı. Preset'ler cinsiyete göre kurgulanmış. Ürün yerleştirme kontrolü yok.
- **Öneri:** **Düşük öncelik.** İnsan odaklı lifestyle carousel aracı; ürün/etiket doğruluğu ihtiyacımızı karşılamıyor.

### 1.6 Relight
- **Ne yapıyor:** Yüklenen fotoğrafın ışığını yeniden kurar. Yön, sertlik, parlaklık ve renk ayarlanır. Blog'a göre "depth-mapping" ile 3B uzayda ışık konumlandırır ve kullanım alanı olarak açıkça "Professional Product Photography" sayılıyor ("Add a Top or Side light to create depth and texture"). [resmî] [blog: Relight, Oca 2026](https://higgsfield.ai/blog/Relight-Director-Style-Cinematic-Lighting)
- **URL:** https://higgsfield.ai/apps/relight
- **Nasıl:**
  1. Görsel yükle → Relight paneli.
  2. Hızlı ızgara: Top / Front / Right / Left / Back / Bottom.
  3. Işık yön pedinde sürükleyerek açı ayarla.
  4. Soft / Hard seç.
  5. Brightness %0–100 (varsayılan %50); renk HEX (varsayılan #FFFFFF).
  6. Generate.
- **Kredi:** Kaynakta yok **[doğrulanacak]**.
- **Sınırlar:** Çıktı çözünürlüğü ve kabul edilen dosya boyutu kaynakta yok **[doğrulanacak]**. Generative yeniden render olduğu için etiket metninin bozulmadan kalıp kalmadığı **test edilmeli**.
  - [3. taraf, gaga.art] Relight'ın GPT Image 1.5/FLUX.2 üzerinde çalıştığını iddia ediyor; resmî doğrulama yok.
  - Ayrıca (changelog 21 Ağu 2026) **video** için ayrı bir Relight ürünü var: 6 preset + 2 özel ışık kaynağı.
- **Öneri:** **Yüksek öncelik (test edilecek).** Depo/mağazada çekilmiş düz ışıklı gerçek ürün fotoğraflarına üst/yan ışık eklemek için ideal aday. Akış: gerçek foto → Relight → etiketi orijinalle piksel düzeyinde karşılaştır. Bozulma varsa etiket bölgesini orijinal fotoğraftan maskeyle geri koy (Photoshop/Canva katmanı).

### 1.7 Inpaint (Nano Banana Pro Inpaint)
- **Ne yapıyor:** Fırçayla maskelenen bölgeyi prompt'a göre değiştirir; maske dışı korunur. Sayılan kullanımlar: nesne kaldırma veya değiştirme, arka plan onarımı, ışık düzeltme, **"Text Editing & Label Fixing — mask a sign or label → rewrite it cleanly and in perspective"**. Hedef kitlede "E-commerce sellers: label edits, product cleanup" sayılıyor. [resmî] [blog: NBP Inpaint, Ara 2025](https://higgsfield.ai/blog/Top-Editing-Tool-in-2025-Nano-Banana-Pro-Inpaint)
- **URL:** https://higgsfield.ai/edit?model=nano_banana_pro_inpaint
- **Nasıl:**
  1. Edit → Nano Banana Pro Inpaint → görsel yükle.
  2. Değişecek alanı maskele. Kenarları temiz tutun; değiştirme yapılacaksa maskeyi biraz geniş alın.
  3. Prompt yaz, örn. "Same lighting, match original shadows".
  4. Kalite seç: Low / Medium / High. Blog ticari iş için High öneriyor.
  5. Generate.
  - Blog ipucu: karmaşık düzenlemeleri küçük adımlarla, katman katman yapın.
- **Diğer maskeli seçenekler:** "Brush over the area on Nano Banana 2, Seedream 5.0 Pro, or Ideogram" (AI Image Editor sayfası). NB 2.1 sayfası 2.1'in Inpaint ve Banana Placement'ı "power" ettiğini söylüyor. [resmî] [ai-image-editor](https://higgsfield.ai/ai-image-editor), [NB 2.1](https://higgsfield.ai/nano-banana-2-1-intro)
- **Kredi:** Kaynakta yok **[doğrulanacak]**.
- **Sınırlar:** "Zero hallucination" ve "pixel-level precision" gibi ifadeler pazarlama iddiası, test edilmedi. Çıktı çözünürlüğü kaynakta yok **[doğrulanacak]**. Eski bir arama sonucunda "SOUL Inpaint" için Pro/Ultimate plan şartı geçiyor (Higgsfield gönderisi, tarihi eski) **[doğrulanacak]**.
- **Öneri:** **Yüksek öncelik.** Gerçek ürün fotoğrafını koruyarak yalnızca arka planı değiştirmek, kir/leke/tozu temizlemek veya sahneye nesne (mikrofiber bez, köpük, araba yüzeyi) eklemek için birincil araç. **Etiket metnini Inpaint ile "yeniden yazdırmak" son çare olmalı.** Doğru etiket her zaman gerçek fotoğraftan gelmeli.

### 1.8 Image Upscale (Topaz / ByteDance)
- **Ne yapıyor:** Görseli 2K/4K'ya ya da (Topaz ile) istenen piksel boyutuna büyütür. Denoise, keskinleştirme, yüz iyileştirme ve "Recovery" (generative onarım) içerir. [resmî] [ai-image-upscaler](https://higgsfield.ai/ai-image-upscaler)
- **URL:** https://higgsfield.ai/upscale
- **Nasıl:**
  1. Görsel yükle veya Higgsfield üretimini seç.
  2. Motoru seç:
     - **ByteDance Upscale:** 2K veya 4K, prompt yok. "Remove-background" seçeneği var ve "e-commerce ready" deniyor.
     - **Topaz:** Herhangi bir boyut; sharpening, denoise (0–1), face enhancement (strength/creativity), Recovery ve texture kontrolü.
  3. Çalıştır ve indir.
- **Mod uyarısı (resmî FAQ):** "Generative Topaz modes like Redefine add more creative change, so use Standard modes when you want the closest match."
- **[3. taraf/eski arama özeti, Ağu 2025]** Topaz görsel preset'leri: Standard, High Fidelity v2, **Text Refine**, Art & CG, Low Res. Ölçek 2x–16x. Pro+ plan gerekiyormuş. Kaynak sayfa artık 404 **[doğrulanacak]**.
- **Kredi:** Kaynakta yok **[doğrulanacak]**.
- **Sınırlar:** FAQ'e göre baskı için "web, screens, and smaller prints" uygun. Sonuç orijinaldeki detaya bağlı.
- **Öneri:** **Yüksek öncelik, ama yalnızca Standard/Precise modlarla.** Tedarikçiden gelen düşük çözünürlüklü ürün fotoğraflarını büyütmek için kullanın. Generative/Recovery/Redefine modları etiket harflerini "uydurabilir"; etiketli görsellerde kapalı tutun. "Text Refine" preset'i mevcutsa test edin.

### 1.9 Face Swap
- **Ne yapıyor:** Hedef foto veya videodaki yüzü kaynak yüzle değiştirir. [resmî] [apps/face-swap](https://higgsfield.ai/apps/face-swap)
- **Nasıl:** Hedef yükle → kaynak yüz yükle → Generate.
- **Kredi/limit:** Free planda **günde 5 ücretsiz görsel face swap**. Video swap yalnızca ücretli planlarda. Süre plana göre 30 sn–2 dk. Tek seferde tek yüz. [resmî]
- **Sınırlar:** Rıza gerekir (Kullanım Koşulları 5.1 / AI Image Editor sayfası: "only with the consent of the person"). Uygulama sayfasına göre ticari hak "paid Pro plans" ile sınırlı; bu, ToU yardım sayfasıyla çelişiyor **[doğrulanacak]**.
- **Öneri:** **Düşük öncelik / kullanılmaması önerilir.** Ürün doğruluğuna katkısı yok. KVKK ve itibar riski taşıyor.

### 1.10 Character Swap (2.0)
- **Ne yapıyor:** Kaynak karakterin kimliğini hedef sahnedeki poz, kıyafet ve ışığa aktarır (image-to-image; text-to-image değil). [resmî] [apps/character-swap](https://higgsfield.ai/apps/character-swap)
- **Nasıl:** Kaynak karakter yükle → hedef sahne yükle → Generate.
- **Kredi/limit:** Free planda **günde 5 ücretsiz** üretim. Ticari kullanım "paid Pro plans" ile (sayfaya göre). [resmî]
- **Sınırlar:** Yalnızca tek karakter. Ürün/nesne değişimi için tasarlanmamış.
- **Öneri:** **Düşük öncelik.** Ürün veya nesne değiştirme ihtiyacı için Inpaint, NB 2.1/Pro ya da Seedream 5.0 Pro "point-level editing" daha uygun.

---

## 2. MODELLER — Kısa tablo

"Metin/etiket" sütunundaki ifadeler kaynağın iddiasıdır ve **test edilmedi**. Kredi rakamları yalnızca kaynakta varsa yazıldı. $ karşılıkları Higgsfield bloglarındaki yaklaşık değerlerdir ve plana göre değişir.

| Model | Güçlü yanı (kaynağa göre) | Ürün/etiket metni (kaynak iddiası) | En/boy · çözünürlük · referans | Kredi (kaynakta varsa) | URL |
|---|---|---|---|---|---|
| **Higgsfield Soul 2.0** | Higgsfield'in kendi "fashion-aware, culture-native" modeli. 20+ preset, Moodboard, Soul HEX, Soul ID. | **Metin "core strength" değil.** Ürün mockup desteği "limited". | 9:16, 3:4, 2:3, 1:1, 4:3, 16:9, 3:2 · kalite 1.5k/2k · batch 1–4 · referans görsel eklenince prompt kapanır | 2K'da 0,125 kredi/görsel (≈$0,006) | [soul-intro](https://higgsfield.ai/soul-intro), [help](https://higgsfield.ai/creator-hub/help-center/ai-models/how-do-i-use-soul-to-generate-images), [kıyas](https://higgsfield.ai/blog/soul-2-vs-nano-banana-pro) |
| **Soul Cinema** | Sinematik ve atmosferik görüntü, "film still" dokusu; video için başlangıç karesi. Preset/Moodboard yok; Soul HEX ve Soul ID var. | Kaynakta iddia yok. | Ayarlar: en/boy, kalite, batch (1–4); değerler ayrıca belirtilmemiş **[doğrulanacak]** · referans eklenince prompt kapanır | "Credit system", rakam yok **[doğrulanacak]** | [soul-cinema](https://higgsfield.ai/soul-cinema), [help](https://higgsfield.ai/creator-hub/help-center/ai-models/how-do-i-use-soul-cinema) |
| **GPT Image 2.5 Sunburst** | Hassas düzenleme, "production-ready campaigns, polished product photography"; daha yavaş. Çok adımlı düzenlemede bozulma olmadığı iddiası. | GPT Image ailesi: "text rendering and precise color better than most" (help). GPT Image 2 için "accurate labels" (ürün fotoğrafçılığı sayfası). | Auto + desteklenen oranlar · 1K/2K/4K · kalite Low→Max · **16 referans** | Flare ile aynı: 1K Low 1,5 kr ($0,075); 2K High 5,5 kr ($0,275); 4K Max 26,5 kr ($1,325) | [blog](https://higgsfield.ai/blog/gpt-image-2-5-higgsfield) |
| **GPT Image 2.5 Flare** | Varsayılan; GPT Image 2'ye göre yaklaşık %50 daha düşük gecikme; sosyal içerik, hızlı varyasyon. | Yukarıdaki GPT Image iddiaları. | Sunburst ile aynı ayarlar | Sunburst ile aynı | [blog](https://higgsfield.ai/blog/gpt-image-2-5-higgsfield) |
| **Nano Banana 2.1** (Google) | Flash hızında, toplu tutarlılık ("up to 40 images from one reference while holding identity, product details and **label text**"). Düzenleme sohbetle yapılıyor. | "Labels… render spelled correctly" + çok dilli çeviri; Google'a göre metin render'ı NB 2'ye göre iyileşti. | 1K varsayılan / 2K / 4K; 512px–4K · 1:8, 8:1, 21:9, 9:21 dahil · **14 referans** (changelog: 4 karakter + 10 nesne; ürün sayfası: 5 karakter + 14 nesne, **çelişki**) | "Flash-tier, Pro'dan düşük", rakam yok **[doğrulanacak]** | [intro](https://higgsfield.ai/nano-banana-2-1-intro), [changelog](https://higgsfield.ai/creator-hub/changelog) |
| **Seedream 5.0 Pro** (ByteDance) | "Point-level editing" (etiket değiştirme dahil, maskesiz), tek geçişte infografik, web'den bilgi çekerek gerçek-zamanlı içerik. | "Native text in 14 languages" (changelog: 10+). Sayfa "fix a label" diyor. Türkçe listede açıkça geçmiyor **[doğrulanacak]**. | **Çelişkili:** sayfada hem "up to 2K" hem "up to 4K" var **[doğrulanacak]** | Dreamina'da 16 kr ([3. taraf/Higgsfield blogu] ≈$0,15); Higgsfield fiyatı yok **[doğrulanacak]** | [seedream-5.0-pro](https://higgsfield.ai/seedream-5.0-pro) |
| **Nano Banana Pro** (Google) | "Reasoning" ile prompt analizi; adet, metin, yüz ve perspektifte "en yüksek hassasiyet"; HEX/RGB marka rengi girişi. | Bu iddiayı en güçlü taşıyan model: "labels, packaging text… perfect spelling" (ai-image), "a product shot with text on the packaging: Nano Banana Pro" (blog). | 1K → 2K → native 4K · **14 referans** · Inpaint sürümü var | 2K: 2 kr (≈$0,10); 4K: 4 kr (≈$0,20) | [help](https://higgsfield.ai/creator-hub/help-center/ai-models/how-do-i-use-nano-banana), [kıyas](https://higgsfield.ai/blog/soul-2-vs-nano-banana-pro), [ai-image](https://higgsfield.ai/ai-image) |
| **FLUX 3 Image** (BFL) | Karmaşık prompt'a sadakat, hassas düzenleme; stiller: photo, illustration, poster, collage, editorial. | "Renders text more accurately in multiple languages" (BFL'e göre). | 768p / 1K / 1.5K / 2K / 4K (2K ve 4K native) · T2I + I2I · editörde run başına 4 varyanta kadar | Yok **[doğrulanacak]** | [changelog 1 Eki 2026](https://higgsfield.ai/creator-hub/changelog) (flux-3 sayfası video odaklı) |
| **Recraft V4.1** | Tasarım odaklı: kompozisyon, renk ve art direction. V4 ailesinde Styles (1–10 referansla stil eşleme) ve **Utility** ("flat light, frontal composition… mockups and product shots") da var. | Recraft "typography" alanını kapsıyor, ama spesifik etiket iddiası yok. **Vektör çıktı** var. | Standard/Pro, raster veya vektör · Styles: 1K/2K · Soul HEX desteği | Standard 1,25 kr; Std vektör 2,5; Pro 8; Pro vektör 10; Styles 1K 0,75 / 2K 1,75 (Ağu 2026) | [blog](https://higgsfield.ai/blog/recraft-v4-higgsfield) |
| **Grok Imagine 2.0** (xAI) | Higgsfield'de görsel modeli olarak **resmî kaynak bulunamadı**. Higgsfield sayfaları Grok Imagine'i video modeli olarak anlatıyor. | [3. taraf] Tipografi ve küçük metin okunabilirliğine vurgu var. | [3. taraf] 1K/2K, geniş oran yelpazesi | — | **[doğrulanacak]**; [3. taraf: runware](https://runware.ai/docs/models/xai-grok-imagine-image-2-0/guides) |
| **FLUX.2** (BFL) | Fizik/ışık tutarlılığı, **JSON yapılandırılmış prompt** (kamera, lens, ışık), **HEX renk** girişi. | "Legible text… infographics… accurate text rendering" iddiası. | "Higher resolution" deniyor, sayı yok **[doğrulanacak]** | Yok **[doğrulanacak]** | [flux-2-intro](https://higgsfield.ai/flux-2-intro) |
| **Z-Image** (Alibaba, açık kaynak) | Çok hızlı (1–3 sn), "minimally filtered"; konsept ve hızlı taslak. | Blog açıkça diyor ki: "Nano Banana Pro remains the king of typography". Z-Image yalnızca ambalaj **fikir taslağı** için. | Kare/dikey/yatay; sayı yok **[doğrulanacak]** | Yok **[doğrulanacak]** | [blog (Ara 2025)](https://higgsfield.ai/blog/Z-Image-New-from-Alibaba-in-AI-Image-Generation) |
| **Topaz** (upscaler) | Upscale, denoise, keskinleştirme, yüz iyileştirme, Recovery; istenen piksel boyutu. | Standard modlar "keeps original look". Generative modlar (Redefine) değişiklik ekler. [3. taraf/eski] "Text Refine" preset'i. | Herhangi bir piksel boyutu (ByteDance alternatifi: 2K/4K) | Yok **[doğrulanacak]** | [ai-image-upscaler](https://higgsfield.ai/ai-image-upscaler) |

**"Metin/etiket doğruluğu" iddiası taşıyanlar (iddianın gücüne göre, test edilmedi):**
1. **Nano Banana Pro:** Higgsfield'in kendi sayfaları en net iddiayı bu model için yapıyor ("perfect spelling", "packaging").
2. **Nano Banana 2.1:** Toplu üretimde "label text" tutarlılığı iddiası.
3. **GPT Image 2.5:** "text rendering and precise color".
4. **Seedream 5.0 Pro:** Çok dilli native metin ve "fix a label".
5. **FLUX 3 Image / FLUX.2:** Çok dilli metin iddiası.
6. Recraft daha zayıf bir iddia taşıyor.
- **Soul 2.0** için kaynak açıkça "metin güçlü yanı değil" diyor.
- **Z-Image** için kendi blogu tipografide NB Pro'yu üstün sayıyor.
- Higgsfield'in "Best AI Image Generators 2026" blogu ayrıca **Ideogram 4.5**'i "text in the frame" için öne çıkarıyor. Bu model kapsam dışı, ama changelog'a göre layout'u koruyarak metin değiştirme/çevirme yapıyor; test listesine eklenebilir.

---

## 3. Entegrasyon önerileri (öneri, kaynak bilgisi değil)

1. **Gerçek ürün fotoğrafını koruyan akış (öncelik 1):**
   - Akış: Gerçek ürün fotoğrafı → (gerekirse) **Upscale Standard** → **Relight** ile ışık → **Inpaint** ile yalnızca arka plan ve sahne değişikliği (etiket maskelenmez).
   - Her adımdan sonra etiketi orijinalle 100% zoom'da karşılaştırın.
   - Bozulma olursa etiket alanını orijinal fotoğraftan katman olarak geri koyun.
2. **Sahne üretimi + ürün yerleştirme (öncelik 2):**
   - NB Pro, NB 2.1 veya GPT Image 2.5 Sunburst'e ürün referansı (birkaç açı) verin; tam etiket metnini tırnak içinde yazın.
   - En az 3 modeli aynı brief'le kıyaslayın: etiket doğruluğu, logo ve kapak rengi. Marka renklerinde HEX girişi destekleyen modelleri tercih edin (NB Pro, FLUX.2, Soul HEX).
3. **Marka estetiği:** Soul 2.0 Moodboard (yüzsüz referanslar) yalnızca ürünsüz sahne ve arka plan için.
4. **Reels kapak / hero kare:** Cinema Studio'nun kamera/lens/diyafram kontrolleri. Çıktı video modeline başlangıç karesi olabilir.
5. **Toplu katalog/varyant:** NB 2.1 ("40 image" tutarlılık iddiası) test edilmeli. Web + Unlimited ile maliyet; MCP/CLI'de her zaman kredi düşer.
6. **Düşük öncelik:** Soul ID, Photodump, Face Swap, Character Swap (insan odaklı; rıza/KVKK riski).
7. **Erken test edilmesi gereken risk:** Marka logolu ürün referansı IP filtresine takılıyor mu? "I own the rights" butonu çıkıyor mu?

---

## 4. Bilgi bulunamayanlar / doğrulanacaklar

- **Cinematic Cameras:** Image menüsündeki bu adla resmî sayfa yok. Cinema Studio görsel modu varsayıldı.
- **Kredi bulunamayanlar:** Relight, Inpaint, Upscale (Topaz/ByteDance), Soul ID eğitimi, Moodboard oluşturma, Photodump, Soul Cinema, NB 2.1, FLUX 3 Image, FLUX.2, Z-Image ve Seedream 5.0 Pro'nun Higgsfield fiyatı. Pricing sayfası JS ile yükleniyor, metni alınamadı.
- **Grok Imagine 2.0 (görsel):** Higgsfield'de varlığına dair resmî kaynak bulunamadı; yalnızca 3. taraf xAI sayfaları var.
- **Seedream 5.0 Pro:** Maksimum çözünürlük çelişkili (2K / 4K), dil sayısı çelişkili (10+ / 14), Türkçe desteği açıkça yazmıyor.
- **NB 2.1:** Karakter/nesne sınırı çelişkili (4+10 / 5+14).
- **Create Image genel çözünürlük:** "native 4K" ile "native 2K + 4K refinement" ifadeleri çelişkili.
- **Ticari hak:** Face Swap/Character Swap sayfaları "paid Pro plans" diyor, ToU yardım sayfası plan şartı koymuyor.
- **Relight ve Inpaint:** Çıktı çözünürlüğü ve dosya sınırları kaynakta yok. Relight'ın arkasındaki model yalnızca 3. tarafa göre GPT Image 1.5/FLUX.2.
- **Topaz preset listesi ("Text Refine") ve 2x–16x ölçek:** Yalnızca 2025 tarihli, artık 404 veren bir sayfanın arama özetinden.
- **Soul Cinema:** En/boy ve çözünürlük değerleri ayrıca belirtilmemiş.
