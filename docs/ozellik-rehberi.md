# Higgsfield özellik rehberi: iş akışımıza nasıl girer?

Tarih: 26 Ekim 2026. Bu belge [özellik envanterindeki](ozellik-envanteri.md) özellikleri bizim işimize (çok markalı oto bakım ürünleri, Instagram post / Reels / reklam) bağlar. Önerilerin hiçbiri bizim ürünlerimizle test edilmedi; test planı 6. bölümde.

## 1. Kısa sonuç

- **Eski rehber yetersiz.** 16 Eylül araştırması ürün görseli odaklıydı. Bugünkü menüdeki özelliklerin büyük kısmını hiç içermiyor: Content Factory, Playable, Ads Studio, Ad Multiplier, Katana, AI Influencer, eklentilerin tamamı, Canvas, 3D Jutsu, Shorts Studio, Relight, Color Palette, Inpaint ve diğerleri. Bir kısmı (Ads Studio 1 Eki, Ad Multiplier 6 Eki, Content Factory 22 Eki, Playable 25 Eki) o tarihten sonra çıktı.
- **Bizim için en değerli yenilikler** (ürün doğruluğunu koruyarak üretim yapma potansiyeli en yüksek olanlar):
  1. **Photoshop ve Figma eklentileri:** AI çıktısı yeni katman olarak geliyor; gerçek ürün fotoğrafı ayrı katmanda dokunulmadan kalıyor.
  2. **Video Relight, Change Color Palette, Shorts Studio, Upscale (ByteDance / FLUX.3 precise):** Kendi gerçek çekimimizi yeniden üretmeden güzelleştiriyor.
  3. **Inpaint ve görsel Relight:** Gerçek ürün fotoğrafında yalnızca arka planı veya ışığı değiştirme.
  4. **Ads Studio:** Meta için toplu statik reklam (reklam başına 4 kredi). Ürün görselini koruyup korumadığı test edilmeli.
  5. **Canvas:** Aynı ürünü 3–4 modelde yan yana deneyip etiketi en iyi koruyanı seçme ve bunu şablon yapma.
  6. **Genjutsu Objects swap ve Ad Multiplier:** Tek gerçek çekimden çok markalı varyasyon. Etiket riski yüksek, ama getirisi de yüksek.
- **Bize az uyanlar:** Playable Ads (yalnızca Enterprise, uygulama reklamı içindir), Face Swap, Character Swap, Photodump, Soul ID (insan odaklı, KVKK riski).

## 2. Altın kural: ürün piksellerine ne kadar dokunuluyor?

Higgsfield'in hiçbir aracı etiketin birebir korunacağını garanti etmiyor. Kendi ürün fotoğrafçılığı sayfası da "her sonucu ürününüzle karşılaştırın" diyor. Bu yüzden araçları, ürünün gerçek piksellerine ne kadar dokunduklarına göre sıralıyoruz. Yukarıdan aşağıya risk artıyor:

| Seviye | Ne oluyor | Araçlar | Etiket |
|---|---|---|---|
| 0. Dokunmuyor | Gerçek ürün ayrı katmanda kalır, AI yalnızca etrafını üretir | Photoshop/Figma/After Effects katmanı, Blender'da gerçek etiket dokusu, Premiere/DaVinci'de AI B-roll | Korunur |
| 1. Renk/ışık | Gerçek görüntü korunur, yalnızca renk veya ışık değişir | DaVinci AI LUT, Color Palette, video Relight, Upscale (Standard/precise), Shorts Studio | Büyük ölçüde korunur; marka rengi ve parlama kontrol edilir |
| 2. Bölgesel | Seçilen bölge yeniden üretilir, dışı korunur | Inpaint, Draw to Edit, Seedance 2.5 Edit, Expand, Reframe | Etiket maskenin dışındaysa korunur |
| 3. Kareyle sabitleme | Video modeli ilk/son kareden başlar | Create Video ilk/son kare, Kling 4.0 keyframe, Veo 3.1 Fast, Grok 1.5 | Kilitli karelerde iyi, ara karelerde risk |
| 4. Referansla yeniden üretim | Model ürünü referanstan yeniden çizer | Marketing Studio, Ads Studio [doğrulanacak], Genjutsu swap, Katana, Cinema Studio, Nano Banana Pro… | Her karede kontrol şart |
| 5. Stilize | Ürün bir stile göre yeniden çizilir | Effects, Mixed Media, Genjutsu Styles, Explainer, Faceless, Content Factory | Gerçek ambalaj beklenmez |

