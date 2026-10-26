# B: Stüdyolar ve Reklam Araçları (Higgsfield), araştırma tarihi 26 Ekim 2026

Kapsam: Cinema Studio, Ads Studio (+ Ad Multiplier), Effects / Viral Presets, Marketing Studio, Click to Ad, Shorts Studio, Faceless Studio, Explainer, Create Video. Ek olarak kapsamla ilişkili yeni bir araç olan Content Factory'ye kısaca değinildi.

Yöntem: higgsfield.ai ürün sayfaları, /blog ve creator-hub/help-center WebFetch ile okundu. Higgsfield MCP araçları çağrılmadı, ücretli üretim yapılmadı.

Notasyon:
- **[doğrulanacak]**: kaynakta bulunamadı ya da kaynaklar çelişiyor.
- **(üçüncü taraf)**: Higgsfield dışı kaynak.
- **(geo.higgsfield.ai)**: Higgsfield'ın SEO amaçlı alt alan adı. Resmî blog/help center'dan daha zayıf kaynak sayıldı.
- Kredi→$ çevirileri kaynakların kendi varsayımıdır. Kaynakların çoğu Plus planını baz alır: "$49 / 1.000 kredi ≈ $0,05/kredi".

**16 Eylül'den sonra çıkanlar (tarihler kaynak meta verisinden):**
- Ads Studio: 1 Eki
- Yeni AI Influencer: 3 Eki
- Ad Multiplier: 6 Eki
- Click to Ad'ı anlatan "best-ai-platforms-create-ads-from-url" yazısı: 13 Eki
- Content Factory: 22 Eki

Cinema Studio için 4.0 (12 Ağu) sonrasında yeni bir sürüm (4.1 / 4.5) bulunamadı.

---

## Cinema Studio (güncel: 4.0)

**Ne yapıyor**
Sinematik video üretim stüdyosu. Kamera, lens, diyafram, ışık, renk ve oyunculuk duygusu sahne bazında kontrol edilir. Sahneler ayrı ayrı düzenlenir ve hikâye ileri ya da geri uzatılabilir. Help center'a göre 4.0 varsayılan olarak açılıyor ve üstteki seçiciden eski sürümlere (2.0–3.5) geçilebiliyor.

Giriş: https://higgsfield.ai/cinema-studio

**Nasıl kullanılır (4.0, Director's Panel)**
1. **Film Setup:** tür (General, Action, Epic, Drama, Comedy, Horror, Noir), dönem (Auto, 60s, 80s, 90s, 2000s, 2020s), tempo (Auto, Chaotic, Dynamic, Calm, Single Shot) seçilir.
2. **Kamera:** gövde (Auto, Modern, 35mm Film, 8mm Film, DV Camcorder), lens (Auto, Clean Sharp, Anamorphic, Vintage Anamorphic, Warm Vintage, Halation Vintage), diyafram (Auto, f/1.4, f/4, f/11) ve "30+" kamera hareketi preseti (POV, Robot Arm, Pan Left, Helicopter Shot…) ayarlanır.
3. **Işık:** Auto, Silhouette, Practicals, Window, Overhead Fall, Contre-jour, Soft Cross presetleri ya da manuel ayar (renk, parlaklık, difüzyon, açı) kullanılır.
4. **Renk paleti:** blog "50+" diyor. Aynı yazıda "45+" ve "30+" da geçiyor [doğrulanacak]. Help center "50+ color grading templates" diyor.
5. **Emotion Wheel:** Hope, Anger, Joy, Trust, Fear, Surprise, Sadness, Disgust duyguları ve bir yoğunluk/ifade kaydırıcısı var. Prompt içinde `@karakter Joy` şeklinde kullanılır.
6. **Sahne promptu** yazılır.
7. Generate. Ardından istenirse Color Grading yapılır (sıcaklık, kontrast, doygunluk, keskinlik, film grain, highlights, pozlama).

**Video modları (4.0)**
- References: yeni klip üretir.
- Forward / Backward Extend: yüklenen videoyu ileri ya da geri uzatır. Video en fazla 30 sn olabilir.
- Edit Video: bir nesne ya da yüz üzerinde bölgesel düzenleme yapar.

**AI Director / asistan**
- 3.5 ile gelen "Claude Chat AI Director" prompt kutusunun yanında duruyor.
- Tür, stil ve kamera ayarlarını değiştirebiliyor. Senaryoyu, kamera parametreleri önceden doldurulmuş çekimlere bölüyor.
- Generate'e kendisi basmıyor: kullanıcı onaylıyor.
- 4.0 blogu bu asistanı "Personal Assistant" diye anıyor.

**Takım özellikleri**
AI Cast, Cinematic Locations, Soul Cinema modelleri, Multi-Model (Seedance 2.5 dahil), canlı çok kullanıcılı üretim, Element paylaşımı, Canvas entegrasyonu, Project Brief, alt klasörler.

**Girdi ve çıktı**
- Girdi: prompt ve en fazla **50 referans** (görsel, video, Soul Cast karakteri). 3.5'te bu sınır 9'du.
- Çıktı: video. 2.5 ve sonrasında ses aynı geçişte native üretiliyor (SFX, konuşma, müzik).
- Help center'a göre 4.0 **Seedance 2.5** üzerinde çalışıyor.

**Süre ve çözünürlük**
- Klip başına **30 sn'ye kadar** (3.5'te 15 sn).
- Çözünürlük: blog SSS'si "up to 1080p" diyor.
- Bazı üçüncü taraf dizinler "native 4K" ve "yaklaşık 1 dk" diyor (üçüncü taraf, resmî kaynakla çelişiyor) [doğrulanacak].
- En-boy oranı listesi verilmemiş [doğrulanacak]. Create Video sayfasının SSS'si Cinema Studio için "21:9 aspect ratio alongside standard formats" diyor.

