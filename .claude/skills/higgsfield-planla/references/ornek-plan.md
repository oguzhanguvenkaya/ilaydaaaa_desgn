# Örnek plan (gösterim amaçlı, üretilmedi)

Bu örnek planın biçimini ve ayrıntı düzeyini gösterir. Ürün bilgileri `higgsfield_test/campaigns/2026-09-rx-pro-lansman/README.md` kaydından alındı. Kling 4.0 kısıtları ve `/label-trace` tarifi 26 Ekim 2026'da canlı MCP ile kontrol edildi. Diğer kredi rakamları tarihli blog örnekleridir.

**Kullanıcının isteği:** "RX Pro için 15 saniyelik bir Instagram Reels lansman videosu istiyorum. Elimde ürün fotoğrafları var, kullanım videosu yok."

---

## Plan: RX Pro lansman Reels (15 sn, 9:16)

**Hedef:** MG PS RX PRO'nun (MG-RPV002) satışa çıktığını duyuran, ürünün doğru göründüğü 15 sn'lik Reels.
**Teslim:** 9:16, 1080×1920, yaklaşık 15 sn, müzikli; yazılar Türkçe.
**Kısa yol:** Videonun büyük kısmını gerçek fotoğraftan kuruyoruz (etiket kesin doğru kalır). Yalnızca açılıştaki 3–5 sn'lik hareketli planı yapay zekâ üretiyor ve o planın ilk ve son karesini gerçek fotoğrafa kilitliyoruz. Yazılar kurguda ekleniyor, AI'a yazdırılmıyor.
**Bilgi tarihi:** 26 Ekim 2026. Kling 4.0 kısıtları canlı katalogdan, `/label-trace` tarifi canlı talimattan, kredi örnekleri blogdan (tarihleri aşağıda).

### Hazırlık (ücretsiz)
- [ ] Ana fotoğraf: `IMG_2033.jpg` (`rxpro.yan`, S/N 226060288). Kampanya kaydına göre logo, turuncu tetik ve siyah taban incelendi.
- [ ] `IMG_1867.jpg` yalnızca teknik bilgi kaynağı; ana fotoğrafın üstüne yapıştırılmayacak (farklı cihaz olabilir).
- [ ] Metinler kampanya kaydından: "RX PRO İLE TANIŞIN", "1200 W rotary polisaj makinesi", "450–2000 dev/dk", "6 kademeli devir ayarı", "Şimdi satışta". Kaynak: Excel D578 + etiket fotoğrafı.
- [ ] `higgsfield account status` → hesap `mtskimyaweb`, workspace doğrulaması.

### Adımlar
| # | Ne yapılacak | Araç / model | Nerede | Girdi → çıktı | Ayarlar | Etiket riski ve kontrol | Kredi (kaynak) |
|---|---|---|---|---|---|---|---|
| 1 | 9:16 ana kare (master) | Photoshop veya Figma; gerekirse eklentiyle yalnızca fon | Eklenti paneli / elle tasarım | IMG_2033 → 1080×1920 PNG, koyu grafit fon | Ürün ayrı katman, gövde ve taban kesilmez | **0**: ürün pikselleri değişmez | Elle tasarım: 0; eklentiyle fon: [doğrulanacak] |
| 2a | Açılış planı, taslak A | Kling 4.0 (`kling4_0`, mode `image-to-video`) | CLI: `higgsfield generate ...` veya web: Video → Create Video → Kling 4.0 | `start_image` = master, `end_image` = master → 5 sn klip | 9:16, 720p, 5 sn; prompt: yavaş push-in ve ışık süpürmesi, ürün sabit | **3**: ara karelerde "MG PS POLISHER" yazısı bozulabilir; klip kare kare izlenir | ~25 (Kling 4.0 blogu, Ekim 2026) |
| 2b | Açılış planı, taslak B | MiniMax H3 (`minimax_h3`) | Aynı | Aynı | 9:16, 2K, 5 sn | **3**: sayfa "packaging labels render cleanly" diyor; test edilmedi | ~20 (H3 blogu) |
| 3 | Kazanan taslağın finali | 2a veya 2b | Aynı | Aynı | Kling için 1080p 5 sn | 3 | ~37,5 (Kling 1080p 5 sn) veya H3 aynı ~20 |
| 4 | Detay planları | Kurgu programı (Ken Burns: fotoğrafa yavaş yakınlaşma) | Premiere / DaVinci / CapCut | IMG_2033'ün tetik ve gövde bölgesi → 3–4 sn'lik planlar | Yazılar: devir aralığı, 6 kademe | **0** | 0 |
| 5 | Kurgu ve yazılar | Premiere / DaVinci veya MCP `video-montage` | Masaüstü / MCP | 0–4 sn AI açılış → 4–11 sn detaylar + özellik yazıları → 11–15 sn master + "Şimdi satışta" | Türkçe yazılar kurguda, AI'da değil | 0 | Masaüstü: 0; `video-montage`: [doğrulanacak] |
| 6 | Renk birliği (isteğe bağlı) | DaVinci AI LUT Creator veya Color Palette | Eklenti / web | Kurgu → aynı tonda video | Hafif ton; turuncu tetik rengi kaymamalı | **1** | Color Palette 15 sn: 135 (Ağustos blogu) [güncel tutar doğrulanacak]; LUT: [doğrulanacak] |
| 7 | Kontrol ve kayıt | — | — | Bitmiş video | Tüm klip izlenir; logo ve yazı kare kare | — | 0 |