**Kural:** Yayınlanacak işte etiketin okunduğu kare 0–2. seviyeden gelmeli. 3–5. seviye atmosfer, hook ve geçiş için kullanılır; etiketli kare kurguda gerçek packshot ile değiştirilir ya da üstüne bindirilir.

## 3. İçerik türüne göre iş akışları (öneri)

### 3.1 Instagram ürün postu / carousel
1. Gerçek ürün fotoğrafı → gerekirse **Image Upscale (ByteDance veya Topaz Standard)**.
2. Photoshop'ta ürünü kendi maskenle ayrı katmana al. **Generate AI Image** veya **Mockup Studio** ile arka planı ayrı katmanda üret. Alternatif: Figma'da post şablonu (logo, yazı vektör) + eklentiyle yalnızca arka plan.
3. Işık uyumu için **Relight**'ı ürünün kopya katmanında dene; etiket bozulursa etiket bölgesini orijinal katmandan maskeyle geri getir.
4. 1:1 → 4:5 / 9:16 türevleri için **Expand** (ürün katmanı yerinde kalır).
5. Hızlı fikir için: Create Image'da **Nano Banana Pro / GPT Image 2.5 / Seedream 5.0 Pro**'ya ürün referansı ver, etiket metnini tırnak içinde yaz. Bu çıktıyı taslak say; yayında ürünü gerçek katmanla değiştir.

### 3.2 Reels: gerçek uygulama çekiminden (en güvenli)
1. Telefon veya kamerayla gerçek çekim (pasta-cila, seramik, köpük yıkama).
2. **Shorts Studio** (stil, metin, overlay) veya Premiere/DaVinci'de kurgu.
3. **Video Relight** (ör. Contre-jour, Soft Cross) → **Color Palette** veya **DaVinci AI LUT** ile marka görünümü.
4. Yatay çekimse **Reframe 9:16**; ürün kadraj kenarındaysa sonucu kontrol et.
5. Aradaki atmosfer planları (su damlası, parlayan boya, garaj) için eklentiden **AI B-roll** (ürünsüz).
6. En son **Upscale: ByteDance veya FLUX.3 precise**. Topaz Video ve FLUX.3 creative kullanma (help center ürün ve metin içeren videoda önermiyor).

### 3.3 Reels: gerçek çekim yoksa
1. Gerçek packshot'ı **ilk ve son kare** yap (Create Video; Veo 3.1 Fast, Kling 4.0, MiniMax H3, Grok 1.5 adayları).
2. Hareketi yavaş tut; ürünün elde dönmesi, köpük altında kalması ve hızlı orbit etiketi en çok bozan durumlar.
3. Kamera hareketini önceden kilitlemek istersen **3D Jutsu** ile previz kur, MP4'ü video modeline referans ver.
4. Etiketin okunduğu anı kurguda gerçek packshot ile değiştir.
5. Taslakları 480p/720p'de üret (Seedance 2.5 8 sn: 24 kredi; 1080p: 128 kredi), finali 1080p'de üret, en son upscale et.

### 3.4 Meta / Instagram statik reklam seti
1. **Ads Studio**'da her marka için ayrı brand aç (logo, renk, font, ses tonu). Distribütör sitesinden içe aktarırken logonun bizim mi, üreticinin mi olduğunu elle düzelt.
2. Ürün başına önce 2–3 reklamlık deneme yap (8–12 kredi); etiket ve logo sadakatini kontrol et.
3. Fiyat/teklif açılı reklamlarda TL fiyatı ve iddiaları elle kontrol et.
4. Alternatif: Marketing Studio **Posters** (üretimden sonra katmanlarıyla düzenlenebilen tek kategori).