**Kredi / plan**
- Plana bağlı. Cinema Studio modelleri planınızın "Unlimited" listesindeyse kredi düşmüyor (help center).
- Üretim başına kredi tutarı kaynakta yok [doğrulanacak].

**Sınırlar**
- "May contain protected content" engeli çıkabilir. Gerçek yüzler ya da tanınabilir telifli içerik varsa üretim engellenebilir.
- 2.5 video yüklemesini kabul etmiyor. 3.0/3.5'te yükleme sınırı 15 sn, 4.0'da 30 sn.

**Öneri: iş akışımıza entegrasyon**
- Marka filmi / Reels hero sahneleri için kullanılabilir: garajda köpük yıkama, pasta-cila makinesi yakın çekimi, seramik kaplama boncuklanması (beading). Tür, ışık ve "Robot Arm" ile "Helicopter" hareketleri bu sahnelere uygun.
- 50 referans sınırı sayesinde aynı ürünün çok açılı fotoğrafları verilebilir.
- **Ürün doğruluğu riski yüksek.** Video modelleri şişe etiketindeki küçük metni (ör. Gyeon "Q² Mohs", Menzerna ürün kodları) bozabilir.
- Önerilen kullanım: ürünü uzak ya da arka planda tutan, etiketin net okunmadığı atmosfer çekimleri üretmek. Etiketin göründüğü kareleri gerçek packshot ile kurgu aşamasında değiştirmek ya da üstüne bindirmek. Edit Video (bölgesel düzenleme) ile etiket düzeltme denemesi yapılabilir ama sonucu [doğrulanacak].

**Kaynaklar**
- https://higgsfield.ai/cinema-studio
- https://higgsfield.ai/blog/cinema-studio-4-0 (2026-08-12)
- https://higgsfield.ai/creator-hub/help-center/tools/how-do-i-use-cinema-studio
- https://higgsfield.ai/blog/how-we-built-cinema-studio
- https://higgsfield.ai/create/video (21:9 notu)
- Üçüncü taraf (4K / 1 dk iddiası): https://yespress.io/higgsfield

---

## Ads Studio (ads_studio: brand / product / run) — YENİ (1 Eki 2026)

**Ne yapıyor**
Web sitesinden ya da elle girilen marka bilgisinden, satış açısına (fayda, fiyat/teklif, içerik/malzeme, kullanım şekli, yaşam tarzı) dayalı **statik** reklam kreatifleri üretiyor. Kreatifler metin ve görselden oluşuyor. Marka kiti kaydediliyor ve sonraki partilerde tekrar kullanılıyor.

Giriş: https://higgsfield.ai/ads-studio

**Kavramlar ve adımlar**
1. **Brand (marka kiti):** "Create my brand" ile web sitesi URL'sinden içe aktarılır ya da elle girilir.
   - Logo
   - Ana renk ve ek hex renkler
   - Fontlar (display ve body)
   - Ses tonu, hedef kitle, estetik
   - Açıklama, satış noktaları
   - Sosyal linkler (Instagram, TikTok, Facebook, Pinterest, YouTube)
   - Tüm alanlar düzenlenebilir.
2. **Product:** Siteden içe aktarılan katalogdan seçilir (ad, görsel, fiyat), ürün linki eklenir ya da manuel yüklenir.
3. **Run (üretim partisi):** Ürün başına **en fazla 20 reklam** seçilir. Toplam kredi üretimden önce gösteriliyor.
4. Sonuçlar incelenir ve seçilir. Chat'te "Mention a product" ile adet ve yeni açı yazılarak ek parti üretilir.
5. İndirilir ve reklam platformuna yüklenir.

