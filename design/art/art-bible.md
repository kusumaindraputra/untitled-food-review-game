# Art Bible — Cicip & Catat

*Status: In Progress*
*Last Updated: 2026-06-26*

---

## 1. Visual Identity Statement

**Arah Visual: "Feed Seseorang yang Mencoba Bertahan Hidup dari Kontennya"**

### One-Line Visual Rule

> Setiap elemen UI dan environment harus terasa seperti feed sosial media yang dikelola sendiri oleh seorang kreator independen — personal, sedikit DIY, nyata — bukan produk perusahaan tech, dan bukan buku catatan fisik.

### Supporting Principles

**Prinsip 1 — Estetika Feed, Bukan Estetika Kertas**
Semua layout UI mengacu pada struktur visual sosial media — grid foto, story format, engagement counter — bukan kertas, tinta, atau artefak fisik.

*Design test*: Kalau elemen UI bisa "dicetak atau difoto sebagai benda fisik" → redesign. Harus hanya bisa eksis di layar: glow subtle, notification dot, angka berubah real-time.

*Pillar yang dilayani*: Pillar 2 — Rutinitas yang Menyerap. Feed sosial media adalah antarmuka paling absorbing yang pernah didesain manusia — player sudah punya muscle memory terhadap bentuk ini. Memakai pola itu membuat ritual bulanan terasa alami dan meditative, bukan asing.

---

**Prinsip 2 — Stamp Digital, Bukan Stempel Fisik**
"Stamp" tetap digunakan sebagai visual, tapi selalu berbentuk digital overlay — badge terverifikasi, emoji yang ditumpuk di atas foto makanan, label "REVIEWED", "VIRAL", atau "BANGKRUT" yang muncul sebagai overlay transparan di atas asset foto.

*Design test*: Kalau stamp yang kamu desain bisa terlihat masuk akal sebagai rubber stamp di atas kertas → ganti bentuk, warna, atau treatment-nya. Stamp yang benar harus terasa seperti overlay dari aplikasi: rounded corner, drop shadow tipis, atau fill solid dengan transparansi — seperti reaction emoji atau verified badge.

*Pillar yang dilayani*: Pillar 3 — Reviewer Bukan Dewa. Stamp digital adalah tanda kekuatan yang diberikan platform, bukan otoritas pribadi. "VIRAL" badge bukan penghargaan — itu notifikasi dari sistem yang tidak kamu kendalikan sepenuhnya.

---

**Prinsip 3 — Foto Makanan sebagai Mata Uang Visual**
Food photography adalah bahasa visual utama game ini. Setiap restoran direpresentasikan pertama-tama sebagai foto makanannya — kualitas foto mencerminkan kelas restoran (foto amatir vs foto profesional).

*Design test*: Kalau bisa memahami "karakter" sebuah restoran hanya dari thumbnail foto makanannya tanpa membaca nama atau deskripsi — desain foto itu berhasil. Kalau foto bisa diganti dengan foto restoran lain tanpa kehilangan identitas → redesign.

*Pillar yang dilayani*: Pillar 4 — Restoran Punya Jiwa. Foto adalah cara tercepat untuk menyampaikan bahwa tempat ini punya kepribadian sebelum player membaca satu kata pun.

### Elemen Visual yang Dihapus

Referensi berikut harus dihindari di semua keputusan visual ke depan:
- Metafora "buku catatan", "kertas lama", "halaman", "coretan tangan"
- "foto polaroid" — diganti dengan format story/feed/grid
- "UI sebagai artefak fisik" — diganti dengan "UI sebagai antarmuka feed"
- Palet warm off-white/cokelat seperti kertas — dikaji ulang di Section 4

---

## 2. Mood & Atmosphere

*Section ini melayani Visual Identity Statement: emosi per state diekspresikan melalui variasi dalam satu bahasa visual feed yang sama — bukan perpindahan ke style yang berbeda.*