### 3.5 Video reklam varyasyonu
- Elimizde iyi performans gösteren gerçek çekimli bir reklam varsa: **Ad Multiplier → yalnız CTA veya hook değişimi** (720p'de en fazla ~35 kredi, kaynağın tahmini). En düşük riskli varyasyon budur.
- Aynı çekimde şişeyi başka markayla değiştirmek: **Genjutsu Objects swap** (≤30 referans, 15 sn 1080p 144 kredi) veya önce **Genjutsu Lite** ile ucuz deneme. Referans fotoğrafları kaynak videodaki açıya ve boyuta yakın çek; etiketi kare kare kontrol et.
- Beğenilen bir kurgu stilini kendi ürünümüzle kopyalamak: **Katana** (≤5 foto, yalnızca hakkı bizde olan referanslar).

### 3.6 Eğitici / eğlenceli içerik (ürünsüz)
- **Content Factory:** "Ya arabanı hiç yıkamasaydın?" gibi 15–60 sn'lik, yüzsüz Reels. 15 sn = 15,75 kredi. Türkçe seste aksan olabilir; önce 15 sn test.
- **Explainer:** Üretici sayfasından veya teknik föyden açıklama videosu (20 sn ≈ 72 kredi). Ürün stilize çizilir; teknik iddialar elle kontrol edilir.
- **Faceless Studio:** Seri kanal içeriği; 1 dk = 246 kredi, pahalı. Türkçe desteği doğrulanmadan yatırım yapılmamalı.

### 3.7 3D ürün sahnesi ve turntable
- **Blender eklentisi:** Şişe veya kutu gövdesini AI (3D Model sekmesi) ya da elle modelle. **Gerçek etiket dosyasını UV doku olarak kendin kapla.** Scene Builder'ı yalnızca ortam için kullan. Kendi Blender kameranla 9:16 turntable render al. Etiketin piksel düzeyinde doğru kaldığı AI destekli 3D reklam yolu bu.
- Bir kez kurulan "stüdyo sahnesi"ne farklı ürün modelleri değiştirilerek konabilir.

### 3.8 Tekrarlanabilir kampanya şablonu (çok marka)
- **Canvas:** [Gerçek ürün foto node'u] + [logo node'u] + [renk paleti] → 2–3 görsel model paralel → en iyi kare → Kling/Seedance node'una başlangıç karesi → Reels.
- Yeni ürün gelince yalnızca ürün node'u değişir. Seedance node'larında prompt'u referansın rolüyle başlat (ör. "PRODUCT: … is the exact product; keep label and logo unchanged").
- Unlimited Canvas'ta geçerli değil; Unlimited'ımız olan modelleri web ekranında kullan.

## 4. Hangi kanaldan kullanmalı?

| Kanal | Ne zaman | Kredi | Not |
|---|---|---|---|
| Web (higgsfield.ai) | Görsel keşif, tam şablon kütüphanesi (Marketing Studio 1.500+), Unlimited modeller, Genjutsu Lite "FREE" | Unlimited ve ücretsiz haklar **yalnızca burada** | |
| CLI + Claude Code / Codex | Tekrarlanan, kayıtlı, ürün doğruluğu hassas üretim (mevcut ana yolumuz) | Her üretim kredi | Higgsfield de kod ajanları için CLI'yi öneriyor |
| MCP (Claude Desktop / claude.ai) | Yalnızca MCP'de olan iş akışları: Katana, Content Factory, Ad Multiplier, Ad Localizer; eklenti kurulum komutları | Her üretim kredi; ücretli abonelik gerekir | Bağlanınca workspace'i doğrula |
| ChatGPT eklentisi | Kod bilmeyen ekip üyeleri | Her üretim kredi | Ses ve web sitesi yok |
| Masaüstü eklentiler | Gerçek ürün katmanını koruyan kompozit işler | Her üretim kredi (help-center) [AE blogu aksini söylüyor] | Yerel bilgisayar gerekir |
| API | İleride yüzlerce SKU için toplu katalog görseli | Ayrı USD bakiye | Marketing Studio Image ≈ $0,0059/görsel |

## 5. Hesap ve güvenlik notları

- **Marka/logo IP filtresi:** Prompt veya referansta marka adı ya da logo varsa üretim engellenebiliyor; kendi girdinde "I own the rights" butonu çıkabiliyor. Distribütörü olduğumuz markalarla ilk testte ölçülmeli. Marka sahiplerinden yazılı kullanım izni olması iyi olur.
- **Eğitim verisi:** Photoshop eklenti sayfası görsellerin eğitimde kullanılmadığını söylüyor; üçüncü taraf bir inceleme ise Team/Enterprise dışındaki planlarda yüklenen içeriğin kullanılabileceğini yazıyor [doğrulanacak: ToS ve plan kartı].
- **Ticari kullanım:** ToS çıktıyı kullanıcıya veriyor; Face/Character Swap sayfaları ücretli plan şartı koyuyor [çelişki].
- **AI karakter ve yüzler:** Rıza ve gerekiyorsa "yapay zekâ ile üretilmiştir" etiketi.

## 6. Önerilen test planı (ücretli, ayrıca onay ister)

Amaç: hangi aracın bizim etiketlerimizi koruduğunu ölçmek. Her testte aynı ürün (ör. RX Pro veya bir Gyeon şişesi), aynı referans seti; sonuç `higgsfield_test` üretim günlüğüne kaydedilir. Kredi rakamları kaynaktaki örnek fiyatlardır; gerçek tutar Generate düğmesinde veya `higgsfield generate cost` ile görülür.

| # | Test | Araç | Tahmini kredi |
|---|---|---|---|
| 1 | Gerçek fotoğrafta yalnızca arka planı değiştir, etiketi maskeleme | Inpaint (NB Pro, High) | [doğrulanacak] |
| 2 | Aynı fotoğrafa üst ışık ekle, etiketi %100 zoom'da karşılaştır | Relight (görsel) | [doğrulanacak] |
| 3 | Aynı brief, 3 model yan yana | Canvas: NB Pro / GPT Image 2.5 Sunburst / Seedream 5.0 Pro | ~2–6 kredi/görsel |
| 4 | 2–3 statik reklam | Ads Studio | 8–12 |
| 5 | Gerçek 15 sn çekime ışık ve renk | Video Relight + Color Palette | 42 + [doğrulanacak] |
| 6 | Packshot ilk/son kare, 5–8 sn, 720p | Kling 4.0 veya MiniMax H3 | 20–25 |
| 7 | Gerçek çekimde şişe değişimi | Genjutsu Lite (web, FREE hakkı varsa) → Objects swap | 32 → 104 (15 sn 720p) |
| 8 | Logo IP filtresi | Herhangi bir görsel model, marka logolu referans | Engellenirse çoğunlukla iade |
| 9 | Türkçe seslendirme | Content Factory 15 sn | 15,75 |

Eklenti testleri (Photoshop/Figma kompozit, Blender etiket dokusu) yerel bilgisayarda yapılır.

## 7. Eski rehberde güncellenmesi gerekenler

`higgsfield_test/docs/higgsfield-arastirma-2026-09-16.md` için:
- **Marketing Studio:** Help center'a göre MCP/CLI'de daha küçük bir preset seti var, tam 1.500+ şablon yalnızca web'de. 364 product_shots kaydı kataloğun bir alt kümesi olabilir.
- **Cinema Studio 4.0:** Klip 30 sn'ye, referans 50'ye çıktı; çözünürlük "1080p'ye kadar" (resmî).
- **Unlimited:** Web dışındaki kanallarda geçerli değil (resmî help-center) bilgisi eklenmeli.
- **CLI'nin ürün referansını iletmesi:** Help center, eski CLI/skill sürümlerinde referans görsellerin iletilmediği bilinen bir sorunu anlatıyor. Güncel sürüm kullanıldığı ve referansın gerçekten gittiği her koşuda kontrol edilmeli.
- **"İlgili özellikler" tablosu** bu repodaki envanterle değiştirilmeli ya da ona link verilmeli.

## 8. En önemli açık sorular

1. Ads Studio ve Marketing Studio ürün görselini pikseliyle mi koruyor, yeniden mi çiziyor?
2. Unlimited eklentilerde ve Supercomputer'da geçerli mi? (Kaynaklar çelişiyor.)
3. Menüdeki Genjutsu "FREE" etiketi Türkiye'deki hesabımız için ne ifade ediyor?
4. Türkçe seslendirme ve altyazı: Content Factory, Faceless, Explainer, Lipsync, Audio.
5. Adobe eklentisinin minimum sürümü (2024 mü 2025 mi), Photoshop panelinde 5 araç mı 12 araç mı var?
6. Relight, Inpaint, Upscale ve çoğu video modelinin kredi tutarı.
7. Content Factory görselleri kodla mı çiziyor (MCP talimatı) yoksa üretiyor mu (blog)? İki resmî kaynak farklı anlatıyor.
8. Audio menüsü ayrıca araştırılmalı.
