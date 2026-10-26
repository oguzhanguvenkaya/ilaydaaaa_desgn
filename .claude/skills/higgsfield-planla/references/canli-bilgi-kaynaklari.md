# Canlı bilgi kaynakları: nereden, hangi sırayla?

Öncelik: **1) canlı şema/katalog → 2) Higgsfield'in kendi iş akışı kılavuzu → 3) resmî web belgesi → 4) yerel notlar → 5) üçüncü taraf.** Çelişkide üstteki kazanır; çelişkiyi kullanıcıya söyle.

## 1. Higgsfield MCP (salt okunur araçlar)

Bağlantı: `https://mcp.higgsfield.ai/mcp`. Bağlanınca hangi hesabın ve workspace'in bağlı olduğunu kontrol et. 16 Eylül'de yönetilen bağlantının `mtskimyaweb` workspace'ine değil, başka bir workspace'e bağlı olduğu görülmüştü.

| Araç | Ne verir | Not |
|---|---|---|
| `models_explore(action:"list", type)` | Tüm modeller: parametreler, süre aralığı, oranlar, girdi rolleri, `supports_unlim` | `type`: image / video / audio / 3d |
| `models_explore(action:"get", model_id)` | Tek modelin güncel kısıtları ve "Unlim configs" | Her plan adımında çağır |
| `models_explore(action:"recommend", query)` | Hedefe göre model önerisi | Sorguya girdi bağlamını yaz ("reference image, product, 9:16, 10s") |
| `get_workflow_instructions()` | Paketli iş akışlarının listesi | Argümansız çağır |
| `get_workflow_instructions(workflow)` | Resmî iş akışı kılavuzu (SKILL.md): kilitli model, intake soruları, sınırlar | Aşağıdaki tabloya bak |
| `get_workflow_bundle_file(workflow, path)` | Kılavuzun alt belgeleri (ör. `references/product-shot.md`, `references/typography.md`) | Yalnızca gerekenleri oku |
| `get_preset_instructions()` | Hazır tarifler (hero-shot, label-trace, product-spin…) ve komutlar | Argümansız: katalog |
| `get_preset_instructions(preset)` | Bir tarifin veya komutun talimatı (`/content-factory`, `/katana`, `/genjutsu`, `/use-photoshop`…) | Okumak oturum açmaz |
| `get_presets(source, category, query, preset_id)` | Galeriler: viral, marketing_studio (product-shot, motion), genjutsu (genjutsu, -trending, -new, -styles), soul, katana, what_if | Widget açar; **`execute_preset` çağırma** |
| `apps_search(query)` / `apps_describe` | Higgsfield Marketplace uygulamaları | Salt okunur |
| `balance`, `show_plans_and_credits` | Bakiye ve plan | Kullanıcı isterse |

**Planlamada çağrılmayacaklar:** `generate_*`, `execute_preset`, `get_katana_config` (oturum açar), `ads_studio_generate`, `ai_influencer_generate`, `shorts_studio_create`, `publish_*`, `deploy_*`, `media_upload*` (kullanıcı onayı olmadan).

### Resmî iş akışları (26 Ekim 2026 listesi)

| İş akışı | Ne zaman | Önemli not |
|---|---|---|
| `product-photoshoot` | Ürün packshot, lifestyle, elde ürün, banner, carousel, statik reklam paketi, restyle | Model **nano_banana_pro 2k** olarak kilitli; 10 mod; varsayılan 3 varyant, 1:1 |
| `ads-studio` | Metinli statik reklam kreatifleri (Meta / Instagram), marka veya ürün linkinden | `ads_studio_*` araçları |
| `ad-multiplier` | 4–30 sn tek videodan çok versiyon (Edit / Recreate) | |
| `ugc-video` | Creator review, yalnızca ürün + dış ses, unboxing, tutorial, web sitesi turu | |
| `video-editing` | Higgsedit ile kesme, müzik, animasyonlu yazı, başlık kartı | |
| `video-montage` | Klipleri birleştirme, müzik, altyazı yakma | |
| `brand-asset-creation` | Logo yeniden renklendirme ve ihracı, marka kiti, mockup, ambalaj, poster, sunum | Resmî logoyu birebir korur |
| `thumbnail-generation` | YouTube / Instagram kapağı | |
| `faceless-video` | Anlatımlı animasyon (Explainer, History, Kids…) | Ürün demosu için değil |
| `katana` | Referans kurguyu kendi öznenle yeniden kurma | |
| `narration` | Sabit pencereye oturan dış ses, sunucu ekleme | |
| `character-sheet` | Tutarlı karakter sayfası | |
| `website-builder-flow` | Web sitesi, uygulama, tarayıcı oyunu | |