**Çıktı**
- Statik reklamlar, başlık ve CTA ile. Formatlar **1:1, 4:5 ve 9:16**.
- Video reklam Ads Studio'nun ana akışında yok. Blog video için Marketing Studio'yu öneriyor. Video tarafı aşağıdaki **Ad Multiplier** ile geldi.
- Altta hangi modellerin kullanıldığı belirtilmemiş [doğrulanacak].

**Kredi**
- "Each ad costs 4 credits". Örnek: 20 reklam = 80 kredi ≈ $4 (kaynağın $0,05/kredi varsayımıyla).

**Sınırlar**
- Ürün başına bir partide en fazla 20 reklam.
- Plan kısıtı belirtilmemiş [doğrulanacak].

### Ad Multiplier (Ads Studio içinde) — YENİ (6 Eki 2026)

**Ne yapıyor**
Tek bir referans video reklamın hareketini, kadrajını, kesmelerini ve zamanlamasını koruyarak varyasyonlar üretiyor. Değiştirilebilen öğeler: ürün, oyuncu, kıyafet, mekân ve mesaj (hook, senaryo, CTA).

Erişim:
- Ads Studio > Explore tools > Ad multiplier
- Higgsfield MCP skill
- Supercomputer

**Adımlar**
1. Referans video yüklenir. Video **4–30 sn** olmalı.
2. **En fazla 20 görsel** eklenir (karakter, ürün, kıyafet).
3. Prompt'ta dosyalar `@` ile referans verilir.
4. Çözünürlük seçilir: **480p / 720p / 1080p**.
5. Butonda gösterilen kredi kontrol edilir ve üretilir.
6. Sonuçlar History'de incelenir.

**Kredi (kaynağın tahmini, Plus planı baz alınarak)**

| Değişiklik | Çözünürlük | Kredi (en fazla) |
|---|---|---|
| Hook + CTA | 720p | ~140 |
| Hook + CTA | 1080p | ~240 |
| Yalnız CTA | 720p | ~35 |
| Yalnız CTA | 1080p | ~60 |

480p fiyatı verilmemiş. Bir çalıştırmada üretilen maksimum varyasyon sayısı belirtilmemiş [doğrulanacak].

**Sınırlar**
- Yalnızca hakkına sahip olunan reklam ve görseller kullanılabilir. Gerçek kişiler için rıza gerekiyor.
- Blog sonuçlarda "ürün görünümü, metin ve iddiaları" kontrol etmeyi açıkça öneriyor.

**Öneri: iş akışımıza entegrasyon**
- Ads Studio'ya her marka (MG Polishing, Gyeon, Menzerna, Innovacar, Fra-Ber, Klin, Flex) için ayrı bir **brand** açılabilir. Distribütör sitemiz ürün kataloğu kaynağı olarak kullanılabilir.
- Meta reklamları için 1:1, 4:5 ve 9:16 statik A/B setleri üretilebilir. Maliyet düşük: 20 reklam ≈ 80 kredi.
- **Ürün doğruluğu riski:** Statik kreatiflerde ürün görselinin birebir mi korunduğu, yoksa AI ile yeniden mi çizildiği kaynakta belirtilmemiş [doğrulanacak]. İlk partide 2–3 reklamla etiket ve logo sadakati test edilmeli.
- Fiyat odaklı açılar (price/offer-led) TL fiyatlarla yanlış metin üretebilir. Fiyat ve iddia metni manuel kontrol edilmeli.
- **Ad Multiplier** için: elimizde iyi performans gösteren gerçek çekimli bir Reels varsa, CTA ya da hook değişikliği için en düşük riskli yol "Yalnız CTA, 720p" (~35 kredi). Ürünü değiştirme (ör. Gyeon yerine Menzerna şişesi) en riskli senaryo, çünkü etiket yeniden üretiliyor.

**Kaynaklar**
- https://higgsfield.ai/ads-studio
- https://higgsfield.ai/blog/higgsfield-ads-studio (2026-10-01)
- https://higgsfield.ai/blog/ad-multiplier-ads-studio (2026-10-06)

---

## Effects / Viral Presets

**Ne yapıyor**
Tek bir fotoğraftan, animasyon, mekân ve stili hazır gelen preset ile kısa video üretiyor. Prompt gerekmiyor.

Giriş:
- https://higgsfield.ai/viral-presets
- https://higgsfield.ai/effects ("Visual Effects" kataloğu)

