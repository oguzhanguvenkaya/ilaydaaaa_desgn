# Canlı Higgsfield MCP kataloğu — salt okunur kontrol (26 Ekim 2026)

Kaynak: Bu oturumdaki yönetilen Higgsfield MCP bağlantısı. **Not:** `higgsfield_test/AGENTS.md`'ye göre bu bağlantı `mtskimyaweb@gmail.com` hesabının workspace'i değil, başka bir özel workspace'e bağlı. Burada yalnızca hesaptan bağımsız katalog/talimat okundu; üretim, preset çalıştırma, Katana oturumu açma YAPILMADI, kredi harcanmadı.

## MCP araç yüzeyinde görülen özellik aileleri (araç adlarından)
- Ads Studio: `ads_studio_create_brand / add_product / quote / generate / list_runs / get_run / cancel_run`
- AI Influencer: `ai_influencer_get_options / list_presets / prepare / generate`, `build_ai_influencer`
- Shorts Studio: `shorts_studio_create / create_preset / list_presets / list_sessions / status`
- 3D: `generate_3d` (görsel → GLB), `scene_builder_3d_*` (3D Jutsu: proje, açı üretimi, video, .blend/.glb alma, Python)
- Katana: `get_katana_config`, `register_katana_result`, `show_katana_result`
- Content Factory / What-If: `register_what_if_result`, `get_presets source:"what_if"`
- Web sitesi / oyun / uygulama: `create_website / deploy_website / publish_website / website_db / website_secrets` (Supercomputer Games ile ilişkili; menüdeki **Playable** ise ayrı bir ürün: Playable Ads + Playable Games, bkz. A-ajan-otomasyon.md)
- Düzenleme: `upscale_image / upscale_video / outpaint_image / reframe / remove_background / motion_control / voice_change / dubbing`
- Analiz: `virality_predictor`, `video_analysis_create`
- TikTok: `tiktok_connect / tiktok_prepare_publish / tiktok_music_trending`
- Projeler ve yayın: `create_project / publish_project / attach_project_asset ...`
- Marketplace uygulamaları: `apps_search / apps_describe / apps_invoke`

## Hazır tarifler (get_preset_instructions, preset belirtmeden)
Ürün odaklı GÖRSEL tarifler: angles, before-after, benefits, bundle, care-guide, color-pop, fabric-wave, feature-zoom, flatlay, gym-bag, hero-shot, how-it-works, ice-capsule, in-hand, inside-pack, kitchen-scene, luxury, main-benefit, minimalist-white, moodboard, myth-fact, new-drop, on-desk, pedestal-shot, powder-cloud, power-angle, product-match, quick-steps, reel-cover, retail-stack, saveable-tip, share-card, shelf-ready, signature-frame, specs, swipe-opener, symmetry, three-reasons, travel-pack, unboxing, usage-guide, vertical-hook, water-splash, weekend-carry, whats-inside.
Ürün odaklı VİDEO tarifler: crane-reveal, detail-scan, floating-roll, half-turn, impact, label-trace (logo ve etiket üzerinde kamera hareketi), light-sweep, liquid-wrap, macro-glide, paint-wave, product-spin, pull-back, push-in, shadow-motion, sunrise-pass, texture-track, topdown-dive, whip-pan.
Ayrıca Cadılar Bayramı temalı portre video tarifleri (vampir, zombi vb.) — bizim için düşük öncelik.

## Paketli iş akışları (get_workflow_instructions)
ad-multiplier (4–30 sn tek videodan çok versiyon; Edit ve Recreate modu), ads-studio (metinli statik reklam kreatifleri, Meta/Instagram), brand-asset-creation (logo yeniden renklendirme/ihracı, marka kiti, mockup, ambalaj, poster, sunum), character-sheet, faceless-video (Explainer/History/Kids/Picture Story/Fairy Tale; ürün demosu için DEĞİL), katana, narration, product-photoshoot, thumbnail-generation, ugc-video (creator review, sadece ürün + dış ses, unboxing, try-on, adım adım tutorial, web sitesi turu), video-editing (Higgsedit: kesme, müzik, animasyonlu yazı, başlık kartları), video-montage (klip birleştirme, müzik, altyazı yakma), website-builder-flow (type: game / website / app).