**Prinsip penggerak utama:** Saturasi adalah lever utama perubahan state.
- Kepercayaan diri / awal bulan = saturasi tinggi, foto makanan dominan
- Tekanan keuangan / akhir bulan = saturasi turun, feed memudar
- Krisis / game over = near-monochrome, satu accent warna tersisa

---

### 2.1 Planning Phase

**Emosi target:** Quiet strategic tension — perasaan menatap kalender dan rekening di awal bulan sebelum keputusan apapun dibuat.

**Karakter cahaya:** Biru-putih layar HP di jam 7 pagi. Cool-dominant palette, low warmth, high clarity. *(Technical: dominant hue cool-neutral, saturation pada foto restoran 100%, saturation pada UI non-foto 30–40%)*

**Deskriptor atmosfer:** "glow layar sebelum hari dimulai" / "spreadsheet yang belum salah" / "feed scroll saat sarapan, masih dalam kendali" / "ketenangan sebelum keputusan pertama"

**Energy level:** Measured. Deliberate.

**Elemen kunci:** Restaurant grid — foto makanan full-saturasi di atas background muted cool-neutral. Kontras antara foto vivid dan surrounding muted membuat restoran terasa seperti kesempatan, bukan kewajiban.

---

### 2.2 Visiting Phase

**Emosi target:** Focused evaluation — perhatian yang menyempit saat duduk di depan hidangan dan memutuskan apa yang sebenarnya kamu pikirkan. Bukan stres — presisi.

**Karakter cahaya:** Warm tapi terarah dan terkontrol. *(Technical: warm color temperature, food subject tile at 100% brightness, background restaurant tiles at 60–70% brightness, checklist UI elements warm-desaturated)*

**Deskriptor atmosfer:** "overhead shot, no filter, just assessment" / "hening membentuk opini" / "cahaya warm yang mengekspos kekurangan secara merata" / "still frame sebelum caption ditulis"

**Energy level:** Contemplative. Lebih lambat dari Planning.

**Elemen kunci:** Foto makanan ditampilkan besar, center-frame, unfiltered. Satu-satunya phase di mana foto makanan mengisi full panel. Checklist items muncul di sekitarnya, tidak di atasnya.

---

### 2.3 Publishing Phase

**Emosi target:** The irreversible click — anxiety-relief spesifik saat menekan "Post". Kekuatan yang digunakan dan tidak bisa ditarik kembali.

**Karakter cahaya:** Screen-bright, sedikit overexposed. Saturasi tertinggi dalam satu run. *(Technical: palette warms from Visiting Phase, contrast increases sharply, draft text area near-white background, badge accent color at maximum saturation, minimal 2-frame pulse animation on upload)*

**Deskriptor atmosfer:** "glow layar detik sebelum tekan send" / "overexposed preview, no going back" / "comment section opening in real time" / "warna notifikasi yang datang"

**Energy level:** Frenetic saat posting → held stillness saat follower count mulai update.

**Elemen kunci:** Badge "REVIEWED" atau star rating overlay muncul di full accent color di atas foto — visual payoff yang dibangun sejak Visiting Phase. Harus terasa conclusive, bukan celebratory.

---

### 2.4 End-of-Month / Bill Paying

**Emosi target:** Reckoning — ketenangan gelap membuka laporan bank. Bukan panik — pengakuan atas aritmatika yang sudah terjadi.

**Karakter cahaya:** Desaturasi tertinggi setelah Game Over. Cool, dingin, kompressed. *(Technical: saturation drops to 15–25% across all elements, food photos thumbnailed small at periphery, balance number rendered in red/amber/green semantic color depending on state, no warm tones)*

**Deskriptor atmosfer:** "notifikasi bank yang tidak bisa di-dismiss" / "layar yang redup karena terlalu lama dilihat" / "angka dalam warna final reminder" / "feed yang tiba-tiba sunyi"

**Energy level:** Slow dan weighted. Animasi hanya pada angka yang berubah.