**Nasıl kullanılır**
1. Preset seçilir.
2. Kaynak fotoğraf yüklenir ve çıktı ayarları seçilir.
3. Generate. Sonra indirilir ya da suite içinde düzenlenmeye devam edilir. İsteğe bağlı olarak Virality Predictor ile tahmin alınabilir.

**Katalog**
- Blog "more than 60 ready-made effects" diyor (14 Ağu 2026).
- Son güncellemede 13 yeni preset eklendi: Living paintings 6, Impossible rides 5, Cinematic reveals 2.
- /effects sayfasında 50 giriş var. Bunların 45'i benzersiz isim, bazıları tekrar ediyor.
- Sayfada "Now in ChatGPT" ibaresi var.
- Örnek efektler: Floating fall, Burning man, Comic, Particles, Bullet time, Lidar transition, Cutout, Vanish, Infinite clones, Palette.

**Çözünürlük ve en-boy oranı**
- Çoğu presette 480p–4K arası.
- Pearl Earring, Dolphin/Penguin Ride ve Skatedog en fazla 720p.
- Preset destekliyorsa dikey çıktı alınabiliyor.

**Kredi (720p, yeni presetler)**
- 27,5–67,5 kredi arası. Örnekler: Pearl Earring 27,5; Bullet Time 67,5; Agamemnon 67,5.
- Daha yüksek çözünürlük daha pahalı. 4K fiyatı verilmemiş.

**Sınırlar**
- Klip süresi, alttaki model ve kullanım kotası belirtilmemiş [doğrulanacak].
- Presetler yüz ya da ana özne odaklı. Ürün fotoğrafına özel kategori yok.

**Öneri: iş akışımıza entegrasyon**
- "Bullet time", "Particles", "Cutout", "Vanish" ve "Lidar transition" gibi efektler ürün fotoğrafıyla Reels "hook" anı (ilk 1–2 sn) için denenebilir.
- Presetler insan ve yüz için tasarlandığından ürün şişesinde sonuç öngörülemez [doğrulanacak]. Efekt sürecinde etiket deforme olma riski **yüksek**.
- Önerilen kullanım: kısa geçiş klibi olarak kullanmak ve finalde gerçek packshot ile kapatmak.
- Önce 720p, düşük kredili presetle (~28 kredi) test edilmeli.

**Kaynaklar**
- https://higgsfield.ai/viral-presets
- https://higgsfield.ai/effects
- https://higgsfield.ai/blog/how-to-make-viral-videos-viral-presets (2026-08-14)

---

## Marketing Studio (V2, güncel durum)

**Ne yapıyor**
Ürün linki ya da görselinden ürün çekimi, reklam görseli, pazaryeri görseli, poster, UGC video ve motion video üretiyor. Kütüphanede **1.500+ şablon** var.

Giriş:
- https://higgsfield.ai/marketing-studio
- Tanıtım sayfası: https://higgsfield.ai/marketing-studio-intro

**Kategoriler**
Blogda 6 kategori, güncel UI ve help center'da 7 kategori var (TikTok kategorisi eklenmiş).

| Kategori | Çıktı | Detay |
|---|---|---|
| Product Shot | Görsel | Studio / Lifestyle / With Model. With Model'de 20 avatar şablonu (blog) |
| Ads | Görsel | Meta ve Google yerleşim spesifikasyonlarına göre |
| Marketplace | Görsel | Pazaryeri listeleme görseli. Resmî uyumluluk garantisi yok |
| Posters | Görsel | Üretimden sonra **Higgsfield Layers** ile düzenlenebilen tek kategori (ürün, yerleşim, metin, öğeler) |
| UGC | Video | Faceless / Talking Head / Silent |
| Motion | Video | Hypermotion, 2D Product Motion, Mixed Media, Motion Design. Product Motion "Higgsfield Motion" üzerinde çalışıyor |
| TikTok | Video | Dikey video reklam |

Tanıtım sayfasındaki modlar: TV Spot, UGC, Tutorial, Product Review, Unboxing, UGC Virtual Try On, Hyper Motion, Pro Virtual Try On, Wild Card.

**Üretim yolları**
1. **Template:** Şablon seçilir, ürün görseli yüklenir (şablondaki ürünün yerine geçer), gerekirse avatar, hook ve mekân değiştirilir, "Recreate"e basılır. Kredi butonda görünür.
2. **Product Link:** Ürün sayfası linki yapıştırılır. Marka sinyalleri, görseller, logo, renkler ve metin otomatik çekilir. TikTok / Reels / Shorts için video reklam üretilir. Click to Ad bu yolun adı (aşağıda).
3. **Prompt:** Reklam tarif edilir, görsel ya da video seçilir, ürün ve avatar eklenir.
4. **Ad Reference:** Hakkına sahip olunan bir referans reklam yüklenir. Yapısı ürünümüzle yeniden kurulur.