## Content Factory (/content-factory)
- Şu an tek format: **what-if shorts** — 9:16, yaklaşık 60 sn, "ya şöyle olsaydı…" senaryolu TikTok/Reels/Shorts.
- Her kare kodla çiziliyor (Higgsedit, sandbox); **görsel/video üretim modeli kullanılmıyor**. Tek ücretli çağrı: ElevenLabs v4 dış ses.
- Stil galerisi: talimat metninde 56 hazır stil listeleniyor (elle sayıldı) (ör. Cutaway Lab "temiz 3D ürün kesitleri", Gold Studio "karanlık stüdyo ürün 3D", Blueprint Line, Swiss Grid, Slow Drip "karanlık makro sıvı").
- Çok bölümlü seri (Part 1/2) destekli; aynı karakter, palet, ses korunur.
- Anlatımlı AI sahneli açıklama videoları, çekim düzenleme, sunuculu Reels bu komutun KAPSAMI DEĞİL.

## Katana (/katana)
- Bir **referans videoyu** (beğenilen bir edit/reklam) kendi öznenle sahne sahne yeniden kuruyor (remix); ya da yüklenen çekimi brife göre düzenliyor.
- Yayınlanmış Katana preset'leri var (Higgsfield ve Community kaynakları); her preset bir referans video + yazar promptu.
- Yalnızca analiz, tek başına özne değiştirme, restyle, hareket aktarımı veya reklam varyantı Katana değildir.
- Ücretsiz Katana çalıştırma hakkı (free_generation) kavramı var; miktarı [doğrulanacak].

## Genjutsu (/genjutsu)
- İki model: `hf_mult_motion_control` (sürücü videodaki hareketi referans görsel öznesine aktarma) ve `hf_mult_replace_object` (kaynak videoda nesne/ürün/kıyafet/karakter değiştirme).
- Galeriler: genjutsu (Higgsfield seçkisi), genjutsu-trending, genjutsu-new, **genjutsu-styles** (kendi videonu bir görsel dünyada yeniden çizer, hareket/kamera korunur; 4–30 sn video, en fazla 5 referans görsel, 720p örnek).
- AI Influencer karakter sayfası Genjutsu ile hareketlendirilebiliyor.
- Bu MCP bağlantısında ücretsiz Genjutsu denemesi (use_free_gens) yok; web'deki "FREE" etiketiyle ilişkisi [doğrulanacak].

## Masaüstü eklentileri (MCP kurulum komutları)
Hepsi aynı mimari: **yerel bilgisayardaki** Claude Code / Codex → yerel npm MCP sunucusu → uygulama. Bulut oturumundan (bu oturum dahil) kurulamaz; Claude Desktop "Code → Local" veya yerel terminal gerekir.
| Komut | Paket / sunucu | Bağlantı | Not |
|---|---|---|---|
| /use-after-effects | `fnf-after-effects-mcp`, sunucu `higgsfield-use-after-effects` | OS scripting / ExtendScript | Panel, bulut hesabı gerekmez |
| /use-premiere | `@higgsfield_org/premiere-mcp`, `higgsfield-use-premiere` | İmzalı CEP köprüsü (paketle gelir) | Kurulumdan sonra Premiere yeniden başlatılır; `pr_*` araçları, bundled skill'ler |
| /use-photoshop | `@higgsfield_org/photoshop-mcp`, `higgsfield-use-photoshop` | OS scripting | `ps_*` araçları; macOS'ta Automation izni |
| /use-davinci | `@higgsfield_org/davinci-resolve-mcp`, `higgsfield-use-davinci` | Resmî Resolve Python Scripting API | **DaVinci Resolve Studio (ücretli) gerekir**, Free sürüm bağlanmaz; yalnızca sınırlı Color sayfası araçları (durum, inceleme, CDL, LUT, kaydetme); `davinci-film-colorist` skill'i |
| /use-blender | `fnf-blender-mcp@latest`, `higgsfield-use-blender` | Arka planda ayrı Blender süreci (bpy) | Eklenti gerekmez; açık penceredeki kaydedilmemiş işi okuyamaz; 0.1.0 sürümü eski |
| Figma | Figma Community'de "Higgsfield" eklentisi | Figma içi panel | Bu farklı: MCP değil, Figma'nın içinde panel (bkz. web araştırması) |
Bu masaüstü MCP'leri **ajan (Claude/Codex) üzerinden uygulamayı kumanda etmek** içindir; web sayfasında anlatılan uygulama-içi panel eklentileriyle aynı ürün olup olmadığı [doğrulanacak].
