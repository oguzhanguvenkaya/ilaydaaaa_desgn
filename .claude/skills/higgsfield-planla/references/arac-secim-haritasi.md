# Araç seçim haritası: hedef → araç zinciri

Bu harita **başlangıç noktasıdır**, son karar değildir. Plana koymadan önce her aracı canlı kontrol et ("Canlı kontrol" sütunu). Risk seviyeleri `docs/ozellik-rehberi.md` 2. bölümdedir: 0 = ürün piksellerine dokunmaz … 5 = stilize yeniden çizim.

Tarih: 26 Ekim 2026. Kredi örnekleri araştırma dosyalarındaki tarihli blog rakamlarıdır.

## A. Ürün görseli / post / carousel

| Hedef | Önerilen zincir (sırayla) | Risk | Canlı kontrol | Alternatif |
|---|---|---|---|---|
| Gerçek ürün fotoğrafıyla etiketi kesin doğru post | Upscale Standard (`topaz_image` Standard V2 veya `bytedance_image_upscale`) → Photoshop'ta ürün ayrı katman → eklentiyle arka plan (Generate Image / Mockup Studio) → kopya katmanda Relight → Expand ile oran türevleri | 0–1 | `models_explore get topaz_image`; `/use-photoshop` | Figma eklentisi (yazı ve logo vektör kalır) |
| Gerçek fotoğrafta yalnızca arka planı değiştir (eklentisiz) | Inpaint (`nano_banana_2_1` veya `nano_banana_2` + `is_inpaint` + mask; webde NB Pro Inpaint) → etiket maskenin dışında | 2 | `models_explore get nano_banana_2_1` | `seedream_v5_pro` `is_inpaint` |
| Hızlı fikir / konsept packshot | Resmî `product-photoshoot` iş akışı (`nano_banana_pro` 2k, ürün referansıyla) | 4 | `get_workflow_instructions("product-photoshoot")` | Canvas'ta NB Pro / GPT Image 2.5 Sunburst / Seedream 5.0 Pro yan yana |
| Şeffaf arka planlı ürün kesimi | `image_background_remover` veya `bytedance_image_upscale` `remove_bg` | 1 | `models_explore get` | `gpt_image_2_5` `background:"transparent"` (yeniden üretir, risk 4) |
| Carousel (3–10 sayfa) | `product-photoshoot` → `social-carousel` modu; yazılar Figma'da | 4 (+ yazı 0) | `get_workflow_bundle_file(product-photoshoot, references/social-carousel.md)` | Hazır tarifler: `swipe-opener`, `three-reasons`, `usage-guide`, `specs` |
| Bilgi kartı (kullanım adımları, özellikler) | Hazır tarifler `how-it-works` / `quick-steps` / `care-guide` / `specs` → metni Figma'da gerçek bilgiyle düzelt | 4 | `get_preset_instructions("/usage-guide")` vb. | Recraft V4.1 `utility` + HEX palet |
| Reels kapağı | `thumbnail-generation` iş akışı veya `reel-cover` tarifi | 4 | `get_workflow_instructions("thumbnail-generation")` | |
| Mockup (kutu, poşet, raf) | Photoshop/Figma Mockup Studio; `brand-asset-creation` | 2–4 | `get_workflow_instructions("brand-asset-creation")` | |
| Logo yeniden renklendirme / SVG | `brand-asset-creation` (resmî logoyu birebir korur); `ideogram_vector` vectorize | 0 | aynı | |
| Düşük çözünürlüklü tedarikçi fotoğrafını büyütme | `topaz_image` Standard V2 veya **Text Refine**; generatif Topaz kullanma | 1 | `models_explore get topaz_image` | `bytedance_image_upscale` |

## B. Reklam

| Hedef | Önerilen zincir | Risk | Canlı kontrol | Alternatif |
|---|---|---|---|---|
| Meta/Instagram statik reklam seti | `ads-studio` iş akışı: brand (siteden) → product → 2–3 reklamlık deneme → tam parti (≤20, reklam başına 4 kredi) | 4 [doğrulanacak] | `get_workflow_instructions("ads-studio")` | `ms_image` (DTC Ads; `style_id` zorunlu, `brand_kit_id`), Marketing Studio Posters (katmanlı düzenleme) |
| Var olan video reklamın varyasyonları | `ad-multiplier` (yalnız CTA/hook değişimi en düşük risk) | 2–4 | `get_workflow_instructions("ad-multiplier")`; `models_explore get ad_multiplier` | Genjutsu Objects swap |
| Ürün linkinden video reklam | Marketing Studio Product Link (Click to Ad); çekilen fotoğrafları kendi doğru fotoğraflarınla değiştir | 4 | `get_presets(source:"marketing_studio")`; `models_explore get marketing_studio_v2_video` | UGC: `ugc-video` |
| Pazaryeri görseli | `marketing_studio_2_image` `type:"marketplace"` | 4 | `models_explore get marketing_studio_2_image` | |

## C. Reels / video

