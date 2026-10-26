# Proje kuralları — Higgsfield özellik rehberi

Bu repo Higgsfield'ın güncel özelliklerinin envanterini, kullanım rehberini ve bizim iş akışımıza entegrasyon planını tutar. Ürün kataloğu, marka kütüphanesi ve üretim kayıt düzeni ayrı repodadır: `oguzhanguvenkaya/higgsfield_test` (kuralları onun `AGENTS.md` dosyasında). Üretim yapılacaksa o repo da açılmalı ve kuralları uygulanmalı.

## İş planlama
- Kullanıcı Higgsfield ile ne yapmak istediğini anlattığında `.claude/skills/higgsfield-planla` skill'ini kullan: hedefi anla → araç seç → canlı doğrula (MCP/CLI/resmî web) → plan şablonuyla yaz → adım adım yönlendir.
- Kullanıcı `/higgsfield-planla <isteği>` yazarak da başlatabilir.
- Firma kurumsal ve profesyonel içerik üretir; trendler kontrollü kullanılır. Her plan `docs/kurumsal-icerik-rehberi.md` çerçevesine uyar.

## İletişim
- Türkçe, sade dille yaz. Teknik terimi ilk kullanışta somut örnekle açıkla.
- Kaynakta olmayan sayı veya iddia uydurma; emin değilsen `[doğrulanacak]` yaz.
- Kanıt olmadan "bitti/çalışıyor" deme. Kapsamı daraltırsan nedenini söyle.

## Bilgi kaynakları ve güncellik
- `research/<tarih>/` tarihli kanıttır, kalıcı güncel sınır değildir. Higgsfield sık değişiyor; üretimden önce canlı şemayı (CLI `higgsfield` komutları, MCP `models_explore`/`get_presets`) kontrol et.
- Resmî kaynak (higgsfield.ai, help-center, changelog) ile üçüncü taraf bilgisini ayrı tut ve işaretle.
- Yeni araştırma eklerken yeni tarihli klasör aç; eski dosyaları değiştirme, `docs/ozellik-rehberi.md` ve `docs/ozellik-envanteri.md`'yi güncelle.

## Para ve hesap
- Araştırma/rehber işi ücretli üretim başlatmaz. Kullanıcı açıkça üretim isterse `higgsfield_test/AGENTS.md`'deki hesap doğrulaması ve maliyet önizlemesi uygulanır.
- Hesap: `mtskimyaweb@gmail.com`, workspace `bd431bd5-11fd-4b9b-a844-ea55812c6b2b`. MCP bağlantısının başka workspace'e bağlı olabileceğini unutma; bağlanınca doğrula.
- Web'deki Unlimited/ücretsiz haklar MCP, CLI, eklenti, Supercomputer ve API'de geçerli değil (resmî help-center; bazı sayfalar çelişiyor).

## Ürün doğruluğu (en önemli kriter)
- Etiket, logo, ambalaj ve şekil birebir doğru olmalı. Hiçbir Higgsfield aracı bunu garanti etmiyor.
- Tercih sırası: gerçek ürün katmanını koru + ortamı AI ile üret (Photoshop/Figma/AE katmanı, Blender'da gerçek etiket dokusu) → ilk/son kare kilitli video → referanslı tam AI üretimi.
- Her çıktı etiket ve logo açısından insan gözüyle kontrol edilir; videoda tüm klip izlenir.
