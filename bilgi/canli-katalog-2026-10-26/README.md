# Canlı model kataloğu özeti — 26 Ekim 2026

Kaynak: Higgsfield MCP `models_explore(action:"list")`, salt okunur. Bu oturumdaki MCP bağlantısı `mtskimyaweb` hesabının workspace'ine değil, başka bir workspace'e bağlıydı. Model kataloğu hesaba göre farklı olabilir [doğrulanacak]; plan yaparken her zaman canlı kontrol et (bkz. [canlı bilgi kaynakları](../../.claude/skills/higgsfield-planla/references/canli-bilgi-kaynaklari.md)).

- `modeller-video.json`: 59 video modelinin ham kaydı (parametreler, süre, oran, girdi rolleri).
- Görsel, ses ve 3D katalogları aşağıda özetlendi; ham kayıtları kaydedilmedi. Yerelde `higgsfield model list --json` ile tazelenebilir.

"Girdi rolleri" modele hangi tür dosyanın hangi görevle verilebileceğini gösterir: `start_image` ilk kare, `end_image` son kare, `image_references` referans görsel, `video_references` referans video, `audio_references` ses, `mask` maske. **U** = katalogda `supports_unlim` (web'deki Unlimited / ücretsiz deneme kapsamına girebilir).

## Görsel modelleri (öne çıkanlar)

| id | Ad | Çözünürlük / kalite | Önemli parametreler | Girdi rolleri | U |
|---|---|---|---|---|---|
| `nano_banana_pro` | Nano Banana Pro | 1k / 2k / 4k (varsayılan 2k) | — | image_references | U |
| `nano_banana_2_1` | Nano Banana 2.1 | 1k / 2k / 4k | `is_inpaint`, `thinking_level`, `seed`, web/görsel arama; oran 8:1'e kadar | image_references, mask, video_references | |
| `nano_banana_2` | Nano Banana 2 | 1k / 2k / 4k | `is_inpaint` | image_references, mask | U |
| `gpt_image_2_5` | GPT Image 2.5 | 1k / 2k / 4k; kalite low → max | `variant`: flare / sunburst; `background`: **transparent** seçeneği | image_references | |
| `gpt_image_2` | GPT Image 2 | 1k / 2k / 4k; low / medium / high | — | image | U |
| `openai_hazel` | OpenAI Hazel | low / medium / high | Katalog açıklaması: "best text rendering", logolar | image_references | |
| `seedream_v5_pro` | Seedream 5.0 Pro | 1k / 1.5k / **en fazla 2k** | `remove_bg`, `is_inpaint` | image_references | U |
| `flux_3_image` | FLUX 3 Image | 768 → 4k | `batch_size` ≤4; ≤10 referans | image_references | |
| `flux_2` | FLUX.2 | 1k / 2k | `variant`: pro / flex / max | image_references | U |
| `flux_2_pro_outpaint` | FLUX.2 Pro Outpaint | — | Kenar başına piksel genişletme veya kırpma | image_references | |
| `recraft_v4_1` | Recraft V4.1 | 1k / 2k | `model_type`: standard / vector / **utility** (ürün çekimi, mockup) / utility_vector; `colors` ≤10 HEX; `background_color` | — (referans yok) | |
| `ideogram_4_5` | Ideogram 4.5 | 1k / 2k | Tipografi; `seed`; maske | image_references, mask | |
| `ideogram_vector` | Ideogram Vector | — | SVG üretme veya **mevcut görseli vektörleştirme** | image_references | |
| `marketing_studio_2_image` | Marketing Studio Product Shot | — | `type`: product_shots / product_shots_people / poster / ads / marketplace; `brand_kit_id`; `preset_id` veya `style_id` | input_images, product_image, character_photo, model_image | |
| `ms_image` | DTC Ads | 1k / 2k / 4k | `style_id` **zorunlu**; `brand_kit_id`; `product_ids` ≤4; `batch_size` ≤20 | image (≤14) | |
| `cinematic_studio_image` | Cinematic Studio Image | 1k / 2k / 4k | Kamera gövdesi, lens, odak **zorunlu**; diyafram | image_references | |
| `cinematic_studio_2_5` | Cinema Studio Image 2.5 | 1k / 2k / 4k | Sinematik kare | image | |
| `soul_2` | Soul 2.0 | 1.5k / 2k | `style_id` (referans görselle birlikte kullanılamaz), `soul_id` | image (≤1) | U |
| `grok_image_2_0` | Grok Image 2.0 | 1k / 2k | low / medium | image_references | |
| `z_image` | Z Image | — | Hızlı, ucuz, stilize | — | |
| `bytedance_image_upscale` | ByteDance Image Upscale | 2k / 4k | `remove_bg` | image_references | |
| `topaz_image` | Topaz (standart) | Hedef piksel | `variant`: Standard V2 / Low Resolution V2 / CGI / High Fidelity V2 / **Text Refine** | image_references | |
| `topaz_image_generative` | Topaz (generatif) | Hedef piksel | Redefine / Recovery; `creativity` 1–6. **Etiketli görselde kullanma** | image_references | |
| `image_decompose` | Image Decompose | — | Görseli katmanlara ayırır (granular / standard) | image_references | |
| `image_background_remover` | Arka plan silme | — | — | image_references | |

## Video modelleri (öne çıkanlar)

"Ses param." sütunu yalnızca katalogda bir ses açma/kapama parametresi olup olmadığını gösterir. Parametre yoksa model yine de sesli üretebilir; bu ayrıca doğrulanmalı.

| id | Ad | Süre (sn) | Çözünürlük | Ses param. | Girdi rolleri | U |
|---|---|---|---|---|---|---|
| `seedance_2_5` | Seedance 2.5 | 4–30 | 480p / 720p / 1080p | var | start, end, image_ref, video_ref, audio_ref | |
| `cinematic_studio_video_4_0` | Cinema Studio 4.0 | 4–30 | 480p–1080p | var | aynı | |
| `kling4_0` | Kling 4.0 | 3–30 | 720p / 1080p | — | start, end, image_ref, video_ref | |
| `kling3_0` | Kling 3.0 | 3–15 | — | var | start, end | U |
| `kling3_0_motion_control` | Kling 3.0 Motion Control | — | — | — | image_ref, video_ref | U |
| `kling_video_edit` | Kling 3.0 Omni Edit | — | — | — | image_ref, video_ref | |
| `minimax_h3` | MiniMax H3 | 4–15 | 2K | — | start, end, image_ref, video_ref, audio_ref | |
| `minimax_hailuo` | Hailuo | 6 / 10 | 512 / 768 / 1080 | — | start, end | |
| `flux_3_video` | FLUX 3 Video | 5–20 | 720p / 1080p / 2k / 4k | var | start, end, image_ref, video_ref | |
| `gemini_omni_flash_1_1` | Gemini Omni Flash 1.1 | 3–10 | 360p → 4k | — | start, end, image_ref, video_ref | |
| `veo3_1` | Veo 3.1 | 4 / 6 / 8 | kalite basic / high / ultra | — | start | |
| `veo3_1_lite` | Veo 3.1 Lite | 4 / 6 / 8 | — | var | start, end | |
| `wan3_0` / `wan3_0_prime` | Wan 3.0 / Prime | ≤30 | 480p–1080p | var | start, end, image_ref, video_ref, audio_ref | |
| `grok_video_v15` / `_lite` | Grok Imagine 1.5 / Lite | 2–15 / 1–15 | 480p–1080p | — | start (+ image_ref, audio_ref) | |
| `happy_horse_video` | Happy Horse | 3–15 | 720p / 1080p | — | start | |
| `hf_mult_replace_object` | Genjutsu (nesne değişimi) | — | 480p–1080p | — | image_ref, video_ref | |
| `hf_mult_motion_control` | Genjutsu (hareket aktarımı) | — | 480p–1080p | — | image_ref, video_ref | |
| `hf_mult_*_flash` | Genjutsu Lite | — | 480p/720p–1080p | — | image_ref, video_ref | |
| `ad_multiplier` / `_v2` | Ad Multiplier / Recreate | 4–30 | 480p–1080p | var | — | |
| `marketing_studio_v2_video` | Marketing Studio Video | 4–30 | 480p–1080p | var | avatars, character_photo, input_images, location_photo, product_photo | |
| `draw_to_video` | Draw To Video | — | 480p–1080p | var | image_ref, ref_image, video | |
| `reframe` | Reframe | — | 480p–1080p | — | start, image_ref, video_ref | |
| `bytedance_video_upscale` | ByteDance Video Upscale | — | 1080p / 2k / 4k | — | video_ref | |
| `topaz_video` | Topaz Video | — | 1080p / 2160p | — | video_ref | |
| `sam_3_video` | Remove Background (video) | — | — | — | video_ref | |
| `fps_boost`, `video_deflicker`, `depth_anything_video` | Kare hızı artırma, titreşim giderme, derinlik haritası | — | — | — | — | |
| `dubbing`, `voice_change`, `sync_so` | Dublaj, ses değiştirme, Sync Lipsync 3 | — | — | — | input_video (+ input_audio) | |

Seedance 2.0 ve 2.0 Mini katalogda **U** işaretli; Seedance 2.5 değil.

## Ses modelleri

| id | Ad | Dil / ses notu |
|---|---|---|
| `elevenlabs_v4` / `_turbo` | Eleven v4 / Turbo | Diyalog, ≤10 ses (Turbo: 1). Katalogda dil parametresi yok; **Türkçe kalite [doğrulanacak]** |
| `text2speech_v2` | Text to Speech V2 | Motor: elevenlabs / minimax / seed_speech / vibe_voice / cozy_voice. U |
| `seed_audio` | Seed Audio 1.0 | Hız, ses yüksekliği, perde ayarı. U |
| `qwen_audio_tts` | Qwen Audio 3.0 TTS | Dil listesi: zh, en, fr, de, ja, ko, ru, pt, th, id, vi, it, ms. **Türkçe yok** |
| `inworld_text_to_speech` | Inworld TTS | Yalnızca oyun akışı; ses listesinde **Türkçe yok** |
| `sonilo_music`, `mirelo_text_to_audio` | Müzik / ses efekti | Yalnızca oyun akışı |

## 3D modelleri (ürün geometrisi için)

| id | Ne yapar | Bizim için not |
|---|---|---|
| `multi_image_to_3d` / `meshy_multi_image_to_3d` | 1–4 açıdan fotoğraftan GLB | Gerçek ürün fotoğraflarından şişe/kutu geometrisi. Etiket dokusu AI'dan gelir; gerçek etiketi Blender'da kendin kapla |
| `tripo_h3_1_multiview_to_3d` | 2–4 sıralı görüntüden GLB | Alternatif |
| `meshy_v7_image_to_3d`, `tripo_h3_1_image_to_3d`, `hunyuan3d_v3_image_to_3d`, `sam_3_3d` | Tek görselden GLB | Hızlı taslak |
| `meshy_v5_retexture` | Var olan modeli yeniden dokular (`enable_original_uv`) | Etiket için kullanma; gerçek baskı dosyası daha doğru |
| `meshy_v5_remesh` | Topoloji ve poligon düzenleme | Blender'a hazırlık |
