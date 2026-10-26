# Plan şablonu

Planı bu yapıda yaz. Gereksiz bölümü sil, ama "Etiket riski", "Kredi" ve "Kaynaklar" hiçbir adımda boş kalmasın (bilinmiyorsa `[doğrulanacak]`).

```markdown
## Plan: <kısa başlık>

**Hedef:** <kullanıcının istediği, kendi cümlesiyle>
**Teslim:** <format, oran, süre/adet, kanal>
**Kısa yol:** <1–2 cümle: hangi araçlar, neden bu sıra>
**Bilgi tarihi:** <canlı kontrol tarihi; hangi kaynaklara bakıldı>

### Hazırlık (ücretsiz)
- [ ] <gerekli gerçek dosyalar: ürün fotoğrafı (hangi açı), logo, video>
- [ ] <hesap/workspace doğrulaması, eklenti kurulumu>

### Adımlar
| # | Ne yapılacak | Araç / model | Nerede | Girdi → çıktı | Ayarlar | Etiket riski ve kontrol | Kredi (kaynak) |
|---|---|---|---|---|---|---|---|
| 1 | | | Web: … / CLI: `…` / MCP: `…` / Eklenti: … | | | | |

### Adım ayrıntıları
**1. <adım adı>**
- Nasıl: <tıklama yolu veya komut>
- Neden bu araç: <1 cümle; alternatife göre farkı>
- Dikkat: <bilinen sınır, tuzak>

### Bütçe
- Ucuz deneme (önce): <adım, ayar, ~kredi>
- Tam üretim: <~kredi aralığı>
- Kesin tutar: Generate düğmesi / `higgsfield generate cost`

### Alternatif yol
- <daha güvenli / daha ucuz / daha hızlı seçenek ve farkı>

### Riskler ve açık noktalar
- <etiket, IP filtresi, Türkçe ses, plan kısıtı…>
- [doğrulanacak] <…>

### Kaynaklar
- <canlı katalog çağrısı / iş akışı adı / help-center URL / blog URL + tarih>

**Karar:** Plan uygun mu? <1. adımdan başlayalım mı / şu soruyu yanıtlar mısın>
```