**Avatarlar**
- Galeriden avatar, AI Influencer, kendi avatarımız ya da yeni avatar kullanılabilir.
- Aynı avatar tekrar kullanıldığında yüz sabit kalıyor.
- Tanıtım sayfası hem "100+" hem "40+" avatar diyor [doğrulanacak]. Özel avatar Soul 2.0 ile üretiliyor.

**Süre ve çözünürlük**
- Video süresi: 18 Ağu blogu UGC ve Motion için "up to 15 seconds" diyor. 13 Eki blogu "UGC Videos and Motion generate video up to 30 seconds" diyor. Süre 30 sn'ye çıkmış olabilir [doğrulanacak].
- Video çözünürlüğü: 720p (fiyat tablosu).
- Görsel çözünürlüğü: 2K.
- En-boy oranı listesi verilmemiş [doğrulanacak]. Örneklerde 9:16 kullanılıyor.

**Kredi (kaynak tabloları)**

| Kalem | Kaynak 1 (18 Ağu) | Kaynak 2 (19 Ağu) |
|---|---|---|
| Video 8 sn 720p | 47,62 kredi | – |
| Video 15 sn 720p | 89,2 kredi | – |
| Motion 15 sn 720p | – | 89 kredi |
| Product Shot 2K | 1,5 kredi | 8 kredi |
| Marketplace banner 2K | – | 8 kredi |
| Poster 2K | 7,5 kredi | – |

İki blog Product Shot 2K fiyatında çelişiyor (1,5 ve 8 kredi) [doğrulanacak]. Kesin fiyat Generate butonunda görülmeli.

**Sınırlar**
- UGC'de seslendirme ve tempo değişken. Yayın öncesi kontrol öneriliyor.
- Posters dışındaki görseller yeniden üretilerek değiştiriliyor. Help center görsellerin My generations'ta metin, kırpma, arka plan ve ışık açısından düzenlenebildiğini söylüyor. Video ancak yeniden üretilerek değiştirilebiliyor.
- **MCP üzerinden daha küçük bir preset seti var**, tam şablon kütüphanesi yalnızca web'de. MCP üretimleri her zaman kredi düşüyor. CLI ve MCP ile yaptığımız 16 Eylül incelemesi bu yüzden kataloğun bir alt kümesini görmüş olabilir.
- URL'den çekim başarısız olursa ürün görselini doğrudan yüklemek gerekiyor.
- Marketplace çıktısı her platformun kendi kurallarına göre kontrol edilmeli (Trendyol, Hepsiburada).

**Öneri: iş akışımıza entegrasyon**
- Kendi beyaz fonlu packshot'larımızla **Product Shot (Studio / Lifestyle)** ve **Posters** en kontrollü yol. Posters katman düzenlemesi sayesinde yanlış metin elle düzeltilebiliyor.
- **Ürün doğruluğu riski:** Görselde ürünün piksel olarak korunduğu garanti edilmiyor [doğrulanacak]. Etiket metni, ml bilgisi ve logo her çıktıda kontrol edilmeli.
- UGC ve Motion videolarında risk daha yüksek. Kısa, ürünün sabit durduğu şablonlar tercih edilmeli.
- Web'de 7 kategori ve 1.500+ şablon olduğundan, CLI'de bulunmayan şablonlar web arayüzünden denenmeli.

**Kaynaklar**
- https://higgsfield.ai/blog/new-marketing-studio-higgsfield (2026-08-18)
- https://higgsfield.ai/blog/ai-ecommerce-ads-2026 (2026-08-19)
- https://higgsfield.ai/creator-hub/help-center/tools/how-do-i-use-marketing-studio-to-create-video-ads
- https://higgsfield.ai/marketing-studio-intro
- https://higgsfield.ai/blog/best-ai-platforms-create-ads-from-url (2026-10-13)

---

## Click to Ad (ürün URL'sinden video reklam)

**Ne yapıyor**
Marketing Studio içindeki URL akışı, "fastest entry point inside Marketing Studio for a single video ad from one link". Link yapıştırıldığında ürün adı, açıklama, **en fazla 8 fotoğraf**, marka renkleri ve logo otomatik çekiliyor. Kullanıcı bunları kontrol edip düzeltiyor, şablon seçiyor ve video üretiyor.

Giriş:
- https://higgsfield.ai/click-to-ad şu an Marketing Studio sayfasına düşüyor.
- Ayrı bir Click to Ad landing sayfası doğrulanamadı [doğrulanacak].