**Elemen kunci:** Angka saldo bulan ini — teks terbesar di layar, dalam warna semantik (hijau = aman, amber = kritis, merah = bahaya). Skala angka relatif terhadap elemen lain membawa beban emosional.

---

### 2.5 Game Over / Bankrupt

**Emosi target:** Finality without melodrama. Bukan jump scare — notifikasi yang lambat. Seperti akun yang di-suspend, bukan gedung yang runtuh.

**Karakter cahaya:** Near-monochrome. Seluruh layar drain ke cold blue-grey, kecuali overlay "BANGKRUT" yang tetap deep red. *(Technical: palette desaturates to ~5%, single accent element at full saturation, no animation except badge appearing)*

**Deskriptor atmosfer:** "akun yang di-flag dan di-suspend" / "grey halaman yang gagal load" / "red text on white error screen" / "feed yang membeku di tengah scroll"

**Energy level:** Completely still. Tidak ada gerakan kecuali badge "BANGKRUT" muncul.

**Elemen kunci:** Badge "BANGKRUT" — full red, besar, applied over foto profil player atau foto terakhir yang di-post. Harus terasa seperti moderation badge platform: klinikal, tidak dramatis.

---

### 2.6 Main Menu / Between Runs

**Emosi target:** Kegelisahan khusus seseorang yang scroll profil lama sebelum mulai kerja lagi. Retrospektif bercampur antisipasi.

**Karakter cahaya:** Neutral-warm, slightly nostalgic. *(Technical: medium saturation, low contrast, archived post thumbnails from previous runs rendered with slight color temperature shift — warmer/softer than in-run versions)*

**Deskriptor atmosfer:** "scroll feed sendiri dari enam bulan lalu" / "cahaya layar warm di kamar yang sepi" / "momen sebelum mulai rekam lagi" / "profile page, belum logout"

**Energy level:** Resting but not idle.

**Elemen kunci:** Tombol "Start Run" — dirancang secara visual seperti tombol "+" create content di social media app. Framing ini memposisikan run baru sebagai membuat konten baru, bukan reload save.

---

### 2.7 Milestone Moments (Viral, Follower Threshold, Restoran Tutup)

**Emosi target:** Disruptive surprise — sesuatu yang merusak ritme. Bukan murni positif, bukan murni negatif. Perasaan uncanny ketika sesuatu yang kamu buat menjadi lebih besar dari yang kamu maksud.

