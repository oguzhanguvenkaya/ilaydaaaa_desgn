# Higgsfield Araştırması — A Ajanı: Otomasyon / Ajan / Yeni Araçlar

Araştırma tarihi: 26 Ekim 2026. Kaynaklar: higgsfield.ai blog (Creator Hub), help-center, changelog ve ürün sayfaları. Ürün sayfalarının bir kısmı (ör. /katana, /playable, /ai-influencer-studio) JavaScript ile yüklendiği için yalnızca meta veri alınabildi; bu yüzden ayrıntılar çoğunlukla blog ve help-center yazılarından geldi.

İşaretler:
- **[resmî]**: higgsfield.ai alan adındaki sayfa
- **[üçüncü taraf]**: Higgsfield dışı blog veya haber
- **[doğrulanacak]**: kaynakta bulunamadı ya da kaynaklar çelişiyor
- **ÖNERİ**: bizim iş akışımız için yorum (kaynak bilgisi değil)

Genel kredi kuralı **[resmî]**: Web'deki "Unlimited" erişim ve ücretsiz üretimler **yalnızca higgsfield.ai web arayüzünde** geçerli. MCP, CLI, ChatGPT eklentisi, Supercomputer ve API üzerinden yapılan her üretim standart ücretle kredi düşer. Tek istisna, Temmuz 2026'daki 24 saatlik "Unlimited MCP" denemesiydi (yeni kullanıcılar için, 31 Temmuz'a kadar). Kaynaklar: help-center "What is Higgsfield MCP", blog/unlimited-mcp.

---

## Content Factory (menüde "New")

**1. Ne yapıyor [resmî]**
Bir "What if…" (ya … olsaydı) sorusunu "faceless" (kamerada sunucu olmayan) kısa bir videoya dönüştürüyor. Senaryoyu sahne sahne yazıyor, karakterleri kendisi seçiyor, görselleri ve seslendirmeyi üretiyor, ardından kurguyu yapıyor. Reels, TikTok ve Shorts formatına ve aynı konudaki çok bölümlü serilere yönelik.
- Giriş: https://higgsfield.ai/content-factory (higgsfield.ai üst menüsü → Content Factory)
- Claude (MCP): `/content-factory <soru>`
- Supercomputer: aynı preset kütüphanesini kullanan bir skill olarak
- Çıkış tarihi: changelog'da 21 Ekim 2026, blogda 22 Ekim 2026

**2. Nasıl kullanılır [resmî]**
1. Üst menüden Content Factory'yi açın.
2. Kütüphaneden bir preset seçin ("50+" hazır format var; sayfada yaklaşık 56 "trending style" referans videosu listeleniyor). İsterseniz tekrarlamak istediğiniz formatların linklerinden kendi preset'inizi kurabilirsiniz.
3. "What if…" alanına konuyu yazın ve hikâyenin yönünü ve tonunu (komedi, korku, açıklayıcı vb.) tarif edin.
4. İsteğe bağlı olarak bir TikTok veya Instagram video linki ekleyin. Bu link **yalnızca format ve tempo** için kullanılıyor; aracın referansın metnini, hikâyesini ya da karakterlerini yeniden kullanmayacak şekilde tasarlandığı belirtiliyor.
5. Bölüm sayısını seçin (1–4).
6. Generate'e basın. Yayınlamadan önce hikâye akışını, anlatımı ve sonu gözden geçirin.

Ayarlar ve çıktılar:
- Süre: 15 saniye – 5 dakika. Üçüncü taraf bir kaynak 5 saniyelik adımlarla ayarlandığını yazıyor. Sayfadaki varsayılan değer 30 saniye.
- Bölüm: 1–4.
- En-boy oranı: Claude akışında dikey 9:16 (FAQ'ye göre). Web için [doğrulanacak].
- Ses: seslendirme otomatik üretiliyor; ses seçimi tarif edilmiyor. Dil: Claude'da istemin dili ya da belirttiğiniz dil kullanılıyor. İngilizce/Rusça dışındaki seslerde "aksan olabilir". **Türkçe seslendirme kalitesi [doğrulanacak].**
- Claude ve Supercomputer'da her sahnenin ayrı senaryosu ve ayrı sesi var, bu yüzden tek bir ses satırı tek başına yeniden üretilebiliyor.
- Üretim genellikle "birkaç dakika" sürüyor.

**3. Kredi [resmî, blog; Plus planı $49/1.000 kredi baz alınarak]**

| Süre | 1 bölüm | 4 bölüm |
|---|---|---|
| 15 sn | 15,75 kredi (~$0,79) | 63 kredi |
| 1 dk | 63 kredi (~$3,15) | 252 kredi |
| 5 dk | 315 kredi (~$15,75) | 1.260 kredi (~$63) |

**4. Sınırlar [resmî]**
- Ürün, logo veya marka girdisi **tanımlanmamış**. Karakterleri araç kendisi seçiyor.
- Anlatımdaki tıbbi, bilimsel ve tarihî iddialar yayından önce kontrol edilmeli.
- [üçüncü taraf, tryclout.ai] Referans linki, başkasının görüntüsünü, sesini veya müziğini kullanma izni vermez. Zamanlanmış yayın özelliği teyit edilmemiş.

**5. ÖNERİ (iş akışımız için)**
- Ürün doğruluğu kontrol edilemediği için Content Factory'yi **ürün tanıtımı için değil**, eğitici ve eğlenceli "faceless" içerik için kullanın. Örnekler: "Ya arabanı hiç yıkamasaydın?", "Ya seramik kaplama olmasaydı?", "Kil (clay bar) boyada ne yapar?"
- Ürün görüntüsünü videoya üretim içinde eklemeyin. Ürünü gösteren sahneyi Marketing Studio veya gerçek ürün çekimiyle ayrıca hazırlayın ve kurguda ekleyin. Böylece etiket ve logo bozulma riski sıfırlanır.
- Türkçe seslendirmeyi önce kısa (15 sn) bir testle deneyin; aksan sorunu varsa sesi ayrıca üretin.
- Teknik iddiaları (sertlik, dayanım süresi vb.) üretici veri sayfasıyla karşılaştırın.

**6. Kaynaklar**
- [resmî] https://higgsfield.ai/blog/higgsfield-introduces-content-factory
- [resmî] https://higgsfield.ai/content-factory
- [resmî] https://higgsfield.ai/creator-hub/changelog
- [üçüncü taraf] https://www.tryclout.ai/blog/higgsfield-content-factory-guide , https://creatorstoolbox.com/blog/higgsfield-content-factory

---

## Playable (menüde "New") — Playable Ads + Playable Games

Not: Menüdeki "Playable", Higgsfield Games'in kendisi değil. Bu, 25 Ekim 2026'da duyurulan **Playable Ads ve Playable Games** ürünü. Ayrıca Supercomputer içinde **Higgsfield Games / Games 2.0** var (aşağıda anlatılıyor).

**1. Ne yapıyor [resmî]**
- **Playable Ads**: izleyicinin oynayabildiği etkileşimli reklamlar (playable ad) üretiyor. **Yalnızca Enterprise planda.**
- **Playable Games**: oynanabilir mobil oyunlar üretiyor. Tüm planlarda var.
- Giriş: https://higgsfield.ai/playable ("Try Playable")

**2. Nasıl kullanılır [resmî]**

Playable Ads:
- Girdiler:
  - Oyun açıklaması (konsept, oyuncu eylemi, mekanik)
  - Tür: Shooter, Runner, Adventure, Action, Strategy, Maze, Puzzle, Simulation
  - Boyut: 2D, 3D veya 3D Fast
  - Mod: Manual (her aşama onaylanır) veya Auto
- İsteğe bağlı yüklemeler:
  - En fazla 40 görsel (sprite, doku vb.)
  - 1 video, 3–60 saniye, MP4/MOV/WebM
  - En fazla 20 ses dosyası
  - En fazla 3 HTML veya ZIP (mevcut oyun ya da playable)
- Çıktı: ağa uygun tek bir `.html` dosyası, en fazla 5 MB. Dışa aktarmadan önce Destination URL (tıklayınca gidilecek adres) giriliyor.
- Dışa aktarma hedefleri: Generic MRAID, Moloco, AppLovin, Google App Campaigns, Unity Ads, Meta, Pangle (TikTok), Mintegral, Liftoff. Dosyayı reklam platformuna kullanıcı kendisi yüklüyor.

Playable Games:
1. "Generate here" (web) ya da "Generate in Claude" (önce MCP bağlantısı gerekiyor) seçin.
2. Hedefi, kontrolleri, engelleri ve oyunun sonunu tarif edin.
3. 2D veya 3D seçin.
4. Türü seçin.
5. İsterseniz "Add reference" ile referans ekleyin.
6. Generate'e basın, test edin ve geliştirin.

Explore bölümünde örnekler oynanabiliyor ve "Recreate" ile çoğaltılabiliyor. Ürettikleriniz "My playables" altında.

**3. Kredi**: Kaynakta kredi veya fiyat yok [doğrulanacak]. Playable Ads yalnızca Enterprise.

**4. Sınırlar [resmî]**
- Yükleme limitleri yalnızca Playable Ads için belirtilmiş; Games için [doğrulanacak].
- Ads çıktısı 5 MB ile sınırlı.
- Yalnızca kullanım izniniz olan varlıkları kullanın.

**5. ÖNERİ**
- Distribütör olarak uygulama yüklemesi (app install) reklamı yapmadığımız için Playable Ads'in (Enterprise, ağ odaklı) bize faydası düşük.
- Playable Games ile basit bir marka mini oyunu düşünülebilir. Örnek: "Kirli arabayı 30 saniyede detayla" gibi bir runner veya puzzle; bayi, fuar ya da kampanya landing page'inde link olarak kullanılabilir. Bu düşük öncelikli bir deneme olur.
- Oyuna ürün şişesi görseli koyulacaksa üretilmiş değil **gerçek ürün PNG'si** yükleyin ve sonucu gözle kontrol edin.

**6. Kaynaklar**
- [resmî] https://higgsfield.ai/blog/higgsfield-playable-ads-and-games
- [resmî] https://higgsfield.ai/playable

### İlgili: Higgsfield Games / Games 2.0 (Supercomputer içinde)

**[resmî]** Metin tarifinden tarayıcıda çalışan, paylaşılabilir linki olan bir oyun üretiyor; kod, mantık, asset, yayına alma ve isteğe bağlı çok oyunculu mod dahil.
- Giriş: https://higgsfield.ai/games-intro , ya da Supercomputer → Gaming
- Seçenekler:
  - Tür: Shooter, Platformer, Novella, Hypercasual, Racing, Horror
  - Stil: Pixel Art, Minimalistic, ASCII, Voxel, Anime, 3D
  - Ortam: Medieval, Cyberpunk, Retro, Modern, Space, Fantasy
  - Çok oyunculu mod anahtarı (üretimden **önce** açılmalı)
- Görsel, ses ve kod/yayın aşamalarının her biri onaylanıyor. Marketplace'e yayınlanabilir ya da gizli tutulabilir.
- Kredi [resmî]: oyun başına ortalama yaklaşık 70 kredi (~$3,50) ile başlıyor; ücret aşama aşama düşüyor. Web'deki Unlimited, Supercomputer'ı kapsamıyor. Oyunlar, App ve Website'larla aynı aylık yayın limitini paylaşıyor.
- Games 2.0 (Eylül 2026) GPT-6 Astra üzerinde; ChatGPT eklentisi ve Supercomputer üzerinden erişiliyor.
- Kaynaklar: [resmî] https://higgsfield.ai/blog/higgsfield-ai-games , https://higgsfield.ai/blog/higgsfield-mcp-gpt6-astra-games-2

---

## Higgsfield Genjutsu

**1. Ne yapıyor [resmî]**
Mevcut bir videonun (gerçek çekim ya da üretilmiş) hareketini, kamerasını ve zamanlamasını koruyup bir kısmını yeniden kuruyor: kişi, mekân, ürün, kıyafet ya da yazı.
- Giriş: https://higgsfield.ai/genjutsu , veya Video → Create Video → Model: Higgsfield Genjutsu
- Çıkış: 1 Eylül 2026

**2. Nasıl kullanılır [resmî, help-center]**

Modlar:
- **Motion transfer**: yalnızca hareketi alır, karakter, mekân ve stil olarak yeni bir sahne kurar. İçinde bir **Style** bloğu var: kütüphaneden bir stil ya da referans görsellerle özel stil seçip Apply'a basılıyor. Changelog 30 Eylül'de bunu "Genjutsu Restyle, 20+ stil" olarak duyurmuş.
- **Objects swap**: seçilen tek bir öğeyi (kişi, ürün, kıyafet, yazı) değiştirir, sahnenin geri kalanını korur.

Adımlar:
1. Mod seçin.
2. Referans video yükleyin (**4–30 sn**) ya da Motion Library'den bir trend seçin. Motion Library'nin üç akışı var: Higgsfield picks, Community trending, Community new.
3. **En fazla 30** referans görsel ekleyin. Görseller Generations, Liked ya da AI Influencer karakterlerinden gelebilir.
4. (Motion transfer'de) isterseniz Style uygulayın.
5. İsteğe bağlı: Prompt anahtarını açıp kısa bir tarif yazın. Tam bir prompt gerekmiyor; preset tek başına yeterli olabiliyor ("30+" preset var).
6. Quality'yi seçin (480p / 720p / 1080p) ve Generate'e basın.

Dosya formatları [doğrulanacak]. Çıktı süresi kaynakta açıkça yazmıyor [doğrulanacak].

**3. Kredi [resmî, blog; "Eylül 2026'da doğrulandı"]**

| Süre | Çözünürlük | Kredi |
|---|---|---|
| 15 sn | 480p | 40 (~$2,00) |
| 15 sn | 720p | 104 (~$5,20) |
| 15 sn | 1080p | 144 (~$7,20) |

- İki mod aynı ücretle çalışıyor. Ücret her çalıştırmadan önce gösteriliyor.
- Genjutsu planınızın Unlimited listesindeyse web'deki üretimler kredi düşmüyor. API, MCP, CLI, eklentiler ve Supercomputer'da her zaman kredi düşüyor.
- [resmî, Facebook duyurusu] "Genjutsu ve Genjutsu Lite, seçili bölgelerde yeni kullanıcılar için ücretsiz denenebilir." Türkiye'nin bu bölgelerden biri olup olmadığı [doğrulanacak].
- [üçüncü taraf, aiposthub] API liste fiyatları: standart Genjutsu $0,318/s (480p), $0,681/s (720p), $1,632/s (1080p).

**4. Sınırlar**
- [resmî] Girdi 4–30 sn, en fazla 30 referans, çıktı en fazla 1080p.
- [resmî] İpuçları: hareketi net okunan kaynak klipler kullanın; referansları kaynak çekimin kadrajına yakın tutun; tam yeniden kurulum için ürünün birden fazla açıdan görselini verin.
- [üçüncü taraf] Kaynak videodaki ses korunabildiği için popüler müzik telif tespitine takılabilir. Yüzler için izin gerekiyor ve yasal zorunluluk olan yerlerde yapay zekâ etiketi konulmalı.

**5. ÖNERİ**
- **Objects swap**, ürün tarafında en umut verici araç. Bir kere çekilmiş "aplikasyon" videosundaki (sprey, pad, şişe tutma) şişeyi başka bir markanın ürünüyle değiştirmek, tek çekimden çok markalı varyasyon üretmenizi sağlar (MG Polishing → Gyeon → Menzerna).
  - **Risk**: etiket yazıları ve logo bozulabilir. Ürün başına 3–6 açıdan net, etiketi okunur, beyaz fonlu referans verin; çıktıyı kare kare kontrol edin.
  - Etiketin kamerada küçük ya da hareketli göründüğü planları tercih edin. Etiketin yakın çekim ve okunur olması gereken planları gerçek çekimle yapın.
- Motion transfer + Style, kampanya için "stilize" varyasyonlarda (anime, kil animasyon vb.) işe yarar; ürün doğruluğu kritik olmayan kısımlarda kullanın.
- Telif riski yüzünden kaynak videoların kendi çekimimiz olmasını tercih edin; trend Motion Library klipleri için müziği değiştirin.

**6. Kaynaklar**
- [resmî] https://higgsfield.ai/blog/higgsfield-genjutsu
- [resmî] https://higgsfield.ai/genjutsu
- [resmî] https://higgsfield.ai/creator-hub/help-center/tools/how-do-i-use-genjutsu
- [resmî] https://higgsfield.ai/creator-hub/changelog
- [resmî, sosyal] https://www.facebook.com/higgsfieldai.fb/videos/introducing-genjutsu-litedrop-your-photo-into-any-trending-video-and-youre-in-it/1479806000661983/
- [üçüncü taraf] https://www.aiposthub.com/higgsfield-genjutsu-lite-cost-math-likeness-risks/

---

## Genjutsu Lite (menüde FREE etiketi)

**1. Ne yapıyor [resmî]**
Genjutsu'nun daha hızlı ve daha ucuz sürümü. "Bir fotoğrafı trend bir videoya koy, sen de içinde ol." **Mod seçimi yok**: değişiklikleri otomatik uyguluyor (help-center ve blogdaki 20 Ekim güncellemesi). Changelog'un 19 Ekim kaydı ise Motion Transfer ve Object Swap'tan bahsediyor; bu çelişkili [doğrulanacak].
- Giriş: https://higgsfield.ai/genjutsu (Lite seçeneği) veya Video model seçicisi
- Lite ayrıca API ("Light" adıyla), MCP, CLI, eklentiler ve Supercomputer üzerinden de kullanılabiliyor.

**2. Nasıl kullanılır / sınırlar [resmî]**
- Referans görsel: **en fazla 10**.
- Çıktı: 720p veya 1080p (API'de 480p de var [üçüncü taraf]).
- **Klip süresinde çelişki [doğrulanacak]:**
  - Blog (20 Ekim güncellemesi) ve help-center: 4–30 sn
  - Changelog (19 Ekim): 4–15 sn
  - genjutsu sayfasındaki bir metin: "up to 30s"
  - Üçüncü taraf (aiposthub): 4–15 sn, yalnızca ilk 15 saniye kullanılıyor
  - Pratikte 15 saniyeyle sınırlı varsayın.
- Kullanım alanları: kısa Reels/TikTok/Shorts, hızlı testler, bir klipten çok sayıda varyasyon.

**3. Kredi / "FREE"**
- [resmî] Higgsfield.ai'de standart Genjutsu'nun yaklaşık üçte biri fiyatına. Kesin ücret üretimden önce gösteriliyor.
- [resmî, sosyal] 720p'de 3,5 kat, 1080p'de 5 kat daha ucuz. Seçili bölgelerde yeni kullanıcılar ücretsiz deneyebiliyor.
- Menüdeki "FREE" etiketinin tam anlamı resmî bir kaynakta açıklanmıyor [doğrulanacak]. Muhtemel açıklamalar: planınızın Unlimited listesinde olması ya da bölgesel ücretsiz deneme. Unlimited/ücretsiz kullanım **yalnızca web'de** geçerli; MCP, CLI ve API'de kredi düşer.
- [üçüncü taraf, aliteq] 720p: 30 kredi, 1080p: 60 kredi (klip başına). Bazı planlarda 2–3 ücretsiz Genjutsu çalıştırma hakkı var.
- [üçüncü taraf, aiposthub] API: $0,05/s (480p), $0,10/s (720p), $0,20/s (1080p). Lite, kaynak videonun süresini de faturalandırıyor.

**4. Sınırlar**
- Mod seçimi olmadığı için kontrol daha az.
- Kalite ve hız karşılaştırması yayınlanmamış [üçüncü taraf].
- Kaynak sesi koruyor (telif riski) [üçüncü taraf].

**5. ÖNERİ**
- "FREE" etiketini, ürün doğruluğunu test etmenin en ucuz yolu olarak kullanın: web arayüzünde 10 referansla (ürünün farklı açılarından çekilmiş gerçek fotoğrafları) aynı şişeyi kısa bir trend klibe yerleştirip etiketin ne kadar korunduğunu ölçün.
- Hedef: ürün yerleştirme testi ve "eğlenceli trend" Reels'leri. Bitmiş reklamda etiketin yakın planda göründüğü sahneler için standart Genjutsu ya da gerçek çekim kullanın.
- Otomasyon (CLI/MCP) üzerinden çağrıldığında FREE geçerli olmaz; toplu testleri web'de yapın.

**6. Kaynaklar**
- [resmî] https://higgsfield.ai/blog/higgsfield-genjutsu (20 Ekim güncellemesi)
- [resmî] https://higgsfield.ai/creator-hub/help-center/tools/how-do-i-use-genjutsu
- [resmî] https://higgsfield.ai/genjutsu
- [resmî] https://higgsfield.ai/creator-hub/changelog
- [üçüncü taraf] https://www.aiposthub.com/higgsfield-genjutsu-lite-cost-math-likeness-risks/ , https://aliteq.com/what-is-higgsfield-genjutsu

---

## Katana

**1. Ne yapıyor [resmî]**
Claude için bir Higgsfield "edit" skill'i. Bir referans kurguyu (kendi videonuz ya da Katana kütüphanesinden bir preset) **sizin karakterleriniz, ürünleriniz veya kıyafetlerinizle** yeniden kuruyor. Referansın plan sırasını, temposunu, kesmelerini ve müziğini koruyor. Higgsfield MCP konektörü üzerinden çalışıyor.
- Giriş: https://higgsfield.ai/katana (topluluk ve presetler)
- Claude'da `/katana` preset kataloğunu açıyor, `/katana/<preset-adı>` belirli bir preset'i çalıştırıyor. "Bu ürünle Higgsfield kullanarak bir edit yap" gibi düz bir istek de Katana'yı başlatıyor. ChatGPT eklentisinde de `/katana` geçiyor (higgsfield.ai/mcp).
- Changelog (8 Ekim 2026): Aura Farming, Motion ve Clipping stillerinde edit; edit başına en fazla 5 görsel.

**2. Nasıl kullanılır [resmî]**
1. Bir referans seçin: kendi kurgunuzu yükleyin ya da kütüphaneden bir preset seçin. Preset kategorileri: Personalized edits, Style transfer, Motion transfer. Kaynaklar: Higgsfield ve Community.
2. **En fazla 5 fotoğraf** ekleyin (karakter, ürün, kıyafet).
3. İsteğe bağlı talimat verin. Örnek: "en önemli ürün planı bu, bunu değiştirme".
4. Generate'e basın. Sonuç sohbette, indirme butonu olan bir widget'ta görünüyor ve Higgsfield Assets'e de kaydediliyor.
5. Düzeltmeleri düz cümleyle isteyin. Yazarın testinde yalnızca etkilenen planlar yeniden üretildi.

Çıktı: MP4. Süre, en-boy oranı ve fps referansla aynı; Claude'da ayrıca ayarlanamıyor.
- Yüklenen referans videonun azami süresi belirtilmemiş [doğrulanacak]. Topluluk preset'i yayınlamak için 3–30 sn hareket videosu ve en fazla 40 görsel gerekiyor.

**3. Kredi [resmî]**
- Mevcut plan kredilerinizi kullanıyor; ayrı MCP faturası ya da ek ücret yok.
- Claude her üretimden önce kesin kredi tutarını gösteriyor.
- Düzeltmeler yeni üretim gerektirirse ek kredi harcanıyor.
- Aktif Higgsfield aboneliği gerekiyor; API anahtarı gerekmiyor.
- Edit başına sabit kredi bilgisi yok [doğrulanacak].

**4. Sınırlar / bilinen sorunlar [resmî]**
- Claude sohbetine doğrudan eklenen görseller Katana'ya referans olarak **geçmiyor**. Higgsfield yükleme penceresi açılıyor ya da medya dosyasının doğrudan linki veriliyor.
- Instagram ve TikTok profil linkleri kabul edilmiyor; referans dosya olarak yüklenmeli.
- Bazı üretimler moderasyon tarafından reddedilebiliyor.
- Preset kütüphanesi zamanla değişiyor.

**5. ÖNERİ**
- Beğendiğimiz bir oto bakım kurgusunu (ör. hızlı kesmeli "before/after" detailing edit'i) referans alıp kendi ürün fotoğraflarımızla yeniden kurmak için uygun.
- 5 fotoğraf sınırı var. Şişe başına 2–3 net etiket fotoğrafı kullanıp tek ürüne odaklanın; çok markalı edit'lerde ürün karışması riski artar.
- Yalnızca kendi çektiğimiz ya da hakkı bizde olan kurguları referans alın (resmî kaynak da bunu istiyor).
- Mevcut CLI/Codex akışımızda Katana bir **Claude MCP skill'i** olarak tanımlı. CLI skill listesinde (generate, soul, product-photoshoot) yer almıyor [doğrulanacak].

**6. Kaynaklar**
- [resmî] https://higgsfield.ai/blog/higgsfield-katana
- [resmî] https://higgsfield.ai/katana
- [resmî] https://higgsfield.ai/creator-hub/changelog
- [resmî] https://higgsfield.ai/mcp

---

## AI Influencer (AI Influencer Studio)

**1. Ne yapıyor [resmî]**
Menülerle (prompt gerektirmeden) özgün bir yapay zekâ karakteri / influencer oluşturuyor ve onu trend videolara Genjutsu ile yerleştiriyor.
- Giriş: https://higgsfield.ai/ai-influencer-studio (Influencer builder sekmesi) ve https://higgsfield.ai/ai-influencer
- Yenilenmiş sürüm: 2–3 Ekim 2026

**2. Nasıl kullanılır [resmî, blog/new-ai-influencer]**
1. AI Influencer → Influencer builder'ı açın.
2. İsteğe bağlı: bir fotoğraf yükleyin. Kendinizin ya da izin vermiş birinin yüz hatları korunuyor.
3. Character type seçin: Average, Bold veya Extreme.
4. 19 ayarı doldurun ya da Randomize'a basın. Ayarlar: cinsiyet, etnik köken, yaş, ten rengi, boy, yapı, oranlar, özellikler, sakal, kafa şekli, boyun, göz şekli ve rengi, saç rengi ve modeli, ayırt edici özellikler, stil, aksesuar. Ayrıca tek cümlelik düzenleme yapılabiliyor (ör. "saçını kazı").
5. Generate'e basın. Çıktı bir yakın portre ve bir tam boy görsel (beyaz fon).
6. Recreate ile tekrar üretin, ya da Create/Assign to element ile karakteri kaydedin.
7. "Turn to motion" → Genjutsu (Motion transfer veya Objects swap) seçin. Referans video (sayfaya göre 3–30 sn, blogda 4–30 sn) ve en fazla 30 görsel ekleyin (ürün sayfası "40'a kadar" diyor [doğrulanacak]). Kaliteyi 480p, 720p ya da 1080p seçip üretin.

Ek bilgiler:
- Karakterler Cinema Studio'da AI Influencer sekmesinden, sahne tarifinde @ ile çağrılabiliyor.
- Batch varyasyon var: aynı kurulum farklı kıyafet, ürün veya mekânla tekrar üretilebiliyor.

**3. Kredi [resmî]**
- Karakter oluşturma ya da düzenleme: **1,12 kredi** (~$0,06; 20 kredi = $1).
- Video: ücret Generate butonunda gösteriliyor.
- Changelog (2 Ekim): her kullanıcıya 5 ücretsiz üretim. Kayıtta ücretsiz kredi veriliyor, miktarı belirtilmemiş.
- ChatGPT'deki AI Influencer eklentisi "ücretsiz denenebilir, kart gerekmez".
- Plan fiyatları (blog, "Ekim 2026'da doğrulandı"): Starter $15/ay; Plus $49/ay ($39 yıllık); Ultra $129/ay ($99 yıllık).

**4. Sınırlar**
- [resmî] Eski help-center sürümüne göre karakter görselleri 4K'ya kadar çıkıyordu; yeni sürümde piksel çözünürlüğü belirtilmemiş [doğrulanacak].
- [resmî] Başkasının yüzü yalnızca izinle kullanılabilir.

**5. ÖNERİ**
- Markadan bağımsız sabit bir "detailing ustası" ya da "marka yüzü" karakteri oluşturulabilir. Bu karakter Genjutsu Objects swap ile ürün tutarken ya da uygularken gösterilir; gerçek model çekimi maliyeti olmadan sürekli Reels üretilir.
- **Risk**: karakterin elindeki ürün yine üretilmiş olacak. Etiket doğruluğu için ürün referanslarını net verin ve etiketin yakın planda göründüğü kareleri gerçek ürün fotoğrafıyla değiştirin ya da yerine koyun.
- Türkiye'de yapay zekâ etiketlemesi ve reklam mevzuatı açısından "AI karakter" kullanımını açıkça belirtin (bu genel bir uyum notu, kaynak iddiası değil).

**6. Kaynaklar**
- [resmî] https://higgsfield.ai/blog/new-ai-influencer
- [resmî] https://www.higgsfield.ai/ai-influencer
- [resmî] https://higgsfield.ai/ai-influencer-studio (yalnızca meta veri okunabildi)
- [resmî] https://higgsfield.ai/creator-hub/help-center/tools/how-do-i-use-ai-influencer (eski sürüm)
- [resmî] https://higgsfield.ai/creator-hub/changelog

---

## ChatGPT Plugin (Higgsfield eklentisi)

**1. Ne yapıyor [resmî]**
ChatGPT içinden Higgsfield görsel ve video modellerini, Genjutsu'yu, efektleri ve skill'leri çalıştıran **resmî eklenti**. ChatGPT için MCP URL'si değil, eklenti kullanılıyor.
- Giriş: ChatGPT Plugins Directory, ya da https://higgsfield.ai/mcp?tab=chatgpt → "Add Higgsfield plugin"

**2. Nasıl kullanılır [resmî]**
1. Eklentiyi ekleyin, Higgsfield hesabınızla giriş yapıp yetki verin. API anahtarı gerekmiyor.
2. Yeni bir sohbet açın. Higgsfield'ı araçlardan seçin ya da `@Higgsfield` ile çağırın.
3. Slash komutları (changelog, 30 Eylül ve sonrası): `/effects`, `/genjutsu`, `/product`, `/motion`, `/marketing-studio`, `/katana`, `/ugc-flow`, `/use-after-effects`.
4. Referans görseli ataç simgesiyle ekleyin (**en fazla 20 MiB**). Görsel Higgsfield hesabınıza yükleniyor ve sohbette tekrar kullanılabiliyor. Model, en-boy oranı ve süreyi istemde belirtin.
5. Sonuç sohbet widget'ında görünüyor ve Assets'e kaydediliyor.

Ek bilgiler:
- Skill kategorileri: Marketing, UGC factory, Faceless content factory, Utility, Motion & Design.
- Games 2.0 de bu eklenti üzerinden çalışıyor.

**3. Kredi [resmî]**
- Her üretim standart ücretle kredi düşüyor; Unlimited yalnızca web'de geçerli.
- Higgsfield'ın kendi test örnekleri: 15 sn 1080p Seedance 2.5 UGC = 270 kredi; GPT Image 2 4K ürün çekimi = 48 kredi; Soul 2.0 karakter sayfası 2K = 0,5 kredi.

**4. Sınırlar [resmî]**
- ChatGPT'de **ses üretimi ve Website Building skill'i yok**.
- Kullanılabilirlik "plana, bölgeye ve workspace ayarlarına" bağlı olabilir.
- Doğal bir kredi limiti yok; "üretmeden önce onay al" talimatı yalnızca istem düzeyinde işliyor.

**5. ÖNERİ**
- Ekipte kod bilmeyen kişiler (sosyal medya sorumlusu) için en kolay yol bu: `/product`, `/marketing-studio` ve `/genjutsu` ile sohbetten ürün görseli veya Reels üretilebilir.
- Bütçe kontrolü için istemin başına "her üretimden önce kredi tutarını göster ve onay iste" yazmayı standart hâle getirin.
- Ürün referansı olarak her zaman gerçek, yüksek çözünürlüklü ürün fotoğrafı yükleyin (20 MiB sınırı içinde).

**6. Kaynaklar**
- [resmî] https://higgsfield.ai/blog/generate-ai-videos-from-chatgpt
- [resmî] https://higgsfield.ai/creator-hub/help-center/integrations/how-do-i-connect-higgsfield-to-ai-agent
- [resmî] https://higgsfield.ai/mcp
- [resmî] https://higgsfield.ai/creator-hub/changelog
- [üçüncü taraf] https://novoads.ai/blog/higgsfield-mcp (ChatGPT "MCP değil, resmî eklenti")

---

## MCP (Higgsfield MCP)

**1. Ne yapıyor [resmî]**
Claude ve diğer MCP uyumlu ajanların Higgsfield'da görsel, video, ses ve karakter üretmesini sağlayan uzak (remote) MCP sunucusu. OAuth ile çalışıyor, API anahtarı gerekmiyor.
- Sunucu: `https://mcp.higgsfield.ai/mcp` (resmî tek URL)
- Tanıtım sayfası: https://higgsfield.ai/mcp

**2. Nasıl kullanılır [resmî]**

Kurulum:
- Claude: Settings (ya da Customize) → Connectors → Add custom connector → ad "Higgsfield", URL yukarıdaki → Connect → yetki verin.
- Cursor: Customize → Marketplace → Higgsfield → Add.
- Diğer MCP istemcileri: sunucu URL'sini ekleyin.

Yetenekler:
- Görsel ve video üretimi (30+ model)
- Marketing Studio (ürün linkinden video reklam)
- Ad Multiplier
- Genjutsu (Motion Transfer / Object Swap / Restyle)
- Soul karakter
- Ses
- Asset kütüphanesi
- Kredi bakiyesi sorgulama
- Bundle'lar: Paid Ads, Motion Design, Production Skills (Blender, Adobe, DaVinci, TouchDesigner için 11 iş akışı)
- Yaklaşık 41 iş akışı; örnekler: Ad Recreator, Hook/Headline Multiplier, Ad Localizer, Ad Resizer, Product Review / Unboxing UGC

Çıktılar Assets'te "MCP" kaynağı etiketiyle görünüyor.

**3. Kredi [resmî]**
- "MCP her zaman kredi kullanır." Unlimited ve ücretsiz üretimler yalnızca web'de geçerli.
- Tüm bağlı ajanlar aynı hesabı ve krediyi paylaşıyor.
- **Aktif ücretli abonelik gerekiyor.**
- İstisna: 24 saatlik "Unlimited MCP" denemesi (Temmuz 2026, yeni kullanıcılar, Plus planına otomatik geçiş). Bu kampanya sona ermiş görünüyor.

**4. Sınırlar / sorunlar [resmî]**
- Ajan, sohbete eklenen dosyaları okuyamıyor. Yerel dosyalar Higgsfield yükleme penceresiyle yükleniyor; web görselleri URL ile içe aktarılabiliyor.
- Doğal bir kredi limiti yok.
- Bilinen hatalar ve çözümleri:
  - "Authorization with the MCP server failed": bağlantıyı kesip yeniden yetki verin.
  - "MCP HTTP exchange failed": tekrar deneyin.
  - Üretim görünmüyorsa 60 saniye bekleyin, sonra Manage Account → Usage'a bakın.
- Kullanım Developer Terms'e tabi; ajanın hesabınızla ürettiği her şeyden siz sorumlusunuz.

**5. ÖNERİ**
- Higgsfield'ın kendi ayrımına göre: **sohbet ajanları (Claude web/Desktop/Cowork) için MCP**, **kod ajanları (Claude Code, Codex, Cursor) için CLI + Skills** daha verimli; CLI'da token yükü daha düşük. Mevcut CLI + Codex/Claude Code akışımız bu öneriyle uyumlu; ikisine birden ihtiyaç yok.
- MCP'yi ek olarak; Katana, Content Factory (`/content-factory`), Ad Multiplier ve Ad Localizer (TR/EN yerelleştirme) gibi yalnızca MCP skill'i olarak sunulan iş akışları için kullanın.
- Kredi koruması için ajan talimatına "her üretimden önce kredi teklifi göster ve onay bekle" kuralını yazın.

**6. Kaynaklar**
- [resmî] https://higgsfield.ai/mcp
- [resmî] https://higgsfield.ai/creator-hub/help-center/integrations/what-is-higgsfield-mcp
- [resmî] https://higgsfield.ai/creator-hub/help-center/integrations/how-do-i-connect-higgsfield-to-ai-agent
- [resmî] https://higgsfield.ai/creator-hub/help-center/integrations/how-do-i-access-higgsfield-via-cli
- [resmî] https://higgsfield.ai/blog/unlimited-mcp

### Ek: CLI (bağlam için) [resmî]

Kurulum:
- `npm i -g @higgsfield/cli`
- `higgsfield auth login`
- `npx skills add higgsfield-ai/skills`

Skill'ler ve presetler:
- 3 skill: **generate** (4K'ya kadar), **soul**, **product-photoshoot**
- Görsel presetleri (10): product_shot, lifestyle_scene, closeup_product_with_person, pinterest_pin, hero_banner, social_carousel, ad_creative_pack, virtual_model_tryout, conceptual_product, restyle
- Video presetleri (9): UGC, Tutorial, Unboxing, Hyper Motion, Product Review, TV Spot, Wild Card, UGC Virtual Try On, Pro Virtual Try On

Notlar:
- Bilinen sorun: referans görseller iletilmiyorsa kurulum komutunu yeniden çalıştırıp güncelleyin. Güncel sürümler tüm referansları iletiyor. **Bizim için kritik: ürün referansının gerçekten iletildiğini kontrol edin.**
- CLI skill'leri ile Supercomputer skill'leri aynı şey değil.

---

## API (genel bakış)

**1. Ne yapıyor [resmî]**
Kendi kodunuzdan 50+ video ve görsel modeline erişim sağlayan, ayrı bir geliştirici ürünü. **Web planlarından, kredilerden ve MCP/CLI'dan bağımsız**; USD bakiye ile kullandıkça ödeniyor.
- Çıkış: 16 Eylül 2026
- Konsol: open.higgsfield.ai ("Open Higgsfield"); blogda console.higgsfield.ai/dashboard olarak da geçiyor
- Endpoint: api.higgsfield.ai
- Dokümantasyon: docs.higgsfield.ai

**2. Nasıl kullanılır [resmî]**
1. API hesabı açın (bireysel ya da şirket).
2. Ödeme yöntemi ekleyin; en az $5 yükleyin.
3. API anahtarı oluşturun. Anahtar **yalnızca bir kez** gösteriliyor ve kaybolursa geri alınamıyor.
4. Python SDK, TypeScript SDK ya da REST ile bağlanın.

Çalışma şekli:
- Asenkron: istek gönderilir, request ID döner, ardından durum sorgulanır (polling) ya da webhook beklenir, sonuç indirilir.
- Bir tahmin (estimate) endpoint'i çalıştırmadan önce maliyeti döndürüyor.
- Modeller: Seedance, Kling, Wan, MiniMax, PixVerse, LTX, Grok, Ideogram, Recraft, Qwen, ve Higgsfield'ın kendi modelleri Soul 2, Soul Cinema, DoP, Marketing Studio Image. Katalog web'den farklı olabilir. Ayrı bir ses modeli yok.
- Genjutsu ve Genjutsu Lite ("Light") API'de de mevcut.
- Kimlik doğrulama header formatı [doğrulanacak]. Üçüncü taraf kaynaklar çelişiyor: `Key id:secret` mi, Bearer mı?

**3. Fiyat [resmî, blog; başlangıç fiyatları]**

| Model | Fiyat |
|---|---|
| Marketing Studio Image | $0,0059 / görsel |
| Soul 2 | $0,0032 / görsel |
| DoP | $0,125 / üretim |
| Kling 2.6 | $0,07 / sn |
| Kling 3.0 | $0,112 / sn |
| Seedance 2.5 | $0,0738 / sn |
| Seedance 2.0 | $0,9332 / sn |
| Wan 3.0 | $0,20 / sn |

- Fiyatlar çözünürlük ve sese göre değişiyor.
- Bakiye bir yıl sonra sona eriyor ve eksiye düşemiyor.
- Yalnızca başarılı üretimler ücretlendiriliyor.
- Promosyonlar (changelog): Ekim'de ilk $100'dan sonra $15 bonus ve %20'ye kadar cashback; Wan 3.0 31 Ekim'e kadar %60 indirimli.

**4. Sınırlar [resmî]**
- API anahtarı oluşturunca 20 eşzamanlı istek açılıyor; bu limit yükleme hacmiyle artıyor.
- Çıktılar **en az 7 gün** saklanıyor; kendi depolamanıza indirin.

**5. ÖNERİ**
- Çok sayıda SKU için şablon üretimi (ör. her ürün için aynı fon ve ışıkta katalog görseli) gerektiğinde, Marketing Studio Image'in görsel başına ~$0,006 fiyatı plan kredisinden ucuz olabilir. Kendi script'imizle toplu iş + webhook + otomatik indirme kurulabilir.
- Plan kredilerinden bağımsız olduğu için "ayrı bütçe" olarak yönetilebilir.
- Ürün doğruluğu için insan onaylı bir QA adımı (etiket ve logo kontrolü) pipeline'a eklenmeli.

**6. Kaynaklar**
- [resmî] https://higgsfield.ai/blog/higgsfield-api
- [resmî] https://higgsfield.ai/creator-hub/help-center/integrations/what-is-the-higgsfield-api
- [resmî] https://higgsfield.ai/creator-hub/changelog
- [üçüncü taraf] https://www.layer3labs.io/guides/higgsfield-api , https://pasqualepillitteri.it/en/news/18087/higgsfield-ai-free-open-source-pay-per-use-models

---

## Supercomputer (ilişki)

**1. Ne yapıyor [resmî]**
Higgsfield'ın sohbet tabanlı ajan çalışma alanı. Görevi planlıyor, her adım için model seçiyor (Soul, Cinema Studio, Seedance, Nano Banana vb.), üretip birleştiriyor. Düzeltme istendiğinde yalnızca değişen kısmı yeniden çalıştırıyor.
- Giriş: https://higgsfield.ai/supercomputer (higgsfield.ai → Supercomputer)

**2. Özellikler [resmî]**
- Sohbet LLM'i: otomatik yönlendirme ya da Anthropic, OpenAI, Google, xAI, DeepSeek modellerinden seçim.
- Projects (ortak workspace) ve Memory.
- Konektörler: Telegram, Slack, TikTok, Gmail, Google Drive, Notion.
- Sidebar: Apps, **Games**, Skills (resmî, topluluk, kişisel), Faceless channel (YouTube için 15 dakikaya kadar, 12 stil).
- "Ask before generating" seçeneği var.
- Skill'ler: Ad Multiplier, Editorial Motion Graphics, Faceless Video, SaaS/Physical UGC Video, Brandkit, Shorts Maker, Website Building.
- **Diğer kapsam özellikleriyle ilişkisi:**
  - Content Factory: Supercomputer'da skill olarak var.
  - Games: Supercomputer'ın içinde.
  - Genjutsu Lite: Supercomputer'dan erişilebilir.
  - Katana: bir Claude MCP skill'i; Supercomputer'da olup olmadığı [doğrulanacak].

**3. Kredi [resmî]**
- Her adım standart ücretle kredi düşüyor ve süren maliyet görev sırasında gösteriliyor.
- Kaynaklar burada çelişiyor [doğrulanacak]:
  - Help-center: "web-only unlimited access applies to Supercomputer"
  - Games blogu: "Unlimited … does not extend to Supercomputer"
  - MCP makalesi: Supercomputer'ı her zaman kredi düşen araçlar arasında sayıyor
- [üçüncü taraf, all-ai.de] Reddit'te bir kullanıcı 5 saniyelik bir reklam klibinin 700+ kredi tükettiğini bildirmiş.
- Depolama plana bağlı; ek depolama satın alınabiliyor.

**4. Sınırlar**
- Karmaşık görevler tek üretimden çok daha fazla kredi harcıyor.
- [üçüncü taraf] Zamanlanmış görev özelliği resmî help-center'da yok [doğrulanacak].

**5. ÖNERİ**
- Kod yazmadan çok adımlı kampanyalar (Brandkit → UGC → varyasyon) için kullanışlı. Ancak maliyet hızla büyüyebileceği için "Ask before generating" seçeneğini açık tutun.
- Mevcut CLI + Codex akışımız zaten benzer orkestrasyonu daha kontrollü yapıyor; Supercomputer'ı daha çok Content Factory/Faceless channel denemeleri ve Brandkit için düşünün.
- Google Drive konektörü, ürün fotoğraf arşivine erişim için faydalı olabilir.

**6. Kaynaklar**
- [resmî] https://higgsfield.ai/creator-hub/help-center/tools-and-workflows/how-do-i-use-supercomputer
- [resmî] https://higgsfield.ai/supercomputer
- [resmî] https://higgsfield.ai/blog/higgsfield-ai-games
- [üçüncü taraf] https://www.all-ai.de/news/news26top/supercomputer-higgsfield-agent , https://postium.ru/higgsfield-predstavila-supercomputer/

---

## Özet: ürün doğruluğu açısından öncelik (ÖNERİ)

| Özellik | Ürün/etiket kontrolü | Bizim için öncelik |
|---|---|---|
| Genjutsu Objects swap | Orta: 30 referansla en iyi kontrol; etiket bozulabilir | Yüksek: tek çekimden çok markalı varyasyon |
| Genjutsu Lite (FREE) | Düşük-orta: en fazla 10 referans, mod seçimi yok | Yüksek: ucuz test alanı (web'de) |
| Katana | Orta: en fazla 5 fotoğraf | Orta-yüksek: kurgu şablonu kopyalama |
| AI Influencer | Karakter iyi; ürün üretilmiş | Orta: sabit marka yüzü |
| Content Factory | Ürün girdisi yok | Orta: eğitici "faceless" içerik (ürünsüz) |
| ChatGPT Plugin / MCP | Araca bağlı | Ekip içi erişim kolaylığı |
| API | Modele bağlı | Toplu SKU otomasyonu için ileride |
| Playable | Enterprise / oyun | Düşük |