**Nasıl kullanılır**
1. Marketing Studio > Product Link (Click to Ad) açılır.
2. Ürün URL'si yapıştırılır.
3. Çekilen isim, açıklama, fotoğraflar (en fazla 8), renk ve logo kontrol edilir. Yanlış olanlar değiştirilir.
4. Şablon seçilir. Arama sonuçları "10 preset" diyor (Higgsfield kaynaklı SEO metni, doğrudan okunamadı) [doğrulanacak].
5. Generate.

**Süre ve çözünürlük**
- Click to Ad'e özel resmî rakam yok.
- Arama özetlerinde "8 sec, 720p" fiyat satırı ve "15 sn sınırı" geçiyor. Kaynak sayfalar 404 döndü [doğrulanacak].

**Kredi**
- Click to Ad'e özel bir rakam bulunamadı [doğrulanacak].
- Marketing Studio'da 8 sn 720p video 47,62 kredi. Click to Ad'in de bu tarifeyle fiyatlandığı varsayılabilir ama doğrulanmadı.

**Sınırlar**
- Sayfada en az bir net ürün fotoğrafı olmalı.
- Fiziksel ve belirgin şekilli ürünlerde daha iyi çalıştığı söyleniyor (arama özeti) [doğrulanacak].
- URL çekimi hatalıysa görsel manuel yüklenmeli (help center).

**Öneri: iş akışımıza entegrasyon**
- Kendi e-ticaret ürün sayfamız (ya da markanın resmî ürün sayfası) ile hızlı bir 9:16 taslak reklam üretilebilir.
- Çekilen 8 fotoğraf mutlaka kontrol edilmeli. Pazaryeri sayfalarında farklı satıcıların düşük kaliteli ya da yanlış ürün fotoğrafları bulunabiliyor, bu yüzden **kendi sayfamızı** kullanmak gerekiyor.
- Distribütör sitemizde logo olarak bizim logomuz, ürün olarak üretici markanın (ör. Menzerna) etiketi çekilebilir. Marka karışması riski var. Logo alanı manuel ayarlanmalı.
- Video modeli etiketi yeniden çizer. Final kesimde gerçek packshot overlay'i öneriliyor.

**Kaynaklar**
- https://higgsfield.ai/blog/best-ai-platforms-create-ads-from-url (2026-10-13; "up to 8 photos")
- https://geo.higgsfield.ai/blog/app-generate-social-media-ads-shopify-url (geo.higgsfield.ai; 24 Eki 2026'da kontrol edildiği yazıyor)
- https://higgsfield.ai/creator-hub/help-center/tools/how-do-i-use-marketing-studio-to-create-video-ads (Product Link modu)

---

## Shorts Studio

**Ne yapıyor**
**Mevcut videoyu** stil presetleriyle dikey kısa formata (9:16) dönüştürüyor. Metinden video üretmiyor.

Giriş: https://higgsfield.ai/shorts-studio

**Nasıl kullanılır**
1. Video kırpılır (preset yüklenen videonun tamamına uygulanıyor).
2. Studio açılır. Video solda, preset kütüphanesi sağda görünür.
3. Preset seçilir. Kütüphanede "40+ styles" var (Bold Urban, Green Contrast, Urban Serenity, Warm Glow…). Ya da "Create a Preset from References" ile özel preset oluşturulur.
4. Generate. Üretim arka planda çalışıyor ve sıraya birden fazla iş konulabiliyor.
5. İnceleyip dışa aktarılır (MP4).

Presetler görünüm, metin işleme ve grafik overlay ekliyor.

**Sınırlar**
- Girdi klip başına **en fazla 2 dk**.
- Çıktı **720p**.
- Tam senkron altyazı için LipSync Studio öneriliyor.
- Ses ve dil özellikleri anlatılmamış [doğrulanacak].
- Kaynak bir yerde "16:9 horizontal 720p" çıktısından da bahsediyor. Bu, gövde metniyle çelişiyor [doğrulanacak].

**Kredi**
- "~$4 per 25-sec clip" (720p). Fiyat Temmuz 2026'da doğrulanmış.
- "Basic from $9/mo".
- Tüm araçlar aynı kredi bakiyesini kullanıyor.

**Öneri: iş akışımıza entegrasyon**
- Gerçek çekim uygulama videolarımız (pasta-cila, seramik uygulama) bu araç için en uygun girdi. Ürün görüntüsü üretilmediği için **etiket doğruluğu riski düşük**. Preset yalnızca stil, metin ve overlay ekliyor.
- Yine de stil presetlerinin renk derecelemesi ürün rengini (ör. Menzerna kapak renk kodları) değiştirebilir. Kontrol edilmeli.
- Özel preset ile marka renklerine uygun tekrar kullanılabilir bir şablon kurulabilir.
- 720p sınırı Reels için kabul edilebilir ama ideal değil.

