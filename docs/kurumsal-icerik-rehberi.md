# Kurumsal içerik rehberi: markalarımız ve ürün ailelerimiz için Higgsfield yol haritası

Tarih: 26 Ekim 2026. Kaynaklar `higgsfield_test` reposundaki kayıtlar: marka kütüphanesi (`brands/`), 639 SKU'luk ürün açıklamaları (`brands/sources/product-descriptions-2026-09-16.jsonl`), yaratıcı yön arşivi (`creative/README.md`) ve RX Pro kampanya kaydı. Higgsfield araç bilgileri bu repodaki [özellik rehberi](ozellik-rehberi.md) ve [envanterden](ozellik-envanteri.md).

"**Öneri**" diye işaretli her şey bizim yorumumuzdur; marka kılavuzu kuralı ya da test edilmiş reçete değildir. Hiçbir öneri henüz kendi ürünlerimizle denenmedi.

## 1. Biz kimiz? (kayıtlara göre)

- Araç bakım ürünleri satan, çok markalı, kurumsal bir firma. Kayıtlarda 15 marka/kimlik ve 639 SKU var.
- **Kendi kimliklerimiz:** MG POLISHING (kurumsal kimlik), MG PS (ürün markası; makineler ve kil ürünleri), MG PADS (sünger ve keçe ailesi). MX-PRO kayıtlarda "MTS KİMYA MX-PRO" başlığıyla geçiyor; kendi markamız mı, dağıtımını yaptığımız bir marka mı [doğrulanacak].
- **Dağıtımını yaptığımız markalar:** Menzerna, GYEON, Innovacar, Fra-Ber, FLEX, KLIN, Little Joe, IK Sprayers, EPOCA, SGCB, Q1 Tapes.
- **Duruş:** Trendleri takip ediyoruz ama ana çizgimiz **profesyonel görsel ve video**. Hedef kitle yalnızca son kullanıcı değil; profesyonel detailing ve pasta-cila uygulamacıları, PPF/cam filmi ustaları ve bayiler de var (RX Pro kaydında öncelikli kitle "profesyonel uygulamacı" olarak önerildi).

### Ürün dağılımı (SKU sayısı, ürün açıklamaları kaydı)

| Marka | SKU | Ağırlıklı ürünler |
|---|---|---|
| GYEON | 140 | Q² kaplamalar, Q²M bakım ürünleri, mikrofiber/aplikatör, cam ürünleri, PPF bakım |
| Fra-Ber | 112 | Profesyonel yıkama ve temizlik kimyasalları (konsantre, bidon), iç temizlik, koku, hızlı cila |
| Little Joe | 71 | Araç kokuları (çok sayıda koku varyantı), kurutma makinesi koku kapsülü |
| Menzerna | 64 | Polisaj pastaları ve cilalar (kesimden finişe), pasta süngerleri, kuzu yünü keçeler |
| SGCB | 49 | PPF/cam filmi aparatları, hava ve su tabancaları, fırçalar, atölye ekipmanı |
| FLEX | 36 | Polisaj makineleri, aydınlatma, akü, tabanlık, taşıma sistemleri |
| Innovacar | 34 | Yıkama şampuanları, su izi ve kireç ürünleri, seramik bazlı koruma, hızlı cila, kova |
| MG PADS | 32 | Pasta, cila ve hare giderici süngerler (çok çaplı), kuzu postu keçeler |
| IK Sprayers | 30 | Basınçlı pompalar (alkali, asit, solvent, gıda), köpük pompaları, PPF pompası, yedek kitler |
| KLIN | 25 | Mikrofiber havlu ve bezler, yıkama eldiveni, aplikatör, önlük |
| EPOCA | 23 | Kimyasal dayanımlı sprey şişe ve basınçlı pompalar, püskürtücü başlıklar |
| MG PS | 12 | Polisaj makineleri (RPV001, RPV002 / RX PRO, OPV001), kil ürünleri |
| MX-PRO | 6 | Seramik kaplama kutu setleri (CRYSTAL, DIAMOND Plus) |
| Q1 Tapes | 5 | Maskeleme bantları |

## 2. Kurumsal kalite çıtası

Bu ilkeler her planın ön koşuludur.

