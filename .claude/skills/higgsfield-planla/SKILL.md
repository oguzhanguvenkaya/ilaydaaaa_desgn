---
name: higgsfield-planla
description: Kullanıcı Higgsfield ile ne yapmak istediğini anlattığında (ürün görseli, post, carousel, Reels, reklam, video düzenleme, 3D, seslendirme, eğitici içerik vb.) hangi Higgsfield araçlarının hangi sırayla, nerede (web / CLI / MCP / eklenti) ve hangi ayarlarla kullanılacağını güncel ve kaynaklı bilgiyle planlar, maliyet ve ürün etiketi riskini gösterir ve kullanıcıyı adım adım yönlendirir. "Higgsfield'da şunu yapmak istiyorum", "hangi aracı kullanayım", "bunu nasıl yaparım", "planla", "yol göster" gibi isteklerde kullan.
---

# Higgsfield iş planlayıcı

Görev: Kullanıcının anlattığı hedefi, Higgsfield araçlarıyla yapılabilir, sıralı, maliyeti ve riski belli bir **plana** dönüştürmek ve kullanıcıyı bu planda adım adım yönlendirmek.

Plan, ezberden değil **güncel ve kaynaklı** bilgiyle yapılır. Higgsfield çok sık değişiyor; yerel notlar tarihli kanıttır, son söz canlı katalog ve resmî belgedir.

## Temel kurallar

- Türkçe ve sade yaz. Teknik terimi ilk geçtiği yerde bir örnekle açıkla (kullanıcı kreatif terimleri zor buluyor).
- Kaynakta olmayan sayı veya iddia uydurma; emin değilsen `[doğrulanacak]` yaz. Kaynak, tarih ve resmî / üçüncü taraf ayrımını belirt.
- **Planlama ücretsizdir; üretim değildir.** Plan aşamasında ücretli üretim, preset çalıştırma (`execute_preset`) veya Katana oturumu açma yok. Kullanıcı planı onaylayıp açıkça "başlat" demeden kredi harcanmaz.
- Ürün doğruluğu (etiket, logo, ambalaj, şekil) en önemli kriter. Her adımın etiket riskini yaz. Higgsfield'in hiçbir aracı bunu garanti etmiyor.
- Ürün veya marka geçiyorsa `higgsfield_test` reposundaki kurallar geçerlidir: `AGENTS.md`, `docs/urun-dogruluk-protokolu.md`, `brands/<marka>/profile.json`, `catalog/index.json`, `docs/urun-aciklamalari.md`. Repo yan klasörde yoksa kullanıcıya söyle.

## Adımlar

### 1. Hedefi anla (intake)

Önce kullanıcının mesajından çıkarabildiğin her şeyi çıkar, sonra **yalnızca planı değiştirecek eksikleri** sor: en fazla 3 kısa soru, tek mesajda. Her soruya bir varsayılan öner ("bilmiyorsan şunu kullanırım").

Kontrol listesi:

| Konu | Neden önemli | Varsayılan |
|---|---|---|
| Ne üretilecek (tek görsel, carousel, Reels, reklam seti, video düzenleme, 3D, ses…) | Araç ailesini belirler | — (sorulur) |
| Ürün / SKU ve marka | Etiket kuralları, referans seçimi | Ürünsüz içerik |
| Hedef kitle (son kullanıcı / profesyonel usta / bayi) | Ton, içerik türü, B2B mi B2C mi | Ürün ailesinden çıkar ([kurumsal rehber](../../../docs/kurumsal-icerik-rehberi.md) 4. bölüm) |
| Elde gerçek materyal var mı (ürün fotoğrafı, çekim videosu, logo dosyası) | En güvenli yol gerçek materyalden başlamaktır | Yok kabul etme, sor |
| Kanal ve format (Instagram feed 4:5, Reels 9:16, Meta reklam 1:1/4:5/9:16, web banner…) | Oran, süre, çözünürlük | Kanaldan çıkar |
| Süre / adet | Kredi | Reels 8–15 sn; görselde 3 varyant |
| Ekranda yazı veya seslendirme (dil) | Türkçe ses desteği sınırlı | Yazıyı sonradan kurguda ekle |
| Bütçe (kredi) ve teslim zamanı | Model ve çözünürlük seçimi | Önce taslak 480p/720p |
| Kullanılabilen kanallar (web, CLI, MCP, hangi masaüstü uygulamaları) | Adımın nerede yapılacağı | Web + CLI |

### 2. Aday araçları seç (yerel bilgi)

Şunları oku:

0. `docs/kurumsal-icerik-rehberi.md`: firmanın profesyonel çizgisi (2. bölüm), marka kuralları ve Higgsfield karşılığı (3. bölüm), **ürünün ailesine göre tarif ve riskler** (4. bölüm), içerik türü (5. bölüm), trend çerçevesi (6. bölüm). Plan bu çerçeveye uymalı; uymayan bir istek varsa nedenini söyleyip alternatif öner.
1. [references/arac-secim-haritasi.md](references/arac-secim-haritasi.md): hedef → araç zinciri; her aracın canlı kontrol komutu.
2. `docs/ozellik-rehberi.md`: 2. bölümdeki "ürün piksellerine dokunma" seviyeleri ve 3. bölümdeki içerik türüne göre akışlar.
3. Gerekirse `docs/ozellik-envanteri.md`, `bilgi/canli-katalog-*/README.md` ve ilgili `research/<tarih>/` dosyası.