**Kaynaklar**
- https://higgsfield.ai/blog/how-to-make-youtube-shorts-with-ai (2026-07-02)

---

## Faceless Studio

**Ne yapıyor**
Kanal açıklaması, stil ve anlatıcı seçimiyle **tam animasyonlu "yüzsüz" bölüm** üretiyor: senaryo, seslendirme, 2D/3D animasyon, müzik ve altyazı tek videoda birleşiyor. Supercomputer içinde bir skill olarak başladı, artık bağımsız bir araç.

Giriş: https://higgsfield.ai/faceless-studio

**Nasıl kullanılır**
1. **Senaryo seçimi:** tek satırlık kanal tanımı yazılır. Önerilen 4 konudan biri seçilir, ya da özel konu yazılır, ya da hazır senaryo dosyası yüklenir. İsteğe bağlı olarak referans YouTube linki eklenir.
2. **Bölüm ayarları:**
   - En-boy: 16:9 ya da 9:16
   - Süre: 1–5 dk
   - Animasyon: Fully animated ya da Frame by Frame
3. **Stil:** 12 preset var. Editorial Motion Graphics, Stickman Cartoon, Fairy Tale & Myth, Paper Diorama, Hand Drawn, Mannequin, Poster Vector, Colorful 3D, Watercolor Chronicle, Paper Collage, Studio 3D, Pastel Flat 2D.
4. **Anlatıcı sesi:** seçilen ses kanalın sesi olarak kaydedilir. Ses seçimi fiyatı etkilemiyor.
5. Generate. Tahmini süre "up to 30 minutes".

"My Channels" sekmesi her kanalın stil, ses, karakter ve bölümlerini saklıyor.

**Kredi**
- 1 dk bölüm 246 kredi (~$12,30).
- 5 dk bölüm 1.230 kredi (~$61,50).
- Kesin fiyat Generate butonunda görünüyor.

**Sınırlar**
- Bölüm en fazla 5 dk. Supercomputer'daki faceless skill 10 dk'ya kadar çıkıyor.
- Kanal kategorileri: Education, History, Kids, Storytelling.
- Altyazı ve ses dil desteği (Türkçe) belirtilmemiş [doğrulanacak].

**Öneri: iş akışımıza entegrasyon**
- Eğitim içerikleri için düşünülebilir: "Pasta-cila nedir", "Seramik kaplama nasıl çalışır" serisi, Editorial Motion Graphics ya da Studio 3D stilinde.
- **Ürün doğruluğu:** Bu araç gerçek ürün görseli koruma amaçlı değil, animasyon stili üretiyor. Ürün ve marka adı geçen sahneler yanlış ambalaj çizebilir. Markasız, genel eğitim içeriği için uygun.
- Türkçe seslendirme desteği doğrulanmadan yatırım yapılmamalı.
- Maliyet görece yüksek (1 dk = 246 kredi).

**Kaynaklar**
- https://higgsfield.ai/blog/faceless-youtube-videos-faceless-studio (2026-08-21)
- https://higgsfield.ai/blog/start-faceless-channel-with-ai (2026-10-06; Faceless Studio'ya yalnızca link veriyor)

---

## Higgsfield Explainer

**Ne yapıyor**
Bir konu, URL ya da dosyadan **10 dakikaya kadar yapılandırılmış açıklama videosu** üretiyor. Çıktı birleştirilecek klipler değil, bitmiş video. Cinema Studio, Marketing Studio ve genel video üreticiden ayrı bir araç.

Giriş: https://higgsfield.ai/explainer (sayfa gövdesi WebFetch ile okunamadı)

**Nasıl kullanılır**
1. **Preset seçilir.** Pixel Art, Claymotion, Mixed Media, 3D Papercraft, 2D Illustrator, Whiteboard Doodle. Meta veride "10+" preset yazıyor.
2. **Girdi verilir:**
   - "What should the video explain?" alanına konu yazılır, ya da
   - "Attach files" ile foto/doküman eklenir, ya da
   - "Link" ile URL verilir. Ürün sayfası, makale ve dokümantasyon örnek olarak geçiyor.
3. **Ayarlar:**
   - En-boy: varsayılan 16:9. Dikey ve kare seçenekleri de var ama oranlar adlandırılmamış.
   - Süre: 20 sn, 30 sn, 1 dk, 3 dk, 5 dk, 10 dk ya da Manual.
   - Ses: "40+" ses preseti ya da özel ses.
4. Generate.

**Kredi**
- 20 sn ≈ 72 kredi (~$3,60).
- 1 dk "orantılı olarak daha fazla", rakam verilmemiş.
- 3 dk ve üzeri "typically exceed $20".

