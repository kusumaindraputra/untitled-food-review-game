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

*This section serves the Visual Identity Statement: the palette distinguishes "platform colors" (what the feed infrastructure uses) from "world colors" (what food and restaurants bring to the screen). Saturation is the single lever that drives phase transitions — no separate per-phase palette is needed.*

---

### 4.1 Primary Palette

Six named colors plus one wild card. Six is the minimum for this game's semantic needs — fewer forces color overloading; more creates management debt for a solo developer. Every color is defined at **nominal saturation** (the value you paint with) and its **collapsed saturation** behavior (what it becomes when the global saturation lever drops during Bill Paying / Game Over).

---

**1. Layar Pagi** ("Morning Screen")
Hue: Blue-white, 200–210°, very low saturation at nominal (10–15%).
Role: Base background tone for all UI panels. Screen-white with a slight cool cast — not warm off-white. Every piece of content sits on top of it.
Most prominent in: Planning Phase (dominant), Bill Paying (returns as clinical presence).
At low saturation: Becomes near-pure white. Correct — reckoning phases should feel like a stark screen, not a warm page.

**2. Aspal Malam** ("Night Asphalt")
Hue: Dark cool-neutral, 215–225°, high value contrast with Layar Pagi.
Role: Primary text color and UI boundary color. All body text, labels, checklist item text, financial figures, inactive UI states. Screen dark, not ink dark.
Most prominent in: All phases equally. Infrastructure color.
At low saturation: Flat cold grey. Correct for Bill Paying — the UI reads as drained and clinical.

**3. Warung Siang** ("Midday Warung")
Hue: Warm amber-orange, 28–38°. Food-warm, not paper-warm. *(Distinction: paper-warm = 40–55°; food-warm = 28–38° — the color of rendered fat, caramelized sugar, afternoon warung light.)*
Role: **World color only — not a UI color.** Used in food photo tiles, restaurant ambiance background tiles, and Visiting Phase ambient warmth. Never appears in buttons, labels, or UI chrome. When Visiting Phase "warms the palette," it is these content tiles that carry the shift, not the UI.
Most prominent in: Visiting Phase, Publishing Phase warm-up.
At low saturation: Muddy sand-beige. The only primary color that looks wrong when drained — which is correct. During Bill Paying, Warung Siang disappearing signals the comfortable food-focused part of the month is over.

**4. Notifikasi** ("Notification")
Hue: Electric blue-violet, 255–265°, high saturation.
Role: **Platform color — interactive only.** Tap targets, selected states, the "+" create content button on Main Menu, follower count highlights, any element that means "this is actionable." This color belongs to the platform, not to the player.
Most prominent in: Planning Phase (restaurant selection), Publishing Phase (post button), Main Menu.
At low saturation: Flat grey-blue, nearly indistinguishable from Aspal Malam. During Bill Paying, interactive affordances should effectively disappear — the lever achieves this automatically.

**5. Saldo Merah** ("Red Balance")
Hue: Pure red, 355–5°. Clinical red — no orange shift, no pink shift. Banking app error red.
Role: Financial danger and the BANGKRUT badge. The most semantically loaded color in the palette — means one thing: the system is warning you.
Most prominent in: Bill Paying (danger state), Game Over (BANGKRUT badge).
At low saturation: **Exempt from the global saturation lever.** BANGKRUT badge stays at full saturation even when the rest of the screen is at 5%. Treat as a non-desaturated overlay on a separate UI layer that bypasses any scene-level saturation shader.

**6. Amber Kritis** ("Critical Amber")
Hue: Warm yellow-amber, 42–50°. Distinct from Warung Siang (orange-amber) — further toward yellow, the hue humans associate with "warning but not yet stopped."
Role: Financial mid-state. When balance is tight but not terminal, financial figures render in Amber Kritis. Also the color of a published review with no engagement yet — the waiting color.
Most prominent in: Bill Paying (warning state), post-Publishing pre-engagement hold.
At low saturation: Pale yellow, nearly invisible on Layar Pagi. See colorblind backup in Section 4.5.

**Wild card — Foto Hijau** ("Photo Green")
Hue: Muted sage-green, 140–150°. Intentionally lower saturation than other primaries at nominal (40–50%). Not bright UI green — the color of a garnish, banana leaf under a dish, healthy produce.
Role: Financial safety (balance number when comfortable), positive review outcome, "safe to proceed" states. Lower saturation at nominal prevents it from reading as triumphant — a safe balance means you get to play another month, not that you've won.
Most prominent in: Bill Paying (safe balance state), Planning Phase (successfully-visited restaurant indicators).
At low saturation: Flat cool grey, indistinguishable from Aspal Malam. See colorblind backup in Section 4.5.