## 2. Higgsfield CLI (yerel bilgisayar)

Kurulum ve giriş: `docs/yerel-kurulum.md`. 16 Eylül'de bu projede çalıştığı kayıtlı bilgi komutları:

```bash
higgsfield account status
higgsfield workspace list
higgsfield model list --json
higgsfield model get <model_id> --json          # ör. seedance_2_5, nano_banana_pro, hf_mult_replace_object
higgsfield workflow list --json
higgsfield workflow get <workflow_id> --json    # ör. marketing_studio_2_image, cinematic_studio_video_4_0
higgsfield preset list marketing-studio-v2 --type product_shots --json
higgsfield generate cost <model_id> ...         # gerçek ayarlarla kredi tahmini; yerel medya verilirse yükleme yapabilir
```

Komut adları sürüme göre değişebilir; emin değilsen `higgsfield --help` ve `higgsfield <komut> --help` ile kontrol et. Help-center: Higgsfield kod ajanları için CLI + Skills yolunu öneriyor (`npx skills add higgsfield-ai/skills`).

## 3. Resmî web kaynakları

| Kaynak | Adres | Ne için |
|---|---|---|
| Help center | `https://higgsfield.ai/creator-hub/help-center/...` | Kullanım adımları, sınırlar, kredi kuralları |
| Changelog | `https://higgsfield.ai/creator-hub/changelog` | Yeni çıkanlar, sürüm değişiklikleri |
| Blog | `https://higgsfield.ai/blog/...` | Tanıtım, örnek fiyat tabloları (tarihli) |
| Ürün sayfaları | `https://higgsfield.ai/<araç>` | Bir kısmı JavaScript ile yükleniyor; metni okunamayabilir |
| Eklentiler | `https://higgsfield.ai/plugins/<ad>` (photoshop, premiere-pro, after-effects, davinci, figma, blender) | Kurulum ve sürüm şartı |
| MCP ve ChatGPT | `https://higgsfield.ai/mcp` | Bağlantı |
| API | `https://docs.higgsfield.ai` | Geliştirici belgesi |

Arama önerisi: `site:higgsfield.ai <araç adı>` ve `site:higgsfield.ai/creator-hub <araç adı>`. Blog fiyatlarını her zaman tarihiyle ver; kesin fiyat Generate düğmesinde veya `generate cost` ile görülür.

## 4. Yerel notlar (bu repo)

- `docs/ozellik-rehberi.md`, `docs/ozellik-envanteri.md`
- `bilgi/canli-katalog-<tarih>/`
- `research/<tarih>/A–F`

Bunlar tarihli kanıttır. 14 günden eskiyse ilgili aracı canlı kontrol et.

## Bilinen tuzaklar

- **Unlimited / ücretsiz haklar** resmî help-center'a göre yalnızca web'de geçerli; MCP, CLI, eklenti, Canvas, Supercomputer ve API her zaman kredi düşer. Bazı sayfalar çelişiyor.
- **Marketing Studio:** MCP/CLI'deki preset seti webdekinden küçük (help-center).
- **Marka/logo IP filtresi:** Logolu referans engellenebilir; kendi girdinde "I own the rights" seçeneği çıkabilir.
- **Eski CLI/skill sürümlerinde referans görsel iletilmeme sorunu** (help-center): Referansın gerçekten gittiğini kontrol et.
- **Türkçe ses:** Katalogdaki Qwen ve Inworld ses listelerinde Türkçe yok; ElevenLabs'ta dil parametresi yok. Türkçe seslendirme için kısa test planla.