| Hedef | Önerilen zincir | Risk | Canlı kontrol | Alternatif |
|---|---|---|---|---|
| Gerçek uygulama çekiminden Reels | (kurgu: Premiere/DaVinci veya Shorts Studio veya `video-editing`/`video-montage`) → video Relight → Color Palette veya DaVinci AI LUT → gerekirse `reframe` 9:16 → `bytedance_video_upscale` | 0–2 | `get_workflow_instructions("video-montage")`; `models_explore get reframe` | Shorts Studio presetleri |
| Gerçek çekim yok, packshot'tan kısa ürün videosu | İlk ve son kare = gerçek packshot: `kling4_0` / `minimax_h3` / `veo3_1_lite` / `seedance_2_5` → yavaş hareket → etiketli kareyi kurguda gerçek packshot ile değiştir | 3 | Her model için `models_explore get` (start/end rolleri) | Hazır video tarifleri: `product-spin`, `half-turn`, `push-in`, `light-sweep`, `label-trace`, `macro-glide` |
| Kamera hareketini önceden kilitlemek | 3D Jutsu previz (`scene_builder_3d_*`) → MP4'ü video modeline referans | 3 | `get_preset_instructions("/3d-jutsu")` | Blender eklentisi |
| Sinematik marka filmi | Cinema Studio 4.0 (`cinematic_studio_video_4_0`, ≤30 sn, ≤50 referans) | 4 | `models_explore get cinematic_studio_video_4_0` | Seedance 2.5 |
| Tek çekimden çok markalı varyasyon | Önce Genjutsu Lite (web, ucuz) → `hf_mult_replace_object` | 4 | `get_preset_instructions("/genjutsu")`; `models_explore get hf_mult_replace_object` | `kling_video_edit` |
| Beğenilen bir kurgu stilini kopyalama | `/katana` (≤5 foto, hakkı bizde olan referans) | 4 | `get_preset_instructions("/katana")` | |
| Videoda küçük bir şeyi silmek (toz, kablo, yabancı marka) | Seedance 2.5 Edit / Draw to Edit (etiketi işaretleme) | 2 | `models_explore get seedance_2_5` | `flux_3_video_edit` |
| Usta hareketini başka karaktere aktarma | `kling3_0_motion_control` veya Genjutsu Motion transfer | 4 | `models_explore get` | |
| Konuşan sözcü / usta | Lipsync Studio; ürün ayrı packshot | 4 | Lipsync modelleri için `models_explore get`; Türkçe test | `narration` iş akışı |

## D. Eğitici / eğlenceli içerik (ürünsüz)

| Hedef | Zincir | Canlı kontrol | Not |
|---|---|---|---|
| "Ya … olsaydı?" Reels | `/content-factory` | `get_preset_instructions("/content-factory")` | 15 sn ≈ 15,75 kredi; Türkçe seste aksan olabilir |
| Ürün kullanımını anlatan animasyon | Explainer (web) veya `faceless-video` | `get_workflow_instructions("faceless-video")` | Ürün stilize çizilir; teknik bilgi elle kontrol |
| UGC tarzı anlatım | `ugc-video` | `get_workflow_instructions("ugc-video")` | Ürün yeniden çizilir |

## E. 3D

| Hedef | Zincir | Canlı kontrol |
|---|---|---|
| Ürünün 3D modeli | 2–4 açıdan gerçek foto → `multi_image_to_3d` veya `tripo_h3_1_multiview_to_3d` → `meshy_v5_remesh` → Blender'da **gerçek etiket dokusu** → kendi kameranla render | `models_explore get multi_image_to_3d` |
| 3D sahne / turntable | Blender eklentisi Scene Builder (ortam) + kendi ürün modeli; ya da 3D Jutsu | `/use-blender`, `/3d-jutsu` |

## F. Ses

| Hedef | Zincir | Not |
|---|---|---|
| Türkçe dış ses | `elevenlabs_v4` veya `text2speech_v2` (elevenlabs/minimax motoru) ile 15 sn test → kurguda ekle | Katalogda Türkçe açıkça listelenmiyor [doğrulanacak] |
| Var olan videoyu dublajlama | `dubbing` | Dil listesi [doğrulanacak] |

## Hazır tariflerin gizli adımları

Hazır ürün tarifleri (`/hero-shot`, `/label-trace`, `/product-spin` vb.) gerçek fotoğrafı doğrudan videoya sokmuyor. Örnek: `/label-trace` talimatı (26 Ekim 2026, `get_preset_instructions`) önce ürünü `nano_banana_pro` ile **yeniden çizerek** tek renk fonlu bir başlangıç karesi hazırlıyor, ardından `seedance_2_0` ile 6 sn, 3:4, 1080p, sessiz video üretiyor. Yani etiket ilk adımda yeniden üretiliyor (risk 4). Bir tarifi plana koymadan önce `get_preset_instructions` ile içindeki model ve adımları oku ve plana yaz.

## Nerede yapılır? (kanal seçimi)

- **Web:** Görsel keşif, tam şablon kütüphanesi, Unlimited/ücretsiz haklar (yalnızca burada), Genjutsu Lite FREE.
- **CLI (Claude Code / Codex):** Tekrarlanan, kayıtlı üretim; `generate cost` ile tahmin.
- **MCP:** Katana, Content Factory, Ad Multiplier, Ads Studio araçları; eklenti kurulum komutları.
- **Masaüstü eklenti:** Gerçek ürün katmanını koruyan kompozit işler (Photoshop, Figma, After Effects, Premiere, DaVinci, Blender).
