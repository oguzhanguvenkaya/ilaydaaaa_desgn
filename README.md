# Higgsfield özellik rehberi ve iş akışı entegrasyonu

Higgsfield'ın Ekim 2026 itibarıyla menüde görünen bütün özelliklerinin envanteri, kullanım rehberi ve oto bakım ürünleri distribütörü olarak iş akışımıza nasıl gireceği.

## Nereden başlamalı?

0. **Planlayıcı (yeni):** Bu repoyu açtığın Claude Code oturumunda yapmak istediğin işi anlat ya da `/higgsfield-planla <isteğin>` yaz. Claude hangi Higgsfield araçlarının hangi sırayla, nerede ve hangi ayarlarla kullanılacağını, kredi tahmini ve etiket riskiyle planlar ve seni adım adım yönlendirir. Bilgiyi canlı Higgsfield MCP/CLI kataloğundan ve resmî belgelerden günceller; plan aşamasında kredi harcamaz. Ayrıntı: [skill](.claude/skills/higgsfield-planla/SKILL.md), [örnek plan](.claude/skills/higgsfield-planla/references/ornek-plan.md).
1. [Özellik rehberi](docs/ozellik-rehberi.md): kısa sonuç, ürün etiketi güvenliğine göre araç sıralaması, içerik türüne göre iş akışları, test planı, açık sorular.
2. [Özellik envanteri](docs/ozellik-envanteri.md): menüdeki her özellik ve model için tek satır; eski rehberde var mı, etiket riski, öncelik, detay linki.
3. [Başka bilgisayarda açma / yerel kurulum](docs/yerel-kurulum.md)

Hiçbir öneri bizim ürünlerimizle test edilmedi. Kaynakta bulunamayan veya kaynakların çeliştiği yerler `[doğrulanacak]` diye işaretli. Araştırma sırasında ücretli üretim yapılmadı.

## İçerik

- [Başka bilgisayarda açma / yerel kurulum](docs/yerel-kurulum.md)
- [Proje kuralları (Claude için)](CLAUDE.md)
- Ham araştırma, 26 Ekim 2026 (kaynaklı, `[doğrulanacak]` işaretli):
  - [A: Content Factory, Playable, Genjutsu, Katana, AI Influencer, ChatGPT eklentisi, MCP, API, Supercomputer](research/2026-10-26/A-ajan-otomasyon.md)
  - [B: Cinema Studio, Ads Studio, Ad Multiplier, Effects, Marketing Studio, Click to Ad, Shorts/Faceless Studio, Explainer, Create Video](research/2026-10-26/B-studyolar-reklam.md)
  - [C: After Effects, Premiere Pro, Photoshop, DaVinci Resolve, Figma, Blender eklentileri ve Canvas](research/2026-10-26/C-eklentiler-canvas.md)
  - [D: Image menüsü özellikleri ve görsel modeller](research/2026-10-26/D-gorsel.md)
  - [E: Video menüsü özellikleri ve video modelleri](research/2026-10-26/E-video.md)
  - [Canlı model kataloğu özeti, 26 Ekim 2026](bilgi/canli-katalog-2026-10-26/README.md): görsel, video, ses ve 3D modellerinin güncel parametreleri
  - [F: Canlı Higgsfield MCP kataloğu (hazır tarifler, iş akışları, eklenti kurulum komutları)](research/2026-10-26/F-canli-mcp-katalog.md)

## İlgili repo

Ürün kataloğu, marka kütüphanesi ve üretim kayıt düzeni: `oguzhanguvenkaya/higgsfield_test`. Oradaki eski araştırma (`docs/higgsfield-arastirma-2026-09-16.md`) ürün görseli odaklıdır ve bu repodaki özelliklerin çoğunu kapsamaz.