### Adım ayrıntıları
**2. Açılış planı neden iki modelle taslak?** Her iki model de katalogda ilk ve son kare (`start_image`, `end_image`) kabul ediyor. Kling 4.0 metin ve logo desteği, H3 ise ambalaj etiketi iddiası taşıyor. Bizim ürünümüzde hangisinin etiketi daha iyi koruduğunu bilmiyoruz. Ucuz taslakla (toplam ~45 kredi) ölçüp yalnızca kazananı finale taşıyoruz.

**Neden hazır `/label-trace` tarifini kullanmıyoruz?** Canlı talimata göre bu tarif önce ürünü Nano Banana Pro ile yeniden çiziyor, sonra 3:4 bir video üretiyor. Gerçek fotoğrafı doğrudan kullanmadığı için etiket riski bizim yolumuzdan yüksek. Formatı da 9:16 değil, 3:4. Karşılaştırma için ayrıca denenebilir.

**Dikkat:** Prompt'a ürünü döndürme, ele alma veya kapağı açma gibi hareketler yazma. Etiketi en çok bunlar bozar. Kampanya kaydına göre kullanım sahnesi bu ilk iş için gerekli değil.

### Bütçe
- Ucuz deneme: 2a + 2b ≈ 45 kredi.
- Tam iş: ≈ 45 + 20–37,5 (final) ≈ 65–85 kredi. İsteğe bağlı 6. adım bu tutarı artırır.
- Kesin tutar: `higgsfield generate cost kling4_0 ...` veya Generate düğmesi.

### Alternatif yol
- **En güvenli ve 0 kredi:** AI hiç kullanmadan master ve detay fotoğraflarından Ken Burns'lü bir Reels yapmak. Sonra yalnızca açılış planını AI ile eklemenin fark yaratıp yaratmadığına bakılır.
- **Daha sinematik:** Cinema Studio 4.0 (≤30 sn, ≤50 referans). Ürün tüm klip boyunca yeniden çizildiği için etiket riski daha yüksek (4).

### Riskler ve açık noktalar
- AI planın ara karelerinde logo veya yazı bozulabilir. Bozuksa planı kısalt ya da yalnızca ilk karede kalan bir "ışık süpürmesi"ne indir.
- Marka/logo IP filtresi üretimi engelleyebilir; engellenirse "I own the rights" seçeneği [doğrulanacak].
- Türkçe dış ses istenirse katalogda Türkçe açıkça listelenmiyor; önce 15 sn ses testi [doğrulanacak].
- Blog fiyatları tarihli; Kling 4.0 kredisi plana göre değişebilir.

### Kaynaklar
- Canlı: `models_explore get kling4_0` (26.10.2026): mode image-to-video, 3–30 sn, 720p/1080p, start_image/end_image, 9:16.
- Canlı: `get_preset_instructions("/label-trace")` (26.10.2026).
- `research/2026-10-26/E-video.md`: Kling 4.0 ve MiniMax H3 kredi örnekleri ve iddiaları (Higgsfield blogu, Ekim 2026).
- `higgsfield_test/campaigns/2026-09-rx-pro-lansman/README.md`: ürün bilgisi, fotoğraf seçimi, metin kaynakları.

**Karar:** Plan uygun mu? Önce 1. adımdaki master kareyi hazırlayalım mı, yoksa ilk denemeyi tamamen ücretsiz yoldan (Alternatif 1) mı yapalım?