---

### 4.2 Semantic Color Vocabulary

Specific to the food reviewer / social media world — not generic UI semantics.

**RED (Saldo Merah) = The platform has flagged you.**
Not abstract "danger" — red means the system has formally notified you of a problem. Bank notification red. Overdue payment red. Account suspension red. It arrives top-down from a system with power over you. This is why BANGKRUT uses the same red as a negative balance — both are the platform asserting authority over the player's account.

**AMBER (Amber Kritis) = You have one more chance to scroll past this.**
The yellow-amber of a notification that has been seen but not addressed. Not yet forcing action, but not ignorable. Also carries the specific anxiety of a post with no engagement — held breath before the algorithm decides.

**GREEN (Foto Hijau) = Your content is performing and your table is set.**
Not "you won" — "you are nourished and stable." Safe balance in Cicip & Catat means you get another month, not victory. The muted saturation prevents it from reading as triumphant.

**BLUE (Notifikasi) = The platform wants your attention.**
Every blue element is a place where the player can take action. Blue is the platform's color, not the player's. The player's color is the absence of a dominant color — the reviewer is represented by Layar Pagi (neutral screen-white).

**NEAR-WHITE (Layar Pagi) = Feed at rest.**
Background that makes content visible. The only time it has meaning is when it is taken away — when it shifts toward Aspal Malam territory, the feed has gone dark and the player is accounting, not creating.

**WARM AMBER-ORANGE (Warung Siang) = You are in the presence of something worth eating.**
The only color that belongs to the world rather than the platform. When Visiting Phase warms toward this hue, the visual grammar says: you are not in the feed right now, you are in a restaurant. The platform recedes; the subject reasserts itself.

---

### 4.3 Per-Phase Color Temperature Rules

*(Food photos always remain at nominal hue unless a special treatment is specified. These rules apply to UI chrome and ambiance/background tiles only.)*

**Planning Phase** — Cool. Blue-white screen glow.
Shift all UI non-photo hues -8 to -12° toward blue. Layar Pagi at full brightness. Notifikasi at full saturation (most interactive phase). Warung Siang absent from UI entirely — only in food photo content.
Food photos: 100% saturation, nominal hue. The only warm things on screen — contrast is deliberate.

**Visiting Phase** — Warm but contained. Overhead-light warmth.
UI panels shift +6 to +10° toward warm. Warung Siang appears in background ambiance tiles. Layar Pagi takes on a barely perceptible cream tint (3–5% warm shift). Checklist UI elements remain Aspal Malam-on-Layar Pagi; checklist row backgrounds can accept 10% Warung Siang tint on selected state.
Food photo: Full panel, 100% saturation, 100% brightness. Warmth lives in background tiles, not UI chrome.

**Publishing Phase** — Overexposed warm. Screen-bright.
UI shift +12–15° warm from Planning baseline. Notifikasi at maximum saturation. Layar Pagi pushes toward pure white (cool cast removed). Badge overlay (REVIEWED, star rating) at full saturation regardless of global saturation value — this is the visual payoff of the entire phase cycle. 2-frame brightness pulse on upload confirmation.
Food photo: 100% saturation but overexposed-bright UI surrounds it — contrast with background reduced. The act of publishing is the subject now, not the food.

**Bill Paying Phase** — Drained. No warmth source.
Global saturation multiplier: 0.15–0.25 on all scene elements except semantic financial colors. Warung Siang disappears. Notifikasi disappears. Remaining: Layar Pagi (clinical white), Aspal Malam (cold grey), and the semantic trio applied to balance number only. Food photos reduced to small desaturated periphery thumbnails.
*Technical note:* Implement as global CanvasModulate or post-process color-grade on scene layer. Semantic financial colors must be drawn on a separate UI layer bypassing this grade.

**Game Over** — Cold halt. Near-monochrome.
Scene layer desaturation ~5%. BANGKRUT badge on top-most UI layer outside saturation shader scope — full Saldo Merah, 100% saturation, 100% opacity. No animation. Layar Pagi reads as cold blue-tinted white — the white of an error screen.

**Main Menu / Between Runs** — Neutral-warm. Nostalgic softness.
Medium saturation (60–70% of nominal). +4 to +6° toward warm from Planning. Archived food photo thumbnails from previous runs: apply faint desaturation and +8° warm shift to signal "this is the past." The "+" create new content button uses Notifikasi blue at full saturation — the only live, current-feeling element in an otherwise retrospective palette.
*Technical note:* Archived photo treatment achievable with a single semi-transparent warm tint overlay (~15% opacity) rather than recolouring individual sprites.