Kural: Etiketin okunduğu kare, 0–2. seviye araçlardan (gerçek katman, renk/ışık, maskeli bölgesel düzenleme) gelmeli. 3–5. seviye araçlar atmosfer, hook ve geçiş için kullanılır.

### 3. Canlı doğrula (zorunlu)

Plana koyduğun **her model ve iş akışı için** güncel bilgiyi kontrol et. Ayrıntılar [references/canli-bilgi-kaynaklari.md](references/canli-bilgi-kaynaklari.md).

- **Higgsfield MCP bağlıysa:**
  - `models_explore(action:"get", model_id)`: parametreler, süre, oran, girdi rolleri, Unlimited kapsamı.
  - `models_explore(action:"recommend", query)`: emin değilsen öneri al.
  - `get_workflow_instructions(workflow)`: Higgsfield'in kendi resmî iş akışı kılavuzu. Hangi modelin kilitli olduğunu, hangi soruların sorulacağını ve sınırları buradan al. Gerekirse `get_workflow_bundle_file` ile alt belgelerini oku.
  - `get_presets(source, category, query)` ve `get_preset_instructions(preset)`: hazır tarifler ve şablonlar. **Yalnızca okuma**; `execute_preset` çağırma.
- **CLI kuruluysa:** `higgsfield model get <id> --json`, `higgsfield workflow get <id> --json`, `higgsfield preset list ... --json`.
- **Web:** Yerel bilgi 14 günden eskiyse, çelişkiliyse veya araç yeni çıktıysa resmî kaynakları ara: higgsfield.ai help-center, blog, changelog. Üçüncü taraf kaynakları yalnızca işaretleyerek kullan.

Bulduğun yeni veya farklı bilgiyi plana kaynak ve tarihle yaz. Bilgi kalıcı değerdeyse 7. adımdaki gibi kaydet.

### 4. Planı yaz

[references/plan-sablonu.md](references/plan-sablonu.md) şablonunu kullan. Örnek: [references/ornek-plan.md](references/ornek-plan.md). Planda bulunması gerekenler:

- Bir cümlelik özet ve neden bu yolun seçildiği.
- Numaralı adımlar. Her adımda: araç ve tam modeli, **nerede yapılacağı** (web tıklama yolu / CLI komutu / MCP aracı / eklenti paneli), girdiler (hangi gerçek dosya, hangi rolde), ayarlar, beklenen çıktı, etiket riski ve kontrolü, kredi tahmini ve kaynağı.
- Adımlar arası bağımlılık (hangi çıktı hangi adıma girer).
- Toplam kredi aralığı ve önce yapılacak ucuz deneme.
- Alternatif yol (daha ucuz, daha güvenli ya da daha hızlı).
- Riskler, `[doğrulanacak]` noktalar, kaynaklar.
- Kullanıcıdan istenen tek net karar ("Plan uygun mu? 1. adımdan başlayalım mı?").

Kredi: Mümkünse `higgsfield generate cost` (CLI) ile gerçek ayarlarla tahmin al. Alamıyorsan blog/help fiyatını tarihiyle ver ve "kesin tutar Generate düğmesinde görünür" de.

### 5. Yönlendir

Onaydan sonra adım adım ilerle:

- **Web adımı:** Kullanıcıya tıklama yolunu ve girilecek değerleri ver. Sonucu beklemesini ve çıktıyı (dosya veya link) geri getirmesini iste.
- **CLI / MCP adımı:** Komutu göster. Kullanıcı üretimi onayladıysa çalıştır. Hesap ve workspace doğrulamasını yap (`higgsfield account status`, `higgsfield workspace list`).
- **Eklenti adımı:** Hangi panelde, hangi aracın, hangi katmanda kullanılacağını söyle.
- Her adımdan sonra kontrol listesini uygula: etiket ve logo %100 zoom'da gerçek ürünle karşılaştırılır; videoda klibin tamamı izlenir. Sorun varsa bir sonraki adıma geçmeden düzeltme yolunu öner.
- Plan değişirse (yeni bilgi, başarısız adım) planı güncelle ve değişikliği açıkça söyle.

### 6. Kayıt

Ürün içeren üretimlerde `higgsfield_test` üretim günlüğüne kaydet (`tools/production_log.py`): kullanılan gerçek referanslar, model, ayarlar, job ID'leri, gözlenen kredi, değerlendirme. Bu kaydı kullanıcı istemese de öner.

### 7. Bilgiyi güncel tut

Canlı kontrolde rehberdekinden farklı ve kalıcı değerde bir bilgi bulduysan:

- `research/<bugünün tarihi>/` altına kaynaklı kısa bir not ekle.
- `docs/ozellik-envanteri.md` içindeki ilgili satırı güncelle.
- Eski kanıt dosyalarını değiştirme.
- Commit mesajında neyin değiştiğini yaz.