**Karakter cahaya:** Interrupts phase palette dengan brief flash overexposed (1–2 frame white-wash), lalu kembali ke phase yang aktif. *(Technical: "Going Viral" uses Publishing Phase peak saturation. "Restoran Tutup" uses grey-wash over restaurant's food photo)*

**Deskriptor atmosfer:** "notification banner yang menginterupsi segalanya" / "color temperature shift saat HP menyala di tengah percakapan" / "overexposed satu frame, lalu normal lagi"

**Energy level:** Sudden spike → rapid resolution. Tidak berlama-lama.

**Elemen kunci:** Notification banner atau overlay label — sama dengan digital stamps dari Section 1, tapi muncul uninvited dari atas layar, bukan sebagai aksi player. Distinction: stamp player = deliberate, placed; platform notification = arrives from top, unsolicited.

---

### Atmosphere Consistency Check

| State | Feed Aesthetic? | Social Media Language? |
|---|---|---|
| Planning | ✓ restaurant grid, engagement preview | ✓ feed scroll, follower estimates |
| Visiting | ✓ food photo as primary frame | ✓ unfiltered post preview |
| Publishing | ✓ post creation UI, upload moment | ✓ send button, notification color |
| Bill Paying | ✓ feed goes quiet, accounting takes over | ✓ notification-as-dread |
| Game Over | ✓ account suspended, frozen feed | ✓ moderation badge language |
| Main Menu | ✓ profile page, archived posts | ✓ "+" create new content |
| Milestones | ✓ notification interrupts feed | ✓ banner, algorithmic surge |

---

## 3. Shape Language

*This section serves the Visual Identity Statement: one shape language, two registers — UI infrastructure (angular/deliberate) and content (organic-simulated through pixel dithering).*

**Overriding constraint:** This is a UI-dominant game. Shape decisions are primarily typographic and compositional. Complex environment geometry is not a priority. Clean silhouettes, consistent border treatment, and deliberate edge radius are the primary tools.

---

### 3.1 Character Silhouette Philosophy

**Working resolution constraint:** Characters are seen primarily in two contexts — feed thumbnails (32×32 or 48×48 px portrait crops within card grid) and encounter panels (larger single-frame during Visiting Phase). Every silhouette must communicate archetype at thumbnail size first.

**Core rule:** One unique silhouette feature per archetype, readable in 4 pixels of width difference.

---

**Player Character (the reviewer)**

Silhouette language: Upright and neutral — no dominant visual feature. The reviewer is the camera, not the subject. In character-facing scenes, the player is always partially obscured: hand holding phone toward camera, back-of-head shot, or phone screen reflection. The player's persistent on-screen identity is a small circular avatar crop in the feed UI, not a full body sprite.

*Pillar 3 — Reviewer Bukan Dewa:* The reviewer has no imposing silhouette. The blank-space-as-self creates identification — "that absence is me." Power without a face.

---

**Restaurant Owners / Warung Operators**

Silhouette language: Wide and low center of gravity. Round-shouldered or square-shouldered depending on establishment tier — always grounded. Distinguishing pixel feature: **headwear** (kopiah, bandana, chef's cloth, baseball cap). The hat is the silhouette apex and primary 4-pixel differentiator at thumbnail scale.

*Pillar 4 — Restoran Punya Jiwa:* Owner silhouette is inseparable from establishment identity. Swap the hat, swap the restaurant.

---

**Chefs**

Silhouette language: Tall and narrow. Vertical emphasis. Distinguishing pixel feature: **hand state** — at least one hand always in active position (holding pan, ladle, cloth). An idle chef with both hands down reads as an owner, not a chef.

*Emotional intention:* Chefs are the source of quality the reviewer never fully controls. Vertical active silhouette = precision in progress, off-screen.

---

**Rival Reviewers**

Silhouette language: Mirror of the player archetype but made legible. Visible faces, forward-leaning posture, consistent "posting gesture." Distinguishing pixel feature: **phone angle** — phone at eye level (evaluation mode, active threat) vs. phone held down (idle).

*Emotional intention:* Recognition-anxiety. "That gesture is mine. They are doing what I do." Shape-language delivery of Pillar 3 with no text required.

---

**Fans / Followers**

Silhouette language: Never individual — always aggregate. Fans exist as comment stacks, follower count numbers, repeated palette-swapped sprites. If a single fan NPC is required, they default to a generic "phone-scroll" posture — no hat, no gesture, no distinguishing feature. Generic on purpose.

*Emotional intention:* Fans don't have faces, they have numbers. Makes the Publishing Phase follower count update feel like moving an aggregate, not connecting with people. Feeds Pillar 1 — followers are eventually rupiah.

---

### 3.2 Environment and UI Geometry

The game has no traditional environment. The "environment" is the Visiting Phase panel — composed food photo tiles, ambiance tiles, and evaluation checklist UI overlay. Environment/UI distinction collapses into one surface: the feed.

**Panel and card geometry grammar:**

**Slight imperfection as authenticity signal.** Outer containers use a consistent **2px corner radius** (deliberate but not corporate-soft). Interior elements — photo crops, badge overlays, checklist items — use **0px radius** (pixel-perfect hard edge). The contrast communicates: the container is the creator's hand; the content inside is raw documentation.

*Design test:* If a UI panel looks like it belongs to a banking app or food delivery service, it has too much geometric consistency. Panels should feel sized to content, not the other way around.

**Grid is scaffolding, not aesthetic.** The Planning Phase restaurant grid uses a consistent column count, but card heights can vary by one unit based on caption length — mimicking real social media grid layout where content crops unevenly. This is not a bug; it is a feature of the "managed by a human" visual language.

**No decorative geometry.** Zero ornamental borders, no corner filigree, no divider lines that exist purely for decoration. Every line on screen is either a content boundary or a functional separator.

*Pillar 2 — Rutinitas yang Menyerap:* Familiar geometry lowers resistance. The player slips into the monthly routine more easily because the UI speaks a language they already have muscle memory for.

---

### 3.3 UI Shape Grammar vs World Aesthetic

One language, two registers — not two separate grammars.

**UI shapes (feed infrastructure):** Sharp corners at content boundaries, consistent 2px outer radius on containers, hard-edge badges, monospaced numerals for all financial figures. Minimum geometry. Functional containers.

**World shapes (food photography, restaurant ambiance tiles):** Organic edge-softness through **pixel dithering at tile borders** — not actual curved geometry. Food photography tiles use 1–2 pixel dithering at subject edges to simulate photographic blur or depth-of-field. The food subject earns softness through photographic realism simulation; the UI frame that holds it remains angular.

**The rule:** UI geometry = angular and deliberate (infrastructure). Content = organic-simulated (what was captured). The contrast between the crisp UI frame and the organic photo inside it is the contrast between "the creator managing a feed" and "the thing they documented."

*Pillar 4 — Restoran Punya Jiwa:* The restaurant's soul lives in the organic texture of its food photo tile, not in the card that frames it.

---

### 3.4 Hero Shapes vs Supporting Shapes — Visual Hierarchy

In a UI-dominant game, hierarchy is achieved through **size delta**, not depth or lighting. Scale communicates importance; no glow, animation, or ornament compensates for inadequate scale. This is a design principle and a production efficiency rule for a solo developer.

| Tier | Element | Shape Treatment | Phase where it peaks |
|---|---|---|---|
| **1** | Food Photo | Fills card edge-to-edge, 0px internal margin — photo IS the card | Visiting |
| **2** | Balance Number | Monospaced block, fixed corner position, no border, peripheral-vision readable | Bill Paying |
| **3** | Checklist Items | Uniform pill row — equal width, height, padding per item. No variation regardless of content length | Visiting |
| **4** | Badges / Overlays | Fixed 2px radius, always top-left or top-right of photo card (never centered, never bottom). App notification badge position. | Publishing / Game Over |

**The one hierarchy rule:** If an element needs to feel more important, make it larger. Never compensate with special effects.

*Pillar 1 — Tiap Rupiah Bercerita:* The financial number at Tier 2 means it is always visible, always readable without focus. Every decision the player makes happens in the peripheral awareness of that number. The shape hierarchy is the mechanic — you cannot not see how much you have left.

---

### Shape Language Consistency Check

| Shape Decision | Serves Feed Aesthetic? | Solo-dev producible? |
|---|---|---|
| One silhouette feature per NPC archetype | Yes — thumbnail-sized social media profile logic | Yes — 4px delta, no complex rigging |
| 2px outer / 0px inner radius contrast | Yes — creator container vs raw content | Yes — two values, applied consistently |
| Grid with 1-unit height variation | Yes — algorithmic feed behavior | Yes — VBoxContainer/GridContainer in Godot |
| No decorative geometry | Yes — feed, not scrapbook | Yes — less work, not more |
| Photo fills card edge-to-edge | Yes — photo IS the card | Yes — zero-padding rule, one decision |
| Monospaced balance number, fixed position | Yes — notification-as-dread | Yes — single font, fixed anchor point |
| Uniform checklist pill rows | Yes — platform checklist UI pattern | Yes — repeated single sprite |
| Badges top-left/right, 2px radius | Yes — app notification badge position | Yes — two positions, one shape |

---

## 4. Color System

[To be authored]

---

## 5. Character Design Direction

[To be authored]

---

## 6. Environment Design Language

[To be authored]

---

## 7. UI/HUD Visual Direction

[To be authored]

---

## 8. Asset Standards

[To be authored]

---

## 9. Reference Direction

[To be authored]
