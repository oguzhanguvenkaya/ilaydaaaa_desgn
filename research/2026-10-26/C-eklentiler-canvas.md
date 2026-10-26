# C — Higgsfield Eklentileri (Plugins) ve Canvas

Araştırma tarihi: 26 Ekim 2026. Kaynaklar higgsfield.ai ürün sayfaları, blog ve help-center (resmî) ile birkaç üçüncü taraf kaynaktır. Üçüncü taraf bilgisi **[3. taraf]** etiketiyle işaretlendi. Kaynakta bulunmayan bilgi **[doğrulanacak]** olarak bırakıldı. Higgsfield MCP araçları çağrılmadı, ücretli üretim yapılmadı.

> **Genel uyarı:** Higgsfield'ın kendi sayfaları birbiriyle çelişiyor. Kurulum dosya biçimi, minimum sürüm, araç sayısı ve "Unlimited" kapsamı sayfadan sayfaya değişiyor. Çelişkiler her bölümde ayrıca not edildi. Kurmadan önce indirme sayfasındaki güncel dosyayı kontrol edin.

## Ortak noktalar (tüm eklentiler)

- **Kredi:** Eklentiler web platformuyla, MCP ve CLI ile **aynı kredi bakiyesini** kullanır. Ayrı abonelik veya hesap gerekmez (help-center).
- **Unlimited:** Help-center'a göre *"Unlimited model access and free generations apply only on higgsfield.ai"*. Yani plan "Unlimited" olsa bile eklentideki her üretim kredi harcar. DaVinci blogu ve thepostflow [3. taraf] de bunu söylüyor. **Çelişki:** After Effects blogu *"Models on your plan's Unlimited list generate through the plugin without using credits"* diyor. Hangisinin geçerli olduğu **[doğrulanacak]**. İhtiyatlı varsayım, eklentide her üretimin ücretli olduğudur.
- **Varsayılan modeller:** Görselde Nano Banana 2, videoda Seedance 2.0 (help-center, DaVinci blogu).
- **İnternet:** Tüm üretim Higgsfield sunucularında yapılır. Çevrimdışı çalışmaz.
- **Ticari kullanım:** Ücretli planlarda web platformuyla aynı koşullar geçerlidir (ToS).
- **Araç başına kredi maliyeti:** Hiçbir eklenti sayfasında yazmıyor. Yalnızca Blender'da maliyet Generate butonunda önceden görünüyor. Diğerleri için **[doğrulanacak]**.
- **Veri ve eğitim:**
  - Photoshop sayfası *"processed securely on our infrastructure and aren't used for training"* diyor.
  - **[3. taraf]** thepostflow ise platform şartlarına göre Starter, Plus ve Ultra planlarda yüklenen ve üretilen içeriğin eğitimde kullanılabileceğini yazıyor. Team ve Enterprise planlarda "No training on your data" olduğunu belirtiyor.
  - Ürün ambalajı ve etiket görselleri için bu konu **[doğrulanacak]**. Kontrol edilecek yerler: ToS ve plan kartı.
- **Agent Bridge:** `https://bridge.higgsfield.ai/mcp` adresine "Higgsfield Bridge" adıyla custom connector eklenirse Claude veya ChatGPT gibi bir ajan, kurulu Blender veya Adobe eklentisini açık sahne ya da kompozisyon içinde kontrol edebilir.
  - Bu adres normal MCP adresinden (`mcp.higgsfield.ai/mcp`) farklıdır.
  - Bridge'in kurulumu ve sınırları help-center'ın "connect to AI agent" makalesinde geçmiyor. Ayrıntılar **[doğrulanacak]**.
- **Adobe Exchange / Blender Extensions / Blackmagic kaynağı:** Aramada resmî bir mağaza listesi bulunamadı. Dağıtım Higgsfield'ın kendi sitesinden yapılıyor. Figma eklentisi ise Figma Community'de yayımlanıyor.

## Photoshop eklentisi