**Sınırlar**
- En fazla 10 dk.
- Dil desteği, dosya boyutu ve URL kısıtları belirtilmemiş [doğrulanacak].

**Öneri: iş akışımıza entegrasyon**
- Ürün teknik föyü ya da üretici ürün sayfası URL'si ile "Ürün nasıl kullanılır" açıklama videosu üretilebilir (ör. Menzerna pasta kademeleri, Gyeon kaplama uygulama adımları). 9:16 seçeneği doğrulanırsa Reels için de kullanılabilir.
- **Ürün doğruluğu:** Stilize presetler (clay, papercraft, illüstrasyon) ürünü yeniden çizer. Gerçek ambalaj beklentisi olmamalı. Teknik iddialar (dilüsyon oranı, kür süresi) URL'den çekilen metne dayandığından **içerik doğruluğu manuel kontrol edilmeli.**
- Türkçe seslendirme desteği [doğrulanacak].

**Kaynaklar**
- https://higgsfield.ai/blog/ai-video-from-text-and-url (2026-07-14)
- https://higgsfield.ai/explainer

---

## Create Video (genel video üretim ekranı)

**Ne yapıyor**
Model seçip prompt ve isteğe bağlı referans görselle video üretilen genel ekran.

Giriş:
- https://higgsfield.ai/create/video
- Üst menüdeki "Video" sekmesi

**Modeller**
- Sayfada listelenenler: Kling 3.0, Seedance 2.0, Wan 2.7, Kling o1, Sora 2, Veo 3.1, Kling 2.6.
- Footer'da Seedance 2.5, Wan 2.6, Grok Imagine ve MiniMax linkleri var.
- Güncel tam liste [doğrulanacak].

**Nasıl kullanılır (help center)**
1. Video > model ya da özellik seçilir.
2. Prompt yazılır.
3. Model destekliyorsa referans görsel yüklenir.
4. Süre, en-boy oranı ve çözünürlük ayarlanır.
5. Generate.

Sonuçlar ilgili bölümde ve Assets'te görünüyor. Üretim genellikle "birkaç dakika" sürüyor.

**Ayarlar**
- "First and Last image reference": ilk ve son kare kilitleme.
- Ses aç/kapa. Seedance 2.0 ve Kling 3.0 native ses üretiyor.
- UI önizlemesinde "8s" ve "Auto" en-boy görülüyor.
- Veo 3.1 kartında "4K generation" yazıyor.
- Model başına süre ve çözünürlük aralıkları sayfada yok [doğrulanacak].

**Kredi / plan**
- Abonelik olmadan ilk videolar üretilebiliyor.
- "Some models, features, and higher usage tiers may require a paid plan."
- Kredi rakamları sayfada yok. Generate butonunda gösteriliyor.

**Öneri: iş akışımıza entegrasyon**
- **First/Last frame kilitleme** ürün doğruluğu için en değerli ayar. İlk ve son kare olarak gerçek packshot verilirse açılış ve kapanışta etiket doğru kalır. Ara karelerde bozulma riski devam ediyor.
- Seedance 2.5 (Cinema Studio 4.0'ın altyapısı, 50 referans) ile ürün referansı ağır üretim için ayrı bir test önerilir. Ecommerce blogunda Seedance 2.5 Direct Control 15 sn 720p = 98 kredi, 30 sn = 195 kredi.

**Kaynaklar**
- https://higgsfield.ai/create/video
- https://higgsfield.ai/creator-hub/help-center/getting-started/how-do-i-create-my-first-generation
- https://higgsfield.ai/blog/ai-ecommerce-ads-2026 (Seedance 2.5 fiyatları)

---

## Ek: Content Factory (kapsam dışı ama yeni, 22 Eki 2026)

"What if…" sorusundan yüzsüz kısa video ya da seri üretiyor.
- 50+ preset
- 1–4 bölüm
- 15 sn – 5 dk
- 9:16 çıktı
- İsteğe bağlı TikTok/Instagram referans linki

Fiyat: 15 sn = 15,75 kredi, 1 dk = 63 kredi.

Ses dili prompt'un dili ile belirleniyor. İngilizce ve Rusça dışındaki dillerde aksan olabilir, bu Türkçe için uyarı niteliğinde.

Giriş: https://higgsfield.ai/content-factory. MCP'de `/content-factory` ile de erişiliyor.

Kaynak: https://higgsfield.ai/blog/higgsfield-introduces-content-factory

Öneri: Markasız eğlenceli hook içerikleri için ucuz bir seçenek ("What if seramik kaplama olmasaydı?"). Ürün doğruluğu için uygun değil.