**Milestone Moments** — Phase flash. Brief overexposure.
1–2 frame white-wash flash, then return to current phase palette. "Going Viral" uses Publishing Phase peak saturation, pushed to maximum. "Restoran Tutup" uses grey-wash over that restaurant's food photo. Notification banners use same digital stamp design from Section 1 — but drawn on top-UI layer, uninvited.

---

### 4.4 UI Palette Rules

**The core rule: UI uses platform colors; world content uses food colors.**

UI elements (panels, buttons, labels, badges, navigation, checklist rows, financial figures) use only: Layar Pagi, Aspal Malam, Notifikasi, and the semantic trio (Saldo Merah, Amber Kritis, Foto Hijau). Warung Siang is never a UI color — it enters the screen only through food photo tiles and ambiance background tiles.

**Background value target:** Layar Pagi ≈ #F5F7FA equivalent. Near-white with barely perceptible blue-cool cast (200–210° hue, 8–12% saturation, 97–98% value in HSV). Produces a simultaneous contrast effect — food photo warm tones read approximately 10–15% more saturated than they technically are because the surround is cooler. A free visual enhancement.

**Dark mode:** Not in scope for first pass. If added later, Aspal Malam becomes background and Layar Pagi becomes text color — roles invert cleanly. Do not add colored tints to either in dark mode.

---

### 4.5 Colorblind Safety

Primary risk: the financial state trio (Foto Hijau / Amber Kritis / Saldo Merah) uses the classic red-amber-green pattern — the most common failure point for deuteranopia and protanopia.

**Required backups — color is never the only signal for financial state:**

- **Saldo Merah (danger):** Downward-arrow glyph prefix on the balance number, rendered in Aspal Malam. The BANGKRUT badge uses text ("BANGKRUT") as primary communication — never relies on red being perceived.
- **Amber Kritis (warning):** Exclamation-mark or warning glyph prefix on the financial number. Warning meaning also reinforced by global saturation reduction of surrounding UI elements — context communicates stress even if the hue is ambiguous.
- **Foto Hijau (safe):** Small stable-state indicator (flat horizontal line or checkmark) adjacent to a safe balance. Lower priority — failing to see "safe" causes false anxiety, not missed danger.

*Asset detail:* Colorblind-safe glyph set defined in Section 8 (Asset Standards). The rule here: backup via shape, position, or text — never add extra colors to solve colorblind problems.

---

### 4.6 Food Photo Color Treatment

Food photos are painted at nominal saturation and left alone. **The UI shifts around them; photos do not shift.** Exception: Bill Paying and Game Over, where photos join global desaturation because in those phases, food is no longer the subject.

**Three-tier photo color system (visual shorthand for restaurant quality — no tutorial needed):**

| Tier | Restaurant type | Color temperature | Contrast | Pixel treatment |
|---|---|---|---|---|
| **Tier 1** (high-end) | Fine dining | Warm bias, controlled | High — subject separates cleanly | Warmest values of Warung Siang as highlight |
| **Tier 2** (mid-range) | Standard restaurants | Neutral | Moderate | "Shot with a decent phone on a good day" |
| **Tier 3** (low-end) | Warung, street food | Cool or mixed | Low — dish doesn't fully separate from table | More dithering at edges, less contrast |

**Color budget per food photo tile: 16 colors** (production target for solo dev; may expand to 24 if resolution requires it). The tile's dominant color must be identifiable as belonging to one of the three temperature tiers above without reading any text.

**Simultaneous contrast note:** During Planning Phase (cool UI surround), food photo warm tones read ~10–15% more saturated than they are. During Visiting Phase (warm UI ambient), this effect diminishes — the photo and UI converge in temperature, creating a subtle "you are now inside the experience" visual signal.

---

### Color System Consistency Check

| Rule | Serves Feed Aesthetic? | Solo-dev producible? |
|---|---|---|
| 6 primary + 1 wild card palette | Yes — minimum viable semantic system | Yes — trackable without a spreadsheet |
| Saturation lever drives all phase changes | Yes — single mechanic, all states | Yes — one CanvasModulate or shader |
| Warung Siang = world/food only, not UI | Yes — platform vs. restaurant distinction | Yes — one rule to check per element |
| Notifikasi blue = platform, interactive only | Yes — feed grammar, tap-target language | Yes — limits blue to one meaning |
| Saldo Merah exempt from saturation lever | Yes — suspension/danger always reads | Yes — separate UI layer |
| Colorblind backup via shape, not palette | Yes — accessibility, not extra colors | Yes — glyph prefixes, no new sprites |
| Food photos painted once, UI shifts around | Yes — photos are currency, not decor | Yes — halves the color management work |
| Photo tier readable from color temperature alone | Yes — visual shorthand, no tutorial | Yes — three temperature bands |

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