1. **Profesyonel gerçeklik, efektten önce gelir.** Ürün, ambalaj, etiket ve logo gerçek ürünle birebir aynı olmalı. Higgsfield'in hiçbir aracı bunu garanti etmiyor; etiketin okunduğu her kare gerçek fotoğraf veya çekimden, ya da ürün piksellerine dokunmayan bir araçtan gelir. Seviye tablosu: [özellik rehberi, 2. bölüm](ozellik-rehberi.md#2-altın-kural-ürün-piksellerine-ne-kadar-dokunuluyor).
2. **Yapay zekânın rolü: ortam, ışık, atmosfer ve geçiş.** Ürünün kendisi değil (öneri).
3. **İddialar SKU kaynağından gelir.** Sayısal değerler, koşullar, hacim ve set içeriği yalnızca seçilen SKU'nun açıklamasından veya üretici belgesinden alınır. "36 aya kadar" gibi koşullu ifadeler koşuluyla birlikte yazılır. Kaynakta olmayan indirim, stok, sertifika ve garanti eklenmez.
4. **Sahte sonuç yok.** Önce/sonra karşılaştırması grafikle abartılmaz (Innovacar sosyal medya kılavuzu, s.21). Bir AI su boncuklanması sahnesi ürünün gerçek test sonucu gibi sunulmaz. Ekran, gösterge veya ölçü değeri uydurulmaz (RX Pro kaydı: "ekrana yapay değer basılmaz").
5. **Marka kimlikleri karışmaz.** Her üretimde tek ana marka olur. Distribütör kimliği (MG POLISHING) ile ürün markası ayrı alanlarda durur.
6. **Yazı tasarım katmanında, ürün üzerinde değil.** Başlık, madde ve CTA Figma, Photoshop veya kurgu programında eklenir; AI'a yazdırılmaz (öneri). Ürünün üzerindeki gerçek yazı ayrıca korunur.
7. **Her çıktı kontrol edilir.** Etiket ve logo %100 büyütmede gerçek ürünle karşılaştırılır; videoda klip baştan sona izlenir. Kayıt `higgsfield_test` üretim günlüğüne girer.

## 3. Marka kuralları ve Higgsfield'deki karşılığı

Kurallar `higgsfield_test/brands/<marka>/README.md` kaynaklarından özetlendi. Ayrıntı ve sayfa numaraları oradadır.

| Marka | Kılavuzdan gelen kural | Higgsfield'de ne demek? (öneri) |
|---|---|---|
| **Menzerna** | Beyaz logo zemini tercih edilir; logo fotoğraf veya belirgin gradyan üzerine doğrudan konmaz. Wordmark yeniden yazılmaz, esnetilmez. Min. 20 mm. Kırmızı #CD1316. Kesim → finiş aşama sistemi | Logo AI sahnesinin üstüne değil, tasarım katmanında beyaz alanda durur. Ads Studio / Marketing Studio otomatik logo yerleşimi bu kuralı bozabilir; çıktı kontrol edilir |
| **Innovacar** | Doğrudan, dürüst teknik dil. Renkli logo yalnızca beyaz zeminli ambalajda. "by FRA-BER" kilidi kurumsal iletişim içindir, kampanyada dayatılmaz. Ürün ailesi renkleri ayrı. Kalabalık kadraj ve sahte önce/sonra yok. Makro detay uygun. Koyu ortam ürün rengini vurgulamak için kullanılabilir. VOLT #D4F205 | `koyu-urun` yönü + makro gerçek çekim. Effects/viral efekt bu kılavuzla çatışabilir; yalnızca ürünsüz hook planında. Su izi / kireç ürünlerinde AI "önce-sonra" üretilmez |
| **Fra-Ber** | Saygılı, teknik, profesyonel ton. Logo yeniden oluşturulmaz. Hobi ve profesyonel ürün ailelerinin ambalaj ve renk ayrımı korunur. Mavi #004C94 | Bidon / konsantre ürünlerde dilüsyon bilgi kartı (SKU'dan). Hobi ve pro ürünü aynı karede karıştırılmaz |
| **GYEON** | Q² / Q²M, EVO, REDEFINED ve hacim seçilen ambalajdan aynen doğrulanır. Certified Detailer serisi, çekimdeki işletmenin yetkili olduğunu göstermez. Resmî renk ve font bilinmiyor | AI ürünü yeniden çizerse EVO/REDEFINED yazıları ve kapak rengi karışabilir; bu seride etiketli kareler gerçek fotoğraftan gelir. Uygulamacı ya da işletme "sertifikalı" gibi sunulmaz |
| **FLEX** | Söylem "this is proformance"; "performance" diye düzeltilmez. Tam model kodu, taban çapı, kablolu/akülü ayrımı kontrol edilir | Makine görsellerinde model kodu ve akü/kablo doğruluğu ilk kontrol. Prompt'ta "proformance" yazımı korunur |
| **MG ailesi** | MG POLISHING = kurumsal kimlik, MG PS = ürün markası, MG PADS = ayrı ürün ailesi, makinedeki "MG PS POLISHER" işareti özgün fotoğrafta korunur | Lansmanlarda model adı büyük olabilir; yeni logo icat edilmez. Kurumsal imza küçük ve ikincil |
| **Diğerleri** (KLIN, Little Joe, IK, EPOCA, SGCB, MX-PRO, Q1) | Tam kılavuz yok; yalnızca sağlanan logolar. Ölçülen renkler resmî palet değil | Resmî renk/font varsayılmaz. Logo kendi dosyasından eklenir |

