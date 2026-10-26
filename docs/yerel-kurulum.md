# Başka bir bilgisayarda bu repoyu açma (yerel Claude Code)

Bu repo bulut oturumunda hazırlandı. Bulut oturumu senin bilgisayarındaki dosyaları göremez. Ürün fotoğrafları, Photoshop/Premiere/DaVinci/Blender bağlantıları ve Higgsfield CLI için çalışmayı **yerel** bir Claude Code oturumunda sürdürmek gerekir.

Aşağıdaki adımlar macOS ve Windows için. Komutlar terminalde (Mac: Terminal, Windows: PowerShell) çalıştırılır.

## 1. Gerekli programlar

| Program | Neden | Kontrol komutu |
|---|---|---|
| Git | Repoyu indirmek ve güncellemek | `git --version` |
| Node.js (LTS) + npm | Higgsfield CLI ve eklenti MCP paketleri npm ile kuruluyor | `node -v` ve `npm -v` |
| Claude Code | Yerel ajan | `claude --version` |
| (İsteğe bağlı) GitHub CLI | GitHub girişini kolaylaştırır | `gh --version` |

Claude Code kurulumu için güncel resmî yol: https://docs.claude.com/en/docs/claude-code (kurulum komutu zamanla değişebilir, oradan bak). Alternatif: **Claude Desktop** uygulamasını kurup içinde **Code → Local** modunu kullanmak.

## 2. Repoyu indir

```bash
# GitHub'a giriş (bir kez)
gh auth login            # veya GitHub Desktop ile giriş yap

# Çalışma klasörüne geç ve indir
cd ~/Projeler            # istediğin klasör
git clone https://github.com/oguzhanguvenkaya/ilaydaaaa_desgn.git
git clone https://github.com/oguzhanguvenkaya/higgsfield_test.git   # marka/ürün kataloğu ve üretim kayıt düzeni
```

**Önemli:** `higgsfield_test` reposunda ürün fotoğraf klasörleri (`MG-*`), `inputs/` ve `library/` Git'e **yüklenmiyor**. Bunları eski bilgisayardan (USB, Drive vb.) aynı klasör yapısıyla kopyalaman gerekir. Aksi hâlde katalogdaki fotoğraf yolları boş kalır.

## 3. Claude Code'u bu klasörde başlat

```bash
cd ~/Projeler/ilaydaaaa_desgn
claude
```

- Claude, klasördeki `CLAUDE.md` dosyasını otomatik okur; proje kuralları orada.
- İki repoyu birlikte görmesi için üst klasörde (`~/Projeler`) başlatabilir ya da oturumda `/add-dir ../higgsfield_test` kullanabilirsin.
- Telefondan veya Claude uygulamasından takip etmek istersen: aynı klasörde `claude remote-control` çalıştır; oturum Claude Code uygulamasında görünür, ama dosyalar ve komutlar yine bu bilgisayarda çalışır.

## 4. Higgsfield CLI (ana üretim yolu)

```bash
npm i -g @higgsfield/cli
higgsfield auth login                 # mtskimyaweb@gmail.com hesabıyla
npx skills add higgsfield-ai/skills   # resmî yardımcı beceriler
higgsfield account status             # hesabın doğru olduğunu doğrula
higgsfield workspace list             # seçili workspace'i doğrula
```

`higgsfield_test/AGENTS.md`'deki kural: ücretli üretimden önce hesap ve workspace doğrulanır (`bd431bd5-11fd-4b9b-a844-ea55812c6b2b`).

## 5. (İsteğe bağlı) Higgsfield MCP bağlantısı

Bazı iş akışları yalnızca MCP üzerinden sunuluyor: Katana, Content Factory, Ad Multiplier, masaüstü eklenti kurulum komutları.

- Claude Desktop / claude.ai: Settings → Connectors → Add custom connector → ad `Higgsfield`, URL `https://mcp.higgsfield.ai/mcp` → Connect → hesabınla yetki ver.
- Claude Code (terminal): `claude mcp add --transport http higgsfield https://mcp.higgsfield.ai/mcp` [doğrulanacak: komut sözdizimi Claude Code sürümüne göre değişebilir; `claude mcp --help` ile kontrol et].
- Bağlandıktan sonra hangi workspace'e bağlandığını kontrol et. 16 Eylül'de yönetilen bağlantının farklı bir workspace'e (`0a7575f2-...`) bağlandığı kaydedilmişti.
- MCP her üretimde kredi düşer; web'deki Unlimited burada geçerli değil. Aktif ücretli abonelik gerekiyor.

## 6. (İsteğe bağlı) Masaüstü uygulama eklentileri

Her eklentinin **iki ayrı biçimi** var; ikisini karıştırma:

| | A) Uygulama içi panel (sen tıklarsın) | B) Ajan bağlantısı / MCP (Claude kumanda eder) |
|---|---|---|
| Kurulum | higgsfield.ai/plugins/... sayfasından indir, kur | Yerel Claude Code'da Higgsfield MCP bağlıyken: `higgsfield mcp, /use-photoshop` yaz; Claude npm paketini kurar ve kaydeder |
| Nerede çalışır | Photoshop/Premiere/AE/DaVinci/Blender/Figma içinde panel | Claude Code ↔ yerel MCP sunucusu ↔ uygulama |
| Bulut oturumundan kurulur mu? | Hayır | Hayır (yalnızca yerel) |

Ayrıntılar ve sürüm gereksinimleri: [eklentiler rehberi](ozellik-rehberi.md#eklentiler).

B) kurulum komutları (Higgsfield MCP talimatlarından):

| Uygulama | Komut | Paket | Not |
|---|---|---|---|
| After Effects | `/use-after-effects` | `fnf-after-effects-mcp` | |
| Premiere Pro | `/use-premiere` | `@higgsfield_org/premiere-mcp` | Kurulumdan sonra Premiere'i yeniden başlat |
| Photoshop | `/use-photoshop` | `@higgsfield_org/photoshop-mcp` | macOS'ta Automation izni isteyebilir |
| DaVinci Resolve | `/use-davinci` | `@higgsfield_org/davinci-resolve-mcp` | **Resolve Studio (ücretli) gerekir**; ücretsiz sürüm bağlanmaz |
| Blender | `/use-blender` | `fnf-blender-mcp@latest` | Eklenti gerekmez; arka planda ayrı Blender süreci açar |

## 7. Repoyu güncel tutma

```bash
git pull                      # başka yerde yapılan değişiklikleri al
git add -A && git commit -m "açıklama" && git push   # kendi değişikliklerini gönder
```

Ya da Claude'a "değişiklikleri commit edip pushla" demen yeterli.