**1. Ne yapıyor / araçlar**
- Sayfa eklentiyi *"a native UXP plugin that brings five Higgsfield AI tools"* olarak tanımlıyor. Beş araç şunlar: **Angles, Mockup Studio, Expand, Remove BG, Relight**.
- Help-center daha uzun bir liste veriyor: Generate AI Image, **Realtime AI** ("AI syncs to each brush stroke in real time"), **Mockup Studio**, **Layer Decompose** (düz görseli düzenlenebilir katmanlara ayırır), Angles, Shots (tek kareden kamera açısı storyboard'u), Character Swap, Remove Background, Face Swap, Upscale, Skin Enhancer, AI Stylist. Help-center'a göre Cinema Studio ve Marketing Studio da eklentinin içinden açılıyor.
- **Mockup Studio:** *"Places a flat design or product shot into a realistic context such as packaging, devices, cards, or scenes."*
- **Angles çelişkisi:** Özellik bölümü Angles'ı oranlara kırpma (9:16, 16:9, 4:3, 3:4, 21:9, 1:1) olarak, *"smart subject tracking"* ile birlikte tanımlıyor. FAQ ise "changing camera angles" diyor.
- **Expand ve Relight:** Photoshop sayfasında açıklaması yok. Figma sayfasında Expand *"extends the canvas and fills the new area"*, Relight ise ışık yönünü ve tonunu değiştiren araç olarak tanımlı.
- Hangi araçların gerçekten panelde olduğu **[doğrulanacak]** (5 araç mı, 12 araç mı).

**2. Kurulum**
- **Gereksinim:** Photoshop 2024 veya üstü. Eski sürümler *"don't support UXP plugins"*. macOS (Apple Silicon ve Intel) ile Windows destekleniyor.
- **Adımlar (ürün sayfası):**
  1. macOS veya Windows için indir. Sayfaya göre .ccx dosyası her iki mimaride çalışıyor.
  2. .ccx dosyasını "ZXP installer" penceresine sürükle.
  3. Photoshop'ta **Window → Extensions → Higgsfield** yolunu aç.
- **Çelişki:** FAQ ".uxp installer + Applications'a sürükle" diyor. Help-center ".UXP installer, helper app gerekmez" diyor. Doğru dosya biçimi **[doğrulanacak]**.
- **Giriş:** Panel içinden Higgsfield hesabıyla yapılıyor. *"Free credits are included with every account"*.

**3. Kullanım**
1. Paneli aç ve giriş yap.
2. Aracı seç (ör. Mockup Studio).
3. Kanvastaki görseli girdi olarak kullan.
4. Üret.

- Çıktı: *"stream directly back into Photoshop as new layers"*. Her sonuç maskelenebilir ve blend edilebilir **yeni bir katman** olarak gelir. *"Smart objects and adjustment layers are fully respected."*
- Layer Decompose düz görseli düzenlenebilir katmanlara ayırır.
- Araç içi adım adım ayarlar (prompt alanı, seçim/maske girdisi var mı vb.) **[doğrulanacak]**.

**4. Sınırlar**
- İnternet gerekli. Photoshop 2024 altı desteklenmiyor.
- Kabul edilen dosya tipi, çözünürlük, boyut sınırı ve araç başına kredi belirtilmemiş **[doğrulanacak]**.
- Tam olarak bizim kullanım senaryomuz olan "seçili katmanı koru, yalnızca arka planı üret" modu olup olmadığı yazmıyor **[doğrulanacak]**.

**5. Öneri (iş akışı)**
- **Öneri:** Gerçek ürün fotoğrafını (etiket ve logo net) ayrı bir katmanda kilitli tutun. Gerekirse Remove BG ile kesin, ama tercihen Photoshop'un kendi seçim araçlarıyla kesip maskeyi siz kontrol edin. Arka plan veya sahne için Generate AI Image ya da Mockup Studio'yu **ayrı bir katmanda** çalıştırın. Sonuçlar yeni katman olarak geldiği için orijinal ürün pikselleri değişmeden kalır.
- **Öneri:** Relight ve Expand doğrudan ürün katmanına uygulanırsa etiket ve yazı bozulabilir. Bu riskli. Önce kopya katmanda deneyin, sonra etiket bölgesini orijinal katmandan maskeyle geri getirin.
- **Öneri:** Angles ile tek bir master görselden 1:1, 4:5 ve 9:16 türevleri çıkarılabilir. 4:5 listede yok, bu yüzden 3:4 veya manuel kırpma gerekir.

**6. Kaynaklar**
- https://higgsfield.ai/plugins/photoshop
- https://higgsfield.ai/photoshop-plugin
- https://higgsfield.ai/creator-hub/help-center/integrations/external-integrations-higgsfield

## Premiere Pro ve After Effects eklentisi (tek kurulum)

**1. Ne yapıyor / araçlar**
- Tek installer ve tek panel. Ürün sayfası "Five pro AI plugins" diyor. AE blogu ise 7 araç sayıyor:
  - **Generate AI Video** (prompt'tan klip, *"drops straight into the timeline"*)
  - **Generate AI Image** (arka plan, overlay, title card)
  - **Reframe** (9:16, 16:9, 4:3, 3:4, 21:9, 1:1 ve subject tracking)
  - **Remove Background** (yeşil perde olmadan key, *"pure alpha channel"*)
  - **Draw to Edit** (kare üzerine çizerek nesne silme, ekleme veya değiştirme, inpainting)
  - **Upscale** (*"up to 4K or 8K"*)
  - **Edit Video** (doğal dille prompt tabanlı düzenleme)
- AI LUT creator Adobe tarafında listelenmiyor. Thepostflow [3. taraf] da bunu teyit ediyor.

**2. Kurulum**
- **Sürüm çelişkisi:** Ürün sayfaları "Premiere Pro / After Effects **2025 (25.0)** veya üstü" diyor. Help-center ve AE blogu "**2024 (24.0)** ve üstü" diyor. Hangisi geçerli **[doğrulanacak]**. Güvenli varsayım 2025.
- **macOS:**
  1. .dmg dosyasını indir.
  2. Higgsfield'ı Applications'a sürükle ve installer'ı çalıştır. Adobe uygulamaları otomatik algılanıyor.
  3. Uygulamada **Window → Extensions → Higgsfield** yolunu aç.
  - Universal binary (M1–M4 ve Intel).
- **Windows (10/11, 64-bit):**
  - Help-center ve AE bloguna göre: aescripts'ten ücretsiz **ZXP Installer**'ı kur, ardından Higgsfield .zxp dosyasını onun penceresine sürükle.
  - Ürün sayfasında ".msi, helper app yok" ifadesi de geçiyor. Hangisi güncel **[doğrulanacak]**.
- **Kurulum ipuçları:**
  - Kurulum sırasında Adobe uygulamaları tamamen kapalı olmalı.
  - Panel görünmezse installer'ı yönetici olarak çalıştırın (Win) veya Privacy & Security'den izin verin (Mac).
- **Giriş:** Panel içinden yapılıyor. FAQ'ta "subscription gerekli mi?" sorusuna "Yes" yanıtı var, ama aynı sayfa "starter credits ile ücretsiz deneyin" de diyor. Bu belirsizlik **[doğrulanacak]**.

**3. Kullanım**
- Panel, aracı seç, ayarla, çalıştır. Sonuç *"sent back into your Adobe timeline"*.
- AE'de görseller *"directly in your project, ready to drop onto a layer"*. Video doğrudan kompozisyona veya timeline'a geliyor.
- Kesin konum (Project panel bin'i mi, yeni track mi) belirtilmemiş **[doğrulanacak]**.
- Adım adım araç ekranları sayfalarda yok **[doğrulanacak]**.
- **Ajan kontrolü (AE):** Bridge MCP veya Supercomputer, kurulu eklentiyi algılayıp efekt, animasyon ve expression üretebiliyor ve üretimleri kompozisyona aktarabiliyor (AE blogu).
- **İpucu (AE blogu):** Tüm video modellerine erişim için web'de üretip panel üzerinden içeri alınabiliyor. Bu, eklentide model seçeneklerinin kısıtlı olabileceğini düşündürüyor **[doğrulanacak]**.

**4. Sınırlar**
- İnternet gerekli. Eski sürümler desteklenmiyor.
- Klip süresi, girdi formatı, eşzamanlı iş sayısı ve kredi maliyeti belirtilmemiş **[doğrulanacak]**.
- DaVinci blogunda üretim klipleri için 4–15 sn sınırı geçiyor. Bu muhtemelen model sınırı ve Adobe için de geçerli olabilir **[doğrulanacak]**.

**5. Öneri (iş akışı)**
- **Öneri (Premiere, Reels kurgusu):**
  - Gerçek ürün çekimlerini (etiket okunur close-up'lar) ana timeline'da tutun.
  - Generate AI Video'yu yalnızca **B-roll ve atmosfer** için kullanın: köpüklü yıkama, su damlaları, parlayan boya yüzeyi, garaj ortamı.
  - Ürün ve etiket çekimleri gerçek kalsın.
- **Öneri:** Yatay çekilmiş eski ürün videolarını **Reframe 9:16** ile Reels'e çevirin. Subject tracking'in şişeyi merkezde tuttuğunu her klipte gözle kontrol edin.
- **Öneri (AE):**
  - Gerçek ürün fotoğrafını **Remove Background** ile değil, mümkünse kendi maskenizle alfa kanallı katman yapın.
  - Arka plan için Generate AI Image ile sahne üretin. Ürün katmanını üstte ayrı tutup 3D kamera veya parallax ile "reklam videosu" hareketi verin.
  - Etiket piksel düzeyinde korunur, çünkü AI ürün katmanına dokunmaz.
- **Öneri:** Edit Video ve Draw to Edit'i ürün etiketinin göründüğü karelere uygulamayın. Yeniden üretim yazıyı bozabilir.

**6. Kaynaklar**
- https://higgsfield.ai/plugins/premiere-pro
- https://higgsfield.ai/plugins/after-effects
- https://higgsfield.ai/blog/higgsfield-after-effects
- https://higgsfield.ai/creator-hub/help-center/integrations/external-integrations-higgsfield
- [3. taraf] https://thepostflow.com/?p=9453

## DaVinci Resolve eklentisi

**1. Ne yapıyor / araçlar**
- Tek panelde 7 çekirdek araç: Generate Video, Generate Image, Edit Video, Draw to Edit, Reframe, Remove Background, Upscale (4K/8K).
- Bunlara ek olarak **AI LUT Creator** var. Referans kare, fotoğraf veya paletten renk eşler. Çıktıyı **.cube LUT** olarak dışa aktarır ya da color node uygular. Thepostflow'a [3. taraf] göre LUT klibe gömülmüyor, Color sayfasına gönderiliyor.
- Yardımcı araçlar: **Last Generations** ve **Import to Resolve**.
- Cinema Studio ve Marketing Studio da panelden açılıyor (DaVinci blogu).
- Help-center aynı özellikleri "Draw to Video" ve "Color Match" adlarıyla anıyor.

**2. Kurulum**
- **Gereksinim:** DaVinci Resolve **19+**, macOS veya Windows. **App Store sürümü desteklenmiyor.** Blackmagic sitesinden indirilen sürüm gerekli.
- **Studio ve ücretsiz sürüm:** Resmî sayfada belirtilmiyor. Thepostflow [3. taraf] ücretsiz sürümün de uygun olduğunu *yorumluyor*. **[doğrulanacak]**
- **Adımlar:**
  1. higgsfield.ai/plugins/davinci adresinden installer'ı indir. Sayfalar Mac için .pkg ya da .dmg, Windows için .exe diyor (kaynaklar tutarsız).
  2. Installer'ı çalıştır. Resolve otomatik algılanıyor.
  3. Resolve'da **Workspace → Workflow Integrations → Higgsfield** yolunu aç. Bazı kurulumlarda yol **Workspace → Scripts**. Panel istenen yere dock edilebiliyor.
- Help-center farklı bir yöntem anlatıyor: "plugins klasörüne yerleştir".
- Thepostflow [3. taraf] eklenti sürümünü 7 Haziran 2026 tarihli olarak veriyor.

**3. Kullanım**
- Aktif klibi veya önizlemeyi kullan, varsa referans ekle, çekimi tarif et.
- Sonuç **Import to Resolve** ile **Media Pool'a veya Timeline'a** gelir. FAQ'a göre *"sent back into your Resolve media pool automatically"*.
- Beğenilmeyen klip aynı panelden yeniden üretilebilir.
- Renk uyumsuzluğu AI LUT Creator ile giderilir.

**4. Sınırlar**
- İnternet gerekli. Resolve 19 altı ve App Store sürümü desteklenmiyor.
- Video klipleri **4–15 saniye** (DaVinci blogu). Uzun master çekim için uygun değil.
- Kare hızı, codec ve gamma etiketi yayımlanmıyor. Thepostflow [3. taraf] bunun timeline'da uyumsuzluk yaratabileceğini söylüyor.
- Upscale tavanının hesaba bağlı olabileceği belirtiliyor [3. taraf].
- Araç başına kredi maliyeti belirtilmemiş **[doğrulanacak]**.

**5. Öneri (iş akışı)**
- **Öneri:** Reels kurgusu DaVinci'de yapılıyorsa ürün çekimleri gerçek kalsın. Kısa (4–15 sn) AI B-roll'leri Media Pool'a alıp araya kesin.
- **Öneri:** **AI LUT Creator** ile marka "look"unu bir referans kareden .cube LUT olarak çıkarın. Sonra bunu tüm Reels'lere uygulayın. Bu, ürün piksellerini yeniden üretmeden yalnızca renk düzeltmesi yapar, bu yüzden etiket doğruluğu açısından güvenli bir AI kullanımıdır. Yine de logo ve marka renklerinin LUT sonrası sapmadığını kontrol edin.
- **Öneri:** Proje kare hızını sabitleyin (ör. 30 fps). AI kliplerinin fps ve renk uzayını import sonrası kontrol edin.

**6. Kaynaklar**
- https://higgsfield.ai/plugins/davinci (not: /plugins/davinci-resolve 404 veriyor)
- https://higgsfield.ai/blog/higgsfield-davinci-resolve
- https://higgsfield.ai/creator-hub/help-center/integrations/external-integrations-higgsfield
- [3. taraf] https://thepostflow.com/?p=9453

## Figma (ve FigJam) eklentisi

**1. Ne yapıyor / araçlar**
- **Ürün sayfası:** Image generation, Video generation, Remove Background, Color Grading (seçili görsele renk profili), Relight (ışık yönü ve tonu), Expand (kanvası genişletip doldurur), Angles (aynı konunun yeni kamera açıları).
- **Help-center ek olarak şunları listeliyor:** **Vector Generation (SVG)**, **Mockup Studio**, **Face Swap**, animasyon.
- **FigJam'e özel:** **Canvas Nodes**, otomatik pipeline ve chain workflow (Canvas'ın FigJam versiyonu). Help-center: *"Canvas Nodes are a FigJam-only feature"*.
- **Mockup Studio:** Ürün sayfasında açıklanmıyor. Panel kartında ve help-center'da adı geçiyor. Figma'daki davranışı (ambalaj veya cihaz mockup'ı) Photoshop'taki tanıma benzer olmalı ama **[doğrulanacak]**.
- **Araç sayısı çelişkisi:** Sayfa bir yerde "six tools", FAQ'ta ise "image, video + five apps" diyor.

**2. Kurulum**
- Figma veya FigJam'de **Plugins → Find more plugins → "Higgsfield AI"** (yayıncı Higgsfield Inc.) ara, ya da Community sayfasından "Add to Figma" de.
- Masaüstü (macOS/Windows) ve tarayıcıda çalışıyor. Ayrı installer yok.
- Community linki: https://www.figma.com/community/plugin/1641150071720162509/higgsfield-ai-remove-background-mockup-face-swap-ai-image-video-generator (sayfa 403 verdi, içeriği okunamadı).
- **Giriş:** İlk çalıştırmada web hesabıyla yapılıyor. Kredi web ile ortak.

**3. Kullanım**
1. Plugins menüsünden eklentiyi aç ve giriş yap.
2. Frame'i veya görseli seç.
3. Aracı seç, prompt yaz ya da düzenlemeyi uygula.
4. Sonuç kanvasa gelir.

- Sonuç *"on your selected frame when possible"* yerleşiyor. Taşınabilir, maskelenebilir standart **image/video katmanı** olarak geliyor. Help-center'a göre Insert, sürükle-bırak veya auto-insert ile ekleniyor.
- **Sayfanın ipucu:** Relight, Color Grading ve Expand için temiz kaynak görselle başlayın. Prompt'ta konu, stil ve atmosferi açıkça yazın.

**4. Sınırlar**
- Çözünürlük, dosya boyutu, kota ve kredi maliyeti belirtilmemiş **[doğrulanacak]**.
- Canvas Nodes yalnızca FigJam'de.
- İnternet gerekli.

**5. Öneri (iş akışı)**
- **Öneri:** Instagram post şablonlarını (marka renkleri, fiyat ve kampanya yazısı, logo) Figma'da tutun. Gerçek ürün PNG'sini sabit katman olarak koyun. Yalnızca arka plan alanını eklentiyle üretin (Image generation veya Expand). Metin ve logo Figma vektörü olarak kaldığı için AI yazı bozulması olmaz.
- **Öneri:** Tek master tasarımdan 1:1 ve 9:16 türevlerine geçerken Expand ile arka planı genişletin. Ürün katmanı yerinde kalır.
- **Öneri:** Mockup Studio'yu ambalaj veya etiket mockup'ı için yalnızca *konsept* aşamasında kullanın. Yayın görselinde gerçek etiket fotoğrafı esas alınsın.

**6. Kaynaklar**
- https://higgsfield.ai/plugins/figma
- https://higgsfield.ai/creator-hub/help-center/integrations/external-integrations-higgsfield
- https://higgsfield.ai/creator-hub/help-center/tools-and-workflows/how-do-i-use-canvas

## Blender eklentisi (add-on)

**1. Ne yapıyor / araçlar**
- 3D viewport üzerinde **yüzen bir prompt çubuğu** var (ayrı pencere veya sidebar değil). Çubukta 7 sekme bulunuyor:
  - **Scene Builder:** Tarif edilen seti obje, yerleşim ve ışıkla birlikte açık .blend içinde düzenlenebilir geometri olarak kurar.
  - **3D Model:** Prompt veya **fotoğraftan** mesh üretir. Mesh 3D cursor'a gelir. Tanıtım ifadesi *"Clean topology", "Materials included"*.
  - **Character Animation:** Rig ve timeline'da keyframe'ler üretir. Standart Blender bone ve action'ları kullanır.
  - **Image:** Görseli plane olarak ekler ya da bir materyale bağlar.
  - **Video:** Scene Builder blockout'larından bitmiş çekim üretebilir.
  - **Camera:** Açıklaması yok **[doğrulanacak]**.
  - **Asset:** Üretim kütüphanesi (3D, Images, Video filtreleri ve diske giden klasör kısayolu).
- **Modeller:** Görselde Nano Banana 2, GPT Image, Seedream 5.0 Pro, Z Image. Videoda Seedance 2.5. 3D'de **Meshy 5**. Ayrıca upscaler'lar.

**2. Kurulum**
- **Blender 5.1+**, Windows veya macOS (help-center). Linux belirtilmemiş **[doğrulanacak]**.
- **Adımlar:**
  1. .zip dosyasını indir, **zipten çıkarma**.
  2. Açık bir Blender penceresine sürükle. Alternatif yol **Edit ▸ Preferences ▸ Add-ons ▸ Install**.
  3. Çubuk viewport üzerinde belirir. Giriş yap.
- Üretim bulutta yapıldığı için güçlü GPU gerekmiyor. Kendi Cycles/EEVEE render'larınız için GPU yine önemli.
- **Kredi:** Web ile aynı kredi kullanılıyor, ayrı abonelik yok. Kişisel ve takım workspace'leri destekleniyor.
- **Maliyet ön izlemesi:** **Generate butonundaki sayı, krediyi basmadan önce gösterir.** Varyant sayacı bu maliyeti çarpar. Bakiye çubukta görünür.

**3. Kullanım**
1. Sekmeyi seç.
2. Modeli, çözünürlüğü ve fps'i seç.
3. Prompt yaz veya referans görsel bırak.
4. Generate butonundaki fiyatı kontrol et ve üret.

- Sonuçlar Asset sekmesinde toplanır ve tek tıkla sahneye eklenir.
- Üretilen içerik .blend dosyasında ve diskte kalır, sonrasında çevrimdışı kullanılabilir.
- **Bridge:** `bridge.higgsfield.ai/mcp` ile bir ajan açık sahnede çalışabilir.

**4. Sınırlar**
- İnternet ve giriş gerekli.
- Mesh doğruluğu, poligon sayısı ve doku çözünürlüğü belirtilmemiş **[doğrulanacak]**.
- **Not:** Blender sayfasının yapılandırılmış verisi (JSON-LD) ve FAQ'ının bir kısmı yanlışlıkla Adobe eklentisine ait.

**5. Öneri (iş akışı)**
- **Öneri:** 3D Model sekmesi fotoğraftan ürün mesh'i çıkarabiliyor. Ancak AI mesh'te etiket dokusunun ve logonun birebir doğru olacağı **garanti değil**. Bu yüzden şöyle ilerleyin:
  1. Şişe veya kutu gövdesini AI ile ya da manuel olarak modelleyin.
  2. **Gerçek etiket görselini (vektör veya baskı dosyası) UV ile kendiniz kaplayın.**
  3. Scene Builder'ı yalnızca ortam için kullanın (garaj, detailing stüdyosu, araç kaputu).
- **Öneri:** Tamamlanan sahneden Blender kamerasıyla 9:16 turntable veya ürün reveal render'ı alın. Bu, etiketin piksel düzeyinde doğru kaldığı tek "AI destekli 3D reklam" yoludur. Video sekmesiyle AI'a render ettirmek etiketi yeniden üretebilir, bu riskli.
- **Öneri:** Çok markalı katalog için bir kez kurulan bir "stüdyo sahnesi"ne farklı ürün modelleri değiştirilerek yerleştirilebilir.

**6. Kaynaklar**
- https://higgsfield.ai/plugins/blender
- https://higgsfield.ai/creator-hub/help-center/integrations/external-integrations-higgsfield

## Canvas (node tabanlı iş akışı)

**1. Ne yapıyor**
- Help-center tanımı: *"node-based infinite board for multi-model visual production"*. Modelleri zincirleme, paralel çalıştırma, çıktıları yan yana karşılaştırma, akışı **şablon** olarak kaydetme ve gerçek zamanlı takım çalışması sağlıyor.
- "Visual ideation meets repeatable AI workflows" ifadesi **[3. taraf]** bir yazıdan (i-scoop) geliyor.
- **Node tipleri:**
  - Help-center: Text Prompt, Generation (her Higgsfield modeli), Reference (görsel veya ses yükleme ya da Assets'ten mevcut üretim), Audio (video node'una ses referansı, voiceover veya sync).
  - canvas-intro sayfası ek olarak şunları gösteriyor: image ve video node'ları, style reference, start/end frame, **product ve logo node'ları**, renk paleti, sketch girdileri.
  - Soul ID karakterleri, **yüklenen ürünler**, marka referansları ve geçmiş üretimler node olarak eklenebiliyor.
- **Modeller (örnek):** Kling 3.0, Seedance 2.0, Wan 2.7, Soul 2.0, GPT Image 2.0, Veo 3.1, Nano Banana Pro. FAQ'a göre her Higgsfield modeli graph içinde çalışıyor.
- **Diğer özellikler:** Node'a bağlı yorumlar, versiyon kaydı, otomatik kayıt (autosave).

**2. Kurulum / erişim**
- Kurulum yok, web üzerinden çalışıyor: higgsfield.ai → **Canvas → New canvas**. Giriş gerekli.
- Şablonlar ve "Quick Start" bağlantıları var.
- **Kredi:**
  - Graph kurmak, bağlamak ve prompt düzenlemek ücretsiz. Kredi yalnızca node **ürettiğinde** düşüyor, model web'deki fiyatıyla ücretlendiriliyor.
  - **Unlimited plan erişimi Canvas'ta geçerli değil.** Her Canvas üretimi plandan bağımsız olarak kredi harcıyor (help-center).

**3. Kullanım**
1. Text Prompt node'u ekle.
2. Generation node'u ekle, prompt'u bağla ve modeli seç.
3. Bir node'un çıktısını sonrakinin girdisine sürükleyerek zincirle.
4. Reference node'ları ekle.
5. Her node'da Generate'e bas (tek tek ya da sırayla).
6. Akışı **şablon** olarak kaydet.

- **Seedance node'ları:** Referansın rolü (character, location, **product**) prompt'un başında yazılmalı. Görsel bağlantı tek başına yeterli değil.
- **Kling node'ları:** Bağlı görsel **başlangıç karesi** olarak kullanılıyor. Karakter veya eleman referansı için önce platformda element oluşturup prompt'ta @element-name ile çağırın.
- **Paylaşım:** Canvas ayarlarından Share ile ekip davet edilir, ekip aynı anda düzenleyebilir.

**4. Sınırlar**
- Node sayısı, dosya boyutu, takım boyutu ve plan sınırı belirtilmemiş **[doğrulanacak]**.
- Unlimited geçerli değil.
- Sorun giderme: hard refresh ya da gizli pencere. Kayıp işte destek için generation ID gerekiyor.
- **[3. taraf]** Dreamina incelemesine göre node arayüzü öğrenme gerektiriyor ve büyük graph'lar karmaşıklaşıyor.

**5. Öneri (iş akışı)**
- **Öneri:** Distribütör için **tekrar kullanılabilir bir "ürün kampanya şablonu"** kurun:
  - [Ürün referans node'u (gerçek fotoğraf)] + [Logo node'u] + [Marka renk paleti node'u] → Görsel model (ör. Nano Banana Pro veya GPT Image) → ortam varyantları (garaj, yağmur sonrası araç, stüdyo).
  - En iyi kare → Kling node'una **başlangıç karesi** olarak bağlanır → Reels klibi üretilir.
  - Yeni ürün geldiğinde yalnızca ürün node'u değiştirilir.
- **Öneri:** Seedance node'larında prompt'u "PRODUCT: [görsel] is the exact product; keep label and logo unchanged…" gibi rol bildirimiyle başlatın (help-center'ın rol bildirme tavsiyesi).
- **Öneri:** Aynı prompt'u 2–3 modelde paralel çalıştırıp **etiket doğruluğunu yan yana karşılaştırın**. En sadık modeli şablona sabitleyin.
- **Öneri:** Canvas çıktıları da AI ile yeniden çizilmiş ürün içerir. Kritik yayın görselinde ürünü yine Photoshop veya Figma'da gerçek fotoğraf katmanıyla değiştirin ya da üstüne bindirin.
- **Öneri:** Figma kullanılıyorsa FigJam'deki **Canvas Nodes** ile ekip beyin fırtınası ve moodboard aşaması FigJam'de yapılabilir.

**6. Kaynaklar**
- https://higgsfield.ai/canvas
- https://higgsfield.ai/canvas-intro
- https://higgsfield.ai/creator-hub/help-center/tools-and-workflows/how-do-i-use-canvas
- [3. taraf] https://www.i-scoop.eu/higgsfield-enables-new-workflows-for-ai-video-creation/
- [3. taraf] https://dreamina.capcut.com/ai-video/higgsfield-canvas

## Hangi araç hangi iş için? (özet öneri tablosu)

| İhtiyaç | Önerilen araç | Etiket güvenliği |
|---|---|---|
| Ürün fotoğrafı + AI arka plan (post) | Photoshop veya Figma eklentisi (yeni katman) | Yüksek (ürün katmanı korunur) |
| Post şablonu, metin ve logo | Figma eklentisi | Yüksek (metin vektör kalır) |
| Reels kurgusu + AI B-roll | Premiere veya DaVinci eklentisi | Yüksek (B-roll'de ürün yoksa) |
| Marka renk look'u | DaVinci AI LUT Creator | Yüksek (yalnızca renk) |
| Yatay → 9:16 | Reframe (Premiere/AE/DaVinci) | Orta (takip kontrolü gerekli) |
| Ürün odaklı reklam videosu (kompozit) | After Effects (ürün katmanı + AI sahne) | Yüksek |
| 3D ürün sahnesi, turntable | Blender (gerçek etiket UV doku + AI ortam) | Yüksek (etiketi elle kaplarsanız) |
| Tekrarlanabilir kampanya üretimi | Canvas şablonu | Orta (AI ürünü yeniden çizer, son kontrol şart) |

Tablodaki tüm satırlar **öneridir**.

## Bulunamayanlar / doğrulanacaklar

- Araç başına kredi maliyetleri (Blender hariç; orada fiyat butonda görünüyor).
- Unlimited planın eklentilerde geçerli olup olmadığı. Help-center "hayır", AE blogu "evet" diyor.
- Adobe minimum sürümü: 2024 (24.0) mı, 2025 (25.0) mı.
- Photoshop installer biçimi (.ccx/ZXP mi .uxp mi) ve Windows Adobe installer biçimi (.msi mi .zxp mi).
- Photoshop panelindeki gerçek araç seti (5 mi, 12 mi).
- Photoshop'ta seçili ürün katmanını koruyarak yalnızca arka plan üreten bir mod olup olmadığı.
- Adobe'de çıktının tam konumu (Project bin mi, yeni track mi).
- DaVinci'nin ücretsiz sürümle uyumu (yalnızca [3. taraf] yorum var). DaVinci menü yolu ve dosya biçimindeki tutarsızlıklar.
- Blender Camera sekmesinin işlevi. Linux desteği.
- Figma'da Mockup Studio'nun ayrıntılı davranışı. Figma Community sayfası 403 verdi.
- Eklentilerde kullanılabilen model listesi (Blender hariç).
- Dosya, çözünürlük ve süre sınırları (yalnızca DaVinci blogunda 4–15 sn video bilgisi var).
- Yüklenen ürün görsellerinin eğitimde kullanılıp kullanılmadığı. Photoshop sayfası "hayır" diyor. [3. taraf] kaynağa göre Team/Enterprise dışındaki planlarda kullanılabiliyor.
- Adobe Exchange, Blender Extensions platformu veya Blackmagic tarafında resmî listeleme bulunamadı.