**Ads Studio ve marka kiti için öneri:** Ads Studio "brand" kaydı web sitesinden logo, renk ve font çeker. Distribütör sitemizden içe aktarırken çekilen logonun MG POLISHING mi, üretici markası mı olduğu karışabilir. Her üretici marka için ayrı brand açılıp logo, renk ve font yukarıdaki kurallara göre **elle** düzeltilmeli. Kılavuzu olmayan markalarda renk ve font alanları boş bırakılmalı [Ads Studio'nun boş alanla davranışı doğrulanacak].

## 4. Ürün ailelerine göre içerik tarifleri

Her ailede aynı yapı: neyi göstermek istiyoruz, nerede risk var, Higgsfield'de hangi zincir, neyi yapmayız. Zincirlerin ayrıntısı ve canlı kontrol komutları [araç seçim haritasında](../.claude/skills/higgsfield-planla/references/arac-secim-haritasi.md).

### 4.1 Polisaj makineleri — MG PS (RPV001, RX PRO / RPV002, OPV001), FLEX

- **Göstermek istediklerimiz:** Alet portresi (premium, koyu), teknik özellik kartı (W, devir, salınım, taban çapı), kontrol detayları (tetik, ekran, kablo), gerçek uygulama, lansman serisi.
- **Riskli noktalar:** Gövde üzerindeki logo ve model yazısı; ekran ve göstergeler (değer uydurma); kablo ve tetik geometrisi; aynı modelin farklı seri numaralı fotoğraflarını tek cihaz gibi birleştirme (RX Pro kaydı); FLEX'te kablolu/akülü karışması.
- **Higgsfield zinciri (öneri):**
  - Statik: gerçek fotoğraf → Photoshop/Figma'da ayrı katman → eklentiyle koyu stüdyo fonu → Relight kopya katmanda → yazılar tasarımda.
  - Video: ilk/son kare gerçek packshot ile Kling 4.0 veya MiniMax H3 (yavaş ışık süpürmesi, push-in) + kurguda Ken Burns detay planları. Örnek: [RX Pro planı](../.claude/skills/higgsfield-planla/references/ornek-plan.md).
  - Uygulama: gerçek çekim → video Relight → Color Palette / DaVinci LUT → Reframe 9:16.
  - 3D (ileride): 2–4 açılı fotoğraftan `multi_image_to_3d` → Blender'da logoyu gerçek dosyadan kaplama → turntable render. Makinenin geometrisi karmaşık olduğu için önce tek modelde dene.
- **Yapmayız:** AI'a makineyi döndürtmek veya elde çalıştırtmak (gövde ve logo bozulur); ekrana değer bastırmak; tanıtım için çalışırken ölçülmemiş performans iddiası.

### 4.2 Polisaj pastaları ve cilalar — Menzerna, GYEON, Fra-Ber, Innovacar hızlı cilalar

- **Göstermek istediklerimiz:** Kesim → finiş aşama sistemi ("hangi pasta hangi aşamada?"), ürün + uyumlu sünger eşleşmesi, pasta dokusunun makro görüntüsü, boya yüzeyinde parlaklık.
- **Riskli noktalar:** Şişe etiketindeki ürün numarası ve aşama bilgisi (ör. Menzerna 1100, 2200); hacim varyantları; Menzerna logo zemini kuralı; abartılı önce/sonra.
- **Higgsfield zinciri (öneri):**
  - Bilgi kartı/carousel: gerçek şişe fotoğrafları + Figma'da aşama şeması (yazı vektör). Arka plan için Recraft V4.1 `utility` veya Figma eklentisi (Expand).
  - Makro doku: ürünsüz pasta damlası ve parlak boya yüzeyi AI B-roll olarak (Seedance 2.5 / Kling); şişe kurguda gerçek packshot.
  - Uygulama Reels: gerçek çekim (pad üzerinde pasta, makine, sonuç) + Relight + LUT.
- **Yapmayız:** Gerçek olmayan çizik giderme sonucu; şişeyi AI'a ürettirip yayınlamak.

### 4.3 Süngerler, pedler, keçeler — MG PADS, Menzerna süngerleri ve keçeleri

- **Göstermek istediklerimiz:** Renk/agresiflik sistemi, çap seçenekleri, set sunumu (flatlay), makineye uyum.
- **Riskli noktalar:** **Renk = fonksiyon.** Kayıtlarda Menzerna'da sarı "İnce Pasta", kırmızı "Kalın Pasta", yeşil "Hare Giderici"; MG PADS'te sarı "Hare Giderici". Renk sistemi markadan markaya farklı; AI veya renk düzeltme sünger rengini kaydırırsa yanlış ürün anlatılır. Çap ve yükseklik ölçüleri (ör. 45/35 mm) SKU'dan gelir.
- **Higgsfield zinciri (öneri):**
  - Flatlay ve set: gerçek fotoğraflardan Photoshop kompoziti. AI yalnızca fon ve gölge için. Hazır `flatlay` / `bundle` tarifleri ürünü yeniden çizdiği için yalnızca konsept olarak.
  - Renk uyumu: Color Palette / LUT kullanılacaksa sünger renkleri öncesi-sonrası karşılaştırılır.
  - Video: pedin dönüşü gerçek çekimle; AI ile pad dönüşü üretme.
- **Yapmayız:** Bir markanın renk kodunu diğerine taşımak; AI ile ped dokusu ve rengi üretmek.

### 4.4 Seramik kaplama ve koruma — GYEON Q², MX-PRO, Innovacar SC0 ve S1

- **Göstermek istediklerimiz:** Premium kit sunumu (kutu, şişe, aplikatör), uygulama adımları, hidrofobik etki (boncuklanma), dayanım ve koşulları.
- **Riskli noktalar:** EVO/REDEFINED, 9H gibi isimdeki ifadeler ve hacim; kutu içeriği (setteki parça sayısı); boncuklanmanın ürünün gerçek sonucu gibi sunulması; "36 aya kadar" türü koşullu iddialar.
- **Higgsfield zinciri (öneri):**
  - Kit: gerçek fotoğraf (kutu açık/kapalı) → Photoshop katmanı + koyu fon (`koyu-urun`). Mockup Studio yalnızca konsept.
  - Boncuklanma: gerçek makro çekim en iyisi. AI ile su boncuğu B-roll ancak ürünsüz ve "temsili" bağlamda; ürün sonucu gibi sunulmaz.
  - Uygulama adımları carousel: Figma bilgi kartı (STIL-005/006 yaklaşımı) + gerçek ürün fotoğrafı.
  - Uzun anlatım: Explainer ile "seramik kaplama nedir" (markasız); teknik bilgiler elle kontrol.
- **Yapmayız:** Sertifika, uygulayıcı yetkisi veya dayanım süresini koşulsuz yazmak.

### 4.5 Yıkama ve temizlik kimyasalları — Fra-Ber, Innovacar, GYEON QM

- **Göstermek istediklerimiz:** Köpük ve yıkama (gün ışığı), konsantre ve dilüsyon bilgisi (ör. Fra-Ber Bersolux kaydında 1:120), profesyonel bidon/5 L/25 L ürünler (B2B), iç temizlik süreçleri, su izi ve kireç çözümleri.
- **Riskli noktalar:** Benzer şişe formları (Genjutsu ile şişe değişiminde karışma); ürün ailesi renkleri (Innovacar); hobi vs profesyonel ayrımı (Fra-Ber); kayıttaki bilinen çelişkiler (71482: başlık 5 kg, açıklama 25 kg).
- **Higgsfield zinciri (öneri):**
  - Köpük Reels: gerçek köpük çekimi + Relight + LUT. Atmosfer planları (su damlası, köpük akışı) AI B-roll.
  - Ürün değişimli seri: tek gerçek yıkama çekimi → Genjutsu Lite ile ucuz deneme → Objects swap. Yalnızca şişe formu benzer ürünlerde; etiket kare kare kontrol.
  - Dilüsyon ve kullanım kartları: Figma; değerler yalnızca SKU açıklamasından.
  - B2B statik reklam: Ads Studio ile 2–3 reklamlık deneme (marka kiti elle düzeltilmiş).
- **Yapmayız:** Innovacar'da sahte önce/sonra; hobi ve pro ürünü aynı karede.

### 4.6 Mikrofiber, havlu, eldiven, aplikatör — KLIN, GYEON Q2M

- **Göstermek istediklerimiz:** Doku (GSM), kurulama ve yıkama kullanımı, renk varyantları, paket içeriği.
- **Riskli noktalar:** Etiket genelde ambalajda, ürün üzerinde değil; bu yüzden lifestyle sahnelerde AI riski görece düşük. Ama GSM, ölçü ve paket adedi SKU'dan gelir; renk varyantları ayrı SKU'dur.
- **Higgsfield zinciri (öneri):**
  - Lifestyle: Nano Banana Pro / GPT Image 2.5 ile ürün referanslı sahne (ambalajsız havlu). Doku yakın planı gerçek fotoğraf.
  - Trend uyumlu kısa video: gerçek kurulama çekimi + Shorts Studio preseti.
- **Yapmayız:** Paket içeriğini veya renk seçeneğini uydurmak.

### 4.7 Pompa ve sprey ekipmanı — IK Sprayers, EPOCA

- **Göstermek istediklerimiz:** Kimyasal dayanım türleri (alkali, asit, solvent, gıda teması), köpük pompası performansı, conta tipi (ör. NBR), yedek parça kitleri, PPF/cam filmi pompaları.
- **Riskli noktalar:** Nozzle, manometre ve conta detayları; "CE/FDA" gibi sertifika ifadeleri yalnızca SKU kaynağında varsa; dayanım tipine göre renk ayrımları.
- **Higgsfield zinciri (öneri):**
  - "Hangi pompa hangi kimyasal için?" bilgi kartı: gerçek ürün fotoğrafları + Figma tablo.
  - Mekanizma anlatımı: Content Factory `Cutaway Lab` stili ya da Explainer, **markasız ve genel**. Gerçek iç yapı bilinmiyorsa çizilmez.
  - Köpük gösterimi: gerçek çekim (köpük kalitesi AI ile gösterilmez).
- **Yapmayız:** AI ile pompa iç yapısı veya sertifika etiketi üretmek.

### 4.8 PPF, cam filmi ve atölye ekipmanı — SGCB, IK PPF, EPOCA TINT

- **Göstermek istediklerimiz:** Usta ekipmanı (ragle, kesici, magnet, kemer, tabure, hava tabancası), atölye düzeni, profesyonel uygulama.
- **Kitle:** Ağırlıklı olarak profesyonel uygulamacı (B2B).
- **Higgsfield zinciri (öneri):** Gerçek atölye çekimi + Relight + Reframe. Ekipman seti flatlay'i Photoshop kompoziti. Usta karakteri gerekiyorsa AI Influencer yalnızca rıza ve "AI karakter" etiketiyle; ürün elde gerçek çekimle.
- **Yapmayız:** Kayıttaki SCCB/SGCB yazım çelişkisini metne taşımak (kayıt SGCB altında; orijinal yazım korunuyor).

### 4.9 Kokular — Little Joe, Fra-Ber kokuları

- **Göstermek istediklerimiz:** Çok sayıda koku varyantı, araç içi kullanım, kalıcılık (kayıtlarda "45 gün"), mevsimsel/trend içerik.
- **Riskli noktalar:** Varyant sayısı yüksek; koku adı ve renk eşleşmesi SKU'dan gelir. Küçük ambalaj yazısı.
- **Higgsfield zinciri (öneri):**
  - Tutarlı varyant serisi: tek gerçek fotoğraf şablonu (Photoshop/Figma) + her koku için yalnızca ürün katmanı değişir.
  - AI lifestyle: koku temasına göre ortam (ör. "Ananas Hindistan Cevizi" için tropik ışık) Nano Banana 2.1 ile, ürün katmanı gerçek.
  - Trend: kokular trend içeriğe en uygun aile. Effects veya Content Factory hook planları ürünsüz kullanılıp sonda gerçek ürün gösterilebilir.
- **Yapmayız:** "45 gün"ü koşulsuz garanti gibi yazmak; koku adlarını karıştırmak.

### 4.10 Kil ve yüzey hazırlık — MG PS kil ürünleri; maskeleme — Q1 Tapes, GYEON MaskingTape

- **Göstermek istediklerimiz:** Proses içerikleri (yıkama → kil → maskeleme → polisaj), ürün sırası, profesyonel hazırlık.
- **Higgsfield zinciri (öneri):** Gerçek proses çekimi + kurguda adım yazıları. "Polisaj öncesi hazırlık" carousel'i: gerçek ürün fotoğrafları + Figma. Bant ve kil aynı karede başka markalarla görünecekse her ürünün etiketi kontrol edilir.

## 5. İçerik türleri ve Higgsfield'deki yeri

| İçerik türü | Amaç | Ana yöntem | Higgsfield'in rolü | Uygun aileler |
|---|---|---|---|---|
| Ürün tanıtımı (hero) | Ürünü premium ve doğru göstermek | Gerçek fotoğraf + katmanlı tasarım | Fon, ışık, oran türevleri (eklenti, Inpaint, Relight, Expand) | Hepsi |
| Teknik bilgi / eğitim | Doğru ürünü seçtirmek, kullanım anlatmak | Figma bilgi kartları, carousel | Arka plan; markasız Explainer/Content Factory | Pasta, ped, pompa, kaplama |
| Uygulama / proses | Gerçek kullanımı göstermek | Gerçek çekim | Relight, Color Palette, LUT, Reframe, Upscale, AI B-roll | Makine, pasta, yıkama, kaplama |
| Lansman | Yeni ürün duyurusu | Seri tasarım + kısa Reels | İlk/son kare kilitli açılış planı, 3D (ileride) | Makine, kaplama |
| B2B / usta | Profesyonele hitap | Gerçek atölye çekimi, teknik kartlar | Ads Studio statik reklam, Reframe | Makine, PPF ekipmanı, bidon kimyasallar |
| Reklam (Meta) | Satış / trafik | Statik set + kısa video | Ads Studio, Ad Multiplier (yalnız CTA/hook), Marketing Studio Posters | Hepsi |
| Trend / eğlence | Erişim, etkileşim | Kısa, eğlenceli | Content Factory, Effects, Genjutsu Styles; **ürünsüz hook + gerçek ürünle kapanış** | Koku, yıkama, mikrofiber |

## 6. Trendleri kurumsal çizgide kullanmak

- **Hook ürünsüz, kapanış gerçek.** Trend efekti veya "ya … olsaydı?" ilk 1–3 saniyede dikkat çeker. Ürün ve etiket son planda gerçek görüntüyle gelir (öneri).
- **Marka kılavuzu önce gelir.** Innovacar'da sahte önce/sonra ve ürünü gölgeleyen büyük grafikler yok. Menzerna logosu efektli fotoğraf üstünde değil. Kılavuzu olan markalarda trend efektini ürünün üzerine uygulama.
- **Telif ve rıza.** Trend müziği ve referans videolar Genjutsu/Katana'da telif sorunu yaratabilir. Mümkünse kendi çekimimizi kaynak kullanın, müziği değiştirin. AI karakter ve yüz kullanımında rıza ve "AI ile üretildi" notu.
- **Distribütör hassasiyeti (öneri):** Dağıtımını yaptığımız markaların ürünleriyle stilize/komik efektli içerik yayınlamadan önce marka temsilcisinin görüşünü almak iyi olur. Bu kayıtlarda bir kural değil; kurumsal ilişki için önerimiz.

## 7. Planlayıcı bunu nasıl kullanır?

`/higgsfield-planla` bir istek aldığında bu belgeden:

1. Ürünün hangi aileye girdiğini bulur (4. bölüm) ve o ailenin risklerini plana yazar.
2. Markanın kuralını (3. bölüm) ve `higgsfield_test/brands/<marka>/` kaydını okur.
3. İçerik türünü (5. bölüm) belirler; trend isteniyorsa 6. bölüm çerçevesini uygular.
4. SKU iddialarını `brand_library.py product` veya `caption-context` ile kaynağından alır.

## 8. Açık konular

- MX-PRO'nun kendi markamız mı, dağıtımını yaptığımız bir marka mı olduğu [doğrulanacak].
- MG PS, MG PADS ve MG POLISHING profil klasörleri bu Git kopyasında yok (`brands/index.json`'da kayıtlı). Yerel bilgisayarda olup olmadıkları kontrol edilmeli.
- Kılavuzu olmayan markaların resmî renk, font ve logo kullanım kuralları.
- Hedef kitle önceliği (son kullanıcı / profesyonel / bayi) ürün ailesi bazında netleştirilmeli.
- İçerik sıklığı ve kanal dağılımı bu belgede belirlenmedi; elimizde performans verisi yok.
