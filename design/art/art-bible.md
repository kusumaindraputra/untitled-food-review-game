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

*This section serves the Visual Identity Statement: characters exist inside a social media feed — they are the faces behind the posts, not heroes in a narrative. Every character design decision must read at feed-card thumbnail scale before encounter panel scale.*

### Production Priority Order

1. Player avatar (24×24px) + hand/phone sprite (48×32px) — **MVP blocker**
2. Restaurant Owner base sprite (32×48px) — **MVP blocker**
3. Encounter panel compositions + Chef + Rival Reviewer sprites — **Vertical Slice**
4. Per-character headwear/accessory variant swaps — **Alpha**

Do not produce anything in priority 3–4 until the MVP checklist loop is validated.

---

### 5.1 Player Representation — The Reviewer as Absence

The player has no protagonist sprite. Three player-presence sprites replace a character sheet:

**5.1.1 Feed Avatar (24×24px circular crop)**

The player's persistent on-screen identity — same position as a profile photo in a social media app.

- Canvas: 24×24px, 2px circular mask with 1-pixel partial alpha at edge (simulates circular crop, not hard rectangular mask)
- Content: Upper face only, eye level to top of head, slightly off-center — an amateur profile photo taken in bad lighting, not a portrait. No mouth visible.
- Color constraint: Layar Pagi + Aspal Malam only. No Warung Siang, no Notifikasi. The reviewer has no brand color.
- Pixel budget: 6–8 colors including transparency. One additional low-saturation skin tone permitted (15–20 HSV saturation).
- Game Over state: BANGKRUT badge composited on top by UI layer — the avatar sprite is not redrawn.
- *Pillar 3 — Reviewer Bukan Dewa:* The avatar is low-resolution, slightly amateur, unimpressive. The reviewer's power is not visible in their face.

**5.1.2 Hand/Phone Sprite (48×32px, landscape)**

The closest thing to a protagonist sprite — appears in the lower portion of the Visiting Phase screen.

- Canvas: 48×32px. Hand enters from bottom-left corner, phone screen facing the food photo above (mimicking the gesture of taking a food photo).
- Content: Hand + phone only. No wrist jewelry, no arm beyond 8px. Phone is identifiable as a phone (rectangular, simple bezel, no brand). Phone screen shows a 2-color silhouette of the current food photo — not a detailed thumbnail.
- Color: Same low-saturation skin tone as the avatar. Phone body in Aspal Malam. Phone screen may carry one simplified warm color if the food photo is warm-tier.
- Animation: **0 frames — static sprite.** Stillness matches the contemplative mood of Section 2.2 (Visiting Phase). The stillness is a feature, not a limitation.
- Pixel budget: 8–10 colors.
- *Pillar 2 — Rutinitas yang Menyerap:* The hand-and-phone is the gestural anchor of the monthly ritual. Every visit begins and ends with this same compositional element.

**5.1.3 Back-of-Head Sprite — Deferred to Vertical Slice**

Not needed for MVP. If produced: 24×40px, rear view, dark hair against restaurant ambient background. No face details, neutral Aspal Malam clothing, no distinguishing features. Deliberate genericness serves Pillar 3.

---

### 5.2 NPC Archetype Design Rules

**Shared production rule:** Design all NPC sprites at 32×48px base. Verify silhouette reads at this size before adding detail. Never design encounter-panel-first.

**Shared color constraints:**
- NPC clothing/accessories may use Warung Siang sparingly (world color, not platform color), but at **70% of food photo tile Warung Siang saturation** — NPCs must not compete with food photography for visual hierarchy.
- Three pre-approved skin tones across the NPC pool: (a) warm medium-dark, (b) warm medium, (c) cool light. Each character assigned one tone for consistency.
- Notifikasi blue (255–265°) never appears on NPC sprites — it is the platform's color.
- Saldo Merah on NPC sprites: reserved for post-Alpha meta-progression indicators only.

---

**Restaurant Owner / Warung Operator**

*Section 3 establishes: wide/grounded silhouette, headwear as 4px differentiator.*

Proportion (32×48px base):
- Height: 38–42px visible body. Width at shoulders: 18–20px (widest NPC archetype).
- Head-to-body ratio 1:3 (head ≈ 12px). Center of gravity in lower third.

Headwear (primary differentiator — permanent per character, never changes):
- Types: (a) kopiah/peci — flat-topped 4px protrusion, formal; (b) bandana at forehead — wider asymmetric; (c) baseball cap — horizontal brim 4px left or right; (d) chef's cloth as bandana — distinct fold from type b; (e) no headwear — reserved for 1–2 "anomalous" memorable owners.
- Headwear carries one high-saturation accent color outside the named palette. This is how individual owners become visually memorable within the archetype.

Expression range (sprite swap, not animation):
- 2 required: Neutral/Guarded + Pleased/Open. Tense/Closed optional.
- Body sprite static and reused. Only the head sprite swaps. This halves expression production cost.
- No mouth or blink animation. Eyebrow angle and shoulder posture carry expression.

Clothing: All owners wear a white (Layar Pagi) apron with Aspal Malam trim — the one shared uniform element. Shirt under apron varies per individual. No logo text on clothing.

*Pillar 4 — Restoran Punya Jiwa:* The owner's grounded stance says: this place has been here longer than you have been reviewing it.

---

**Chef**

*Section 3 establishes: tall/narrow silhouette, active hand state as differentiator.*

Proportion (32×48px base):
- Height: 44–46px (tallest archetype). Width at shoulders: 12–14px.
- Head-to-body ratio 1:4 (head ≈ 10px). Forward tilt of 2–3px in shoulders — the chef is always mid-task.

Hand state (primary differentiator — fixed per encounter):
- (a) Ladle/spoon held forward — production cooking, high confidence
- (b) Cloth over arm, one hand on hip — between tasks, evaluating
- (c) Both hands raised — rare, specific encounter moment (argument, revelation). Not an idle state.

Expression range: Same economy as owners — 2 base states, body static, head swaps. Chef's toque/cloth cap is the same across all chefs — no headwear variation (hand state is the differentiator, not the hat).

Clothing: White chef's coat (Layar Pagi body, Aspal Malam collar/button line) identical across all chefs at MVP. One accent thread on sleeve edge per individual. No apron — aprons belong to owners, distinguishing the archetypes at thumbnail scale.

Context: Chefs appear primarily in the background of kitchen-context panels or as secondary figures. Design for legibility at 60% screen coverage, not full-frame.

*Pillar 4:* Perpetual chef activity = evidence the restaurant's soul lives in process. *Pillar 3:* You can evaluate what comes out of the kitchen; you cannot direct what happens inside it.

---

**Rival Reviewer**

*Section 3 establishes: mirror of player archetype, visible face, forward lean, phone angle as differentiator.*

Proportion (32×48px base):
- Height: 40–44px. Width: 14–16px. Forward lean 3–4px from heel line — posture provides visual mass beyond width.
- Head-to-body ratio 1:3.5. **The rival has a visible face; the player does not.** This is deliberate.

Phone angle (primary differentiator):
- Eye level: actively assessing, threat present (same restaurant as player)
- Hip level, screen outward: present but not focused (background state)

Expression: Neutral/Focused + Smug/Noticed. Rivals have more expressive mouths than owners or chefs — a visible smirk or flat line communicates character. Mouth is primary; eyebrows secondary.

Clothing: Variable per individual. One shared marker across all rivals: a small lanyard/press credential (2×3px rectangle in Aspal Malam with one accent pixel) at the chest. Visible at encounter panel scale, not thumbnail scale — thumbnail differentiation relies on phone angle + forward lean alone.

*Pillar 3 — Reviewer Bukan Dewa:* The rival's visible face is the most direct visual statement of this pillar. They are doing what you do. They have a face. You don't.

---

### 5.3 Expression and Pose Style

**Global rule: sprite swap, not animation.**

Body sprite is static and reused. Head is a separate sprite at a fixed anchor. Expression changes between player interactions, not during them — consistent with Section 2's meditative rhythm.

**Idle animation:** 2-frame breathing loop (frame A: rest; frame B: shoulders +1px up, head -1px) at 0.8–1.2 second cycle. Optional in MVP — static NPCs are acceptable.

**Exaggeration level:** Moderate. Reference: Papers Please NPC design — caricatures with functional emotional reads, not portraits. Eyebrow angle is the primary expression tool. Eye shape is secondary. Mouth tertiary (rivals only at thumbnail scale).

**Pixel-level guidance:**
- Eyes at 32×48px: 3×2px. At encounter scale: 5×3px with 1-pixel highlight (painted into static sprite, not animated).
- Eyebrows: 4px wide, single color. Three states: horizontal (neutral) / angled inward-up (tense/proud) / angled outward-down (open/tired).
- Mouth at 32×48px: not shown on owners or chefs. At encounter scale (5px wide): flat (neutral) / slight curve (positive) / tight corners (tense).
- Skin pixel count at 32×48px: ≈40–60 pixels. Fewer, larger shapes read better than noisy detail.

---

### 5.4 LOD Philosophy — One Sprite, Two Display Scales

The game operates at two effective display scales:

**Card thumbnail scale (32×48px portrait within feed card):** Communicates archetype only — not emotion, not story. Hat silhouette, hand state, phone angle must read here. This is the canonical sprite.

**Encounter panel scale (≈80×128px display, 2.5× nearest-neighbor from base sprite):** Same sprite rendered larger. The visible pixel grid is intentional — it is the visual language of deliberate evaluation. No additional detail painted at encounter scale.

*Technical note (Godot 4.6):* Use `texture_filter = NEAREST` (or CanvasItem equivalent) for pixel-perfect scaling. The encounter panel adds a painted backdrop (ambiance tiles + compositional frame) — the NPC sprite itself is the same asset at both scales.

*Pillar 2 — Rutinitas yang Menyerap:* The player's eye learns archetypes at thumbnail scale first. Recognition at encounter scale is immediate — routine has primed the read.

---

### 5.5 Encounter Panel Visual Treatment

**Framing:** Half-body (cropped at waist). Head and torso visible. This matches social media content language for restaurant/counter subjects and reduces visible sprite area by 40% without information loss.

**Composition offset (never centered):**
- Owner encounters: NPC at 65–70% from left
- Chef encounters: NPC at left 20–30% (kitchen doorway, partially occluded)
- Rival encounters: NPC at 30% from left (approaching from left, forward lean direction reinforces movement)

**Screen zone rule:** Food photo (center/top) / NPC (lower-left or lower-right) / Checklist UI (opposite side from NPC). These three zones do not overlap.

**No portrait border, no vignette.** NPC exists in scene space as a figure, not as a character card. Consistent with Section 3's "no decorative geometry" rule.

**Expression on checklist confirmation:** When the player confirms a criterion that affects the NPC (e.g., marking Service as poor), the NPC head sprite swaps to Tense expression immediately — no delay, no animation. Abruptness is correct; decisions have immediate weight.

**Empty stool:** Some Tier 3 warung encounters have no staffed counter. The NPC zone shows an environmental tile (empty stool, cloth over counter) instead of a sprite. Absence communicates as meaningfully as presence.

*Pillar 4:* Encounter panel is where the restaurant's soul is present (a face) or withheld (an empty stool). *Pillar 1:* NPC expression swap on checklist confirmation makes every criterion feel consequential beyond its number.

---

### 5.6 Character Consistency Check

| Decision | Serves Section 1 (Feed)? | Serves a Pillar? | Solo-dev producible? |
|---|---|---|---|
| No protagonist sprite; avatar + hand/phone | Yes — profile photo + user gesture | P3 — no imposing hero face | Yes — 2 assets replace full character sheet |
| Archetype readable at 32×48px | Yes — grid card readability | P2 — routine primes recognition | Yes — silhouette-first discipline |
| Sprite swap for expressions | Yes — static post logic | P2 — stillness = contemplation | Yes — halves expression production cost |
| One sprite, two scales (nearest-neighbor) | Yes — pixel aesthetic intentional | P2 — no resolution break in routine | Yes — zero additional art per scale |
| Half-body framing, offset, no border | Yes — across-the-counter feed content | P4 — figure in their place | Yes — no border art needed |
| NPC at 70% Warung Siang saturation | Yes — NPCs serve food photos, not compete | P4 — food photo hierarchy T1 | Yes — one saturation rule per archetype |
| Empty stool for unmanned encounters | Yes — absence as content | P4 — soul can be withheld | Yes — 1 environmental tile reused |

---

## 6. Environment Design Language

*This section serves the Visual Identity Statement: environment art exists only to make the feed feel real. The feed IS the environment. Ambiance tiles are not a world — they are evidence that a world exists behind the feed.*

**Governing rule:** Environment only appears in three contexts: (1) ambiance tiles in the Visiting Phase, (2) card background impressions in the Planning Phase feed, (3) neutral feed backdrop between phases. No explorable world exists.

---

### 6.1 Ambiance Tile System

The Visiting Phase panel is the only place with something resembling a scene — a composed arrangement of tiles behind the NPC and food photo. Tile-based composition is a production efficiency principle: a small shared library recombined per restaurant keeps total asset count feasible for a solo developer.

**What tiles depict:** Fragments of architectural or material reality — a wall surface, a single decorative element, a glimpsed ceiling fixture, a counter edge. Each tile is a piece of evidence: visual archaeology the player reads as the restaurant's history without text.

**Resolution:** 48×48px per tile. Aligns with NPC base sprite width for consistent composition grid. Displayed at native resolution — `texture_filter = NEAREST`, consistent with Section 5.4.

**Visible area per visit:** 3–4 tiles wide × 2–3 tiles tall, arranged in a fixed compositional grid behind the NPC. Total: 6–9 tiles drawn from that restaurant's tile set.

**Dithering (from Section 3):** Apply 1–2px dithering at the vertical seam where ambiance zone meets UI overlay layer. Within tiles: wall textures, wood grain, and plaster use 2–3px dithering clusters to simulate material texture. This is the primary form of surface detail — not painted complexity, but dithered material language.

**How Warung Siang enters through tiles (from Section 4):**
- Tier 3 (warung) tiles: Warung Siang at full saturation — primary carrier of the Visiting Phase warmth
- Tier 2 (mid-range) tiles: Warung Siang at 60–70% saturation
- Tier 1 (high-end) tiles: Warung Siang at 20–30% — warmth as trace, not statement

The Visiting Phase palette shift reads differently per tier. Visiting a warung feels noticeably warmer than visiting a fine dining restaurant — produced entirely through tile color, no UI behavior change required.

---

### 6.2 Restaurant Visual Identity Per Tier

Each tier must be immediately distinguishable by tile composition alone — before the player reads any name, price, or description.

**Tier 1 — Fine Dining / High-End**
*Visual thesis: This place spent money on surfaces. Every surface says so.*
- Architecture: Clean plaster or tile walls with deliberate hue (off-white, sage, warm grey). Geometric tile patterns. Pendant lighting at tile-top edge.
- Texture: Smooth and regular. Dithering minimal — highlight edges only. Uniformity is a luxury.
- Prop density: Low. 1–2 props per tile with deliberate space between them.
- Materials: Cloth napkins, ceramic/glass surfaces, dark-stained wood, 2px brushed metal accent. No raw/unfinished materials.
- Color: Warung Siang at 20–30% saturation. Cool-neutral or warm-grey dominant.
- *Pixel guidance:* If you can see grain or plaster texture across most of the tile, it is not Tier 1. Save dithering budget for lower tiers.
- *Pillar 4:* Restraint itself is the soul. "We have been doing this long enough to remove everything unnecessary."

**Tier 2 — Mid-Range / Standard Restaurant**
*Visual thesis: This place tried, and you can see the trying.*
- Architecture: Painted walls with visible age — minor crack, paint seam. Soft yellow or warm-white with slightly uneven dithering at paint edges. Posters or framed certificates at tile edges.
- Texture: Moderate dithering. Paint edges, tile grout lines (4px apart, 1px dark), subtle stain gradients.
- Prop density: Moderate. 2–3 props per tile. Condiments in cluster (1–2px bottles), framed menu, seasonal decoration.
- Materials: Formica/laminate table surfaces (flat color, hard edge). Plastic chairs at tile bottom. Fluorescent tube at tile top as thin white rectangle. Stainless steel counter edge.
- Color: Warung Siang at 60–70% saturation. Fluorescent tube provides a cooler value contrast at the upper tile register.
- *Pillar 4:* The soul of Tier 2 is in the trying — the framed award slightly crooked, the wall repainted but not perfectly. Every imperfection is legible data about a business that cares but operates under constraint.

**Tier 3 — Warung / Street Food**
*Visual thesis: Every surface has a history of use, and the history is useful.*
- Architecture: Exposed/stained concrete, raw wood with visible grain, corrugated metal or plastic tarpaulin at tile edge. No architectural finish — the material IS the surface. Layers of different eras visible.
- Texture: Maximum dithering budget. Concrete, wood grain, rust marks, grime at corners — all via 2–3px dithering clusters.
- Prop density: Dense. 3–4 props per tile. Thermal flask, hanging plastic bags (2px silhouettes), stacked bowls, cable via tape, a fan at tile edge.
- Materials: Unpainted concrete block (dithered grey with warm undertone), raw/painted plywood, plastic resin chairs (single flat color, 3px), aluminium implements at counter height.
- Color: Warung Siang at full saturation (28–38°). Open-air afternoon light as dominant source — warm, horizontal, slightly overexposed at right tile edge.
- *Pillar 4:* The most visible history of any tier — layers of repair, objects moved and left where they landed, surfaces cleaned ten thousand times.
- *Pillar 1:* Visiting a warung has economic weight. Its margins are thin; a bad review carries outsized consequence relative to revenue. The tile density and warmth should create sympathy before the checklist begins.

---

### 6.3 Environmental Storytelling Guidelines

**Core constraint:** No scrolling tooltips, no lore text in tiles, no environmental popups. Every story detail delivered through what a 48×48px tile at 16 colors can render.

**Maximum density rule:** No single tile tells more than one story. Each tile carries one signal — either age OR newness OR success OR struggle OR character-specific. Tile combinations tell compound stories; individual tiles provide a single, legible note.

**Signal categories:**

*Age ("this place has been here 20 years"):*
- Stain gradients at wall-floor seam (dithered brown-grey, bottom 6px of adjacent wall tile)
- Mismatched tile repair — 3×3px area within a regular tile pattern using a slightly different value
- Paint layers at door frame: 2px edge of previous color beneath current
- Calendar showing a year (single digit sufficient at this resolution)
- Patina on metal: dithered rust-orange at fixture corners only, not broadly
- Worn counter edge: leading edge 1px lighter than counter surface — polish from repeated contact

*Newness ("this opened recently"):*
- No staining at wall-floor seam
- Tile grout visibly white, not grey
- Single printed menu in new plastic holder (2×4px, Layar Pagi highlight)
- Chairs all same color (older establishments accumulate variation)
- QR code on wall (4×4px abstract representation)

*Success ("this place is doing well"):*
- Small potted plant at tile edge (3px of organic green at corner)
- Wall art that is decorative, not an achievement certificate
- Updated equipment visible: newer-model appliance silhouette, LED strip instead of tube light

*Struggle ("business is difficult"):*
- Empty display case (case present, interior dithered grey — no product)
- Faded promotional material (color temperature shifted warm-grey vs full saturation)
- Broken light (fluorescent tube with missing pixel at center, uneven brightness dithering)
- Condiment bottles nearly empty (pixel-level fill level visible in bottle silhouette)

*Character-specific ("the owner's personality lives in this space"):*
Each restaurant's object signature tile must contain one character-specific detail aligned with the NPC's design. If the owner wears a baseball cap: a row of caps on wall hooks (3px each). These connections should be discoverable — not labeled, not highlighted.

*Pillar 4 — Restoran Punya Jiwa:* The soul is not in the menu. It is in the broken light nobody replaced yet, and the calendar from 2018 still on the wall because removing it would feel wrong.
*Pillar 3 — Reviewer Bukan Dewa:* Environmental storytelling gives enough information to feel sympathy or suspicion before the checklist — then forces rating by criteria anyway. The broken light doesn't change the food score.

---

### 6.4 Phase Background Contexts

**Non-Visiting phases = feed contexts.** The player is at a screen, not in a restaurant. Background serves feed aesthetic, not architectural atmosphere. No ambiance tiles appear outside the Visiting Phase.

**Planning Phase:** Layar Pagi (#F5F7FA). No environmental element. Optional: 2–3px random single-pixel scatter at 4% Aspal Malam opacity, tiled 64×64px — produces subtle "phone screen grit." MVP-defer unless pure white reads too flat.

**Publishing Phase:** Layar Pagi pushing toward pure white. No new environmental element. Screen-grit disappears here (brightness increase removes it) — correct, as Publishing is the most overexposed phase.

**Bill Paying Phase:** Layar Pagi at clinical near-white. Desaturated food photo thumbnails at periphery (same assets, reduced size/saturation — no new production). Optional: 4–6% brightness darkening at four screen corners as a static 8px feathered overlay — "layar yang redup karena terlalu lama dilihat." Defer to Vertical Slice pending full UI layout confirmation.

**Main Menu / Between Runs:** Layar Pagi with +4 to +6° warm shift. Archived food photo thumbnails (15% opacity warm tint overlay). Optional: single desaturated ambiance tile from most recently visited restaurant at 20–25% opacity behind the "Start Run" button zone — grounds the retrospective mood from Section 2.6. Defer to Vertical Slice.

*Pillar 2 — Rutinitas yang Menyerap:* The near-absence of environmental art during non-Visiting phases is intentional. When a restaurant ambiance tile appears, the player knows they are in Visiting Phase — without a UI label.

---

### 6.5 Asset Reuse Strategy

**Three-pool system:**

| Pool | Contents | Count | When produced |
|---|---|---|---|
| Unique tiles | Wall signature + object signature per restaurant | 30 tiles (2 × 15) | Per restaurant |
| Tier shared pool | 6 tiles per tier × 3 tiers | 18 tiles | Once per tier |
| Universal shared pool | Ceiling strips, neutral floor edges, counter base surfaces | 10 tiles | Once |

**Total: 58 tiles.** At ~1.5–2 hours per tile, approximately 85–115 hours of tile production. Feasible within a 3–5 week environment production window at 4–6 hours per day.

**Variation within shared tiles (zero new production):**
1. **Palette swap:** Same tile re-exported with different plaster/surface hue (2px hue shift). Each restaurant in a tier can have a distinct wall tone from the same texture pattern.
2. **Horizontal flip:** For tiles without directional elements (window light, posters), flipping doubles visual variety at zero cost. Never flip tiles with directional props.

**Tiles that must NOT be shared:** Wall signature tile, object signature tile, any tile containing character-specific storytelling detail from Section 6.3.

**MVP shortcut:** All MVP restaurants are Tier 3. Only Universal pool (10) + Tier 3 shared (6) + 10 unique tiles (2 per 5 restaurants) = **26 tiles for MVP.** Tier 1 and Tier 2 tile sets defer entirely to Vertical Slice.

**Animation budget: zero.** All ambiance tiles static. Movement would compete with the NPC's 2-frame breathing loop for attention — and the NPC loop is itself optional in MVP.

**Tile naming convention:**
- Unique: `env_[restaurant-slug]_wall_48.png` / `env_[restaurant-slug]_object_48.png`
- Tier shared: `env_tier[1/2/3]_[surface]_[variant]_48.png` (e.g. `env_tier3_wall_plaster_a_48.png`)
- Universal: `env_shared_[surface]_[variant]_48.png` (e.g. `env_shared_ceiling_strip_48.png`)

*Pillar 2:* The shared tile pool is also a narrative consistency system. The same plaster tile appearing across multiple Tier 3 restaurants creates subconscious recognition — these places exist in the same world. Repetition is atmosphere, not laziness.

---

### Environment Consistency Check

| Decision | Pillar served | Solo-dev achievable? |
|---|---|---|
| 48×48px tiles, fixed grid | — (technical efficiency) | Yes — consistent with NPC sprite unit |
| 2 unique tiles per restaurant + shared pools | P4 — identity without full unique set | Yes — 58 tiles total, phased |
| Tier warmth ladder (T3 full / T2 60-70% / T1 20-30%) | P4 — soul in material temperature | Yes — one palette rule per tier |
| Dithering at tile borders and surface textures | Section 3 — organic content vs angular UI | Yes — 2–3px dithering, no filter |
| Max one storytelling signal per tile | P4, P3 — legible, not illustrated | Yes — discipline rule, reduces overwork |
| No ambiance tiles in non-Visiting phases | P2 — feed IS the environment | Yes — less production, not more |
| Object signature tile has character-specific detail | P4 — soul through owner detail | Yes — 1 discoverable detail per restaurant |
| Zero animation | P2 — contemplative stillness | Yes — eliminates entire production category |
| MVP = Tier 3 only (26 tiles) | Scope — validates loop before full art | Yes — defers 32 tiles to Vertical Slice |

---

## 7. UI/HUD Visual Direction

*This section serves the Visual Identity Statement: the HUD is the feed. Every screen is a social media screen in a different state of use — browsing, composing, posting, reviewing stats. There is no separate overlay layer; UI and content are the same surface.*

---

### 7.1 HUD Composition Philosophy

The game has no traditional HUD. There is no minimap, no floating health bar, no world-space overlay. All information is presented as panels, cards, counters, and feeds — the same containers a food blogger uses to organize their work.

**Three persistent elements across all non-Game-Over phases:**

1. **Month Indicator** — top-left, Zone A. Format: `BULAN 03 / 12`. Monospaced numerals (Slot B). Functions identically to a "post N of 12" story counter.
2. **Follower Counter** — top-right, Zone A. Person-silhouette glyph prefix + numeral in Slot B, Aspal Malam. Never animated mid-phase; updates only at phase transitions.
3. **Current Balance Chip** — persistent small format, bottom-right of Zone A or Zone C depending on phase. Format: `Rp 1.250.000` (Indonesian period separator). Slot B numerals in state-semantic color (Foto Hijau / Amber Kritis / Saldo Merah). Glyph prefix: `!` (warning) or `!!` (danger) prepended to `Rp`. In Bill Paying phase, superseded by the full-width Balance Panel (see 7.4).

Everything else is phase-specific. Phase transitions are instantaneous swaps — no slide, no fade, no tween.

**Three-zone screen layout:**

- **Zone A (top bar, ~48px):** Month Indicator (left) + Follower Counter (right). Always visible.
- **Zone B (main content area):** Phase-dependent. Restaurant grid, food photo + checklist, balance panel, or run archive. Occupies the vertical majority.
- **Zone C (action bar, ~64px):** Phase-dependent. Primary action button(s). Bottom-anchored. Collapses if empty in a given phase.

No zone contains decorative content. Dead space is not reserved.

**Saturation lever — text exemption rule:** The global CanvasModulate desaturation shader applies to fills, borders, photo tints, and decorative elements only. All body text in Aspal Malam is exempt — text color values are set to full Aspal Malam regardless of the global saturation value. Functional text must remain legible in every phase state, including Bill Paying (15–25%) and Game Over (~5%). Implement by drawing all Label nodes on a separate CanvasLayer above the CanvasModulate node, or by restricting the modulate to content/environment CanvasLayers only.

---

### 7.2 Phase-by-Phase Screen Composition

#### Planning Phase

**Social media analog:** Feed browsing — scrolling a "to-visit" queue before deciding which restaurant to cover.

**Zone A:** Month Indicator (left). Follower Counter (right).

**Zone B:** Restaurant grid. 2-column layout, slight card height variation (±1 unit per card per Section 3 grid rules). **Each card contains: food photo thumbnail (TextureRect, fixed aspect ratio) + restaurant name label below the photo.** No cost data, no tier indicator on the card surface. The player chooses by feel and visual impression — the food photo is the primary decision-making signal. A "visited this run" indicator (small Foto Hijau checkmark badge, top-right of card, per Section 3 badge rules) appears only for previously visited restaurants. No other badge in Planning Phase. The grid is the only scrollable element in the game.

**Zone C:** Budget overview strip (informational, not a button). Single row: `Sisa Bulan Ini: Rp [X]` in Slot B + state-semantic color. Gives overall budget position without per-card cost data. The `KUNJUNGI` button also lives in Zone C and activates only when a card is selected (selected state: 2px Notifikasi border on card container, thumbnail at immediate 1.05× scale).

**Primary focal element:** Food photo on the selected card.

**Hidden:** Checklist, balance panel, star control, badge overlays.

---

#### Visiting Phase

**Social media analog:** Composing a review — at the location, evaluating the meal before writing.

**Zone A:** Month Indicator (left). Follower Counter (right).

**Zone B:** Two-column split (~55/45, left-heavy).
- **Left column:** Food photo (TextureRect, full column height). 100% saturation, no decorative border — fills to the column edge. Restaurant name in Slot A body weight below the photo.
- **Right column:** NPC panel (top ~20%, fixed TextureRect, optional 2-frame breathing) + Checklist panel (middle ~60%) + Overall Star Rating control (bottom ~20%, above Zone C).

**Zone C:** `SELESAI EVALUASI` confirm button. Inactive until all checklist rows are confirmed AND the overall star rating is set.

**Notification deferral rule:** Any notification banner received during Visiting Phase is queued and displayed at the Planning Phase of the following month — not mid-evaluation. Exception: game-state-critical events that end the current visit (restaurant closure mid-visit) surface immediately as an acknowledgment prompt.

**Primary focal element:** Food photo, left column.

**Hidden:** Restaurant grid, balance panel.

---

#### Publishing Phase

**Social media analog:** Hitting "post" — content is about to go live.

**Zone A:** Month Indicator (left). Follower Counter (right) — updates immediately after post confirmation.

**Zone B:** Food photo from Visiting Phase fills Zone B entirely. Over it: a semi-transparent overlay (Aspal Malam at ~40% alpha) with a centered review card preview (2px corner radius, Layar Pagi fill) showing: star badge (overall rating), restaurant name, three-line checklist summary, estimated engagement range (`~[X]–[Y] tayangan`).

At the moment of posting: 1-frame white-wash (full-screen ColorRect on CanvasLayer 100, white, alpha 1.0, one frame) fires then clears. The overlay disappears; the REVIEWED badge stamps onto the photo (2-frame pulse: 1.2× → 1.0×). Follower counter updates instantaneously.

**Zone C:** Single button — `POST`. 48px height, Notifikasi fill, white Slot A label, all caps. Only interactive element on screen. Activates one frame after the review card preview renders (prevents accidental double-click on phase entry).

**Primary focal element:** `POST` button, then badge stamp at confirmation.

**Hidden:** Checklist, restaurant grid, budget strip.

---

#### Bill Paying Phase

**Social media analog:** Monthly analytics and account management — checking numbers, paying dues.

**Zone A:** Month Indicator (left). Follower Counter (right) — updated count from this month's posts.

**Zone B:** Balance Panel, full width. Layout top-to-bottom:
- Header: `RINGKASAN BULAN [X]` — Slot A, small, all caps, letter-spaced, Aspal Malam.
- Gross income: `+ Rp [X]` — Slot B, Foto Hijau, medium.
- Fixed costs (up to 4 rows, e.g. sewa, makan, transport): `– Rp [X]` — Slot B, Aspal Malam, medium.
- Divider: 1px Aspal Malam horizontal rule (Saldo Merah tint if debt is active).
- Net balance: `Rp [X]` — Slot B, state-semantic color, largest text on screen (~1/8 of screen height). Glyph prefix `!!` if danger, `!` if warning.

Global CanvasModulate drops to 15–25% saturation on the main scene layer. All semantic financial colors (Foto Hijau, Amber Kritis, Saldo Merah) render on a separate UI CanvasLayer outside the modulate scope — full saturation retained. Effect: Zone A near-monochrome; balance numbers retain color. The persistent Balance Chip is hidden here.

**Zone C:** `LANJUT` button. Inactive for 1.5 seconds from screen entry (Timer node; no countdown animation — button simply becomes clickable after delay). Prevents accidental skipping of financial information.

**Primary focal element:** Net balance numeral.

**Hidden:** Restaurant grid, food photo, checklist, star control.

---

#### Game Over / Main Menu

**BANGKRUT (Game Over):** Full screen, near-monochrome (global saturation ~5%). Zone B center: final visit food photo (desaturated), overlaid by BANGKRUT badge at full size (see 7.6). Below photo: `BULAN [X] / 12` — Slot B, small, Aspal Malam. Below that: final follower count — Slot A, small. Zone C: `COBA LAGI` (Notifikasi fill) and `MENU UTAMA` (Notifikasi outline, no fill). Static. No animation.

**Main Menu / Run Archive:** Full saturation. Zone B: vertical feed of past run cards — each card shows best food photo + final month reached + peak follower count + badge strip (including BANGKRUT if applicable). Past run cards at reduced saturation with +8° warm shift (archived-post treatment, Section 2.6) — signals concluded, not active or in-progress. At the top of the feed, above all archive cards: the `+` creation card (see 7.5). Zone A: game title header. Zone C: absent; all actions embedded in Zone B cards.

**Primary focal element (BANGKRUT):** BANGKRUT badge, Saldo Merah, Zone B center.
**Primary focal element (Main Menu):** `+` new run card, top of feed.

---

### 7.3 Checklist UI Design

The checklist is the primary evaluation mechanic. It must feel like a review form native to a mobile food app while remaining legible without competing with the food photo in the adjacent column.

**Layout:** Vertical list of pill rows in the right column's middle zone. Each row is one criterion: Rasa, Pelayanan, Kebersihan, Harga (expandable by equipment upgrades). All rows uniform — equal height (~36px), equal width (full right-column width minus 8px side padding). Label length does not affect row height.

**Row anatomy (HBoxContainer):**
- **Criterion label** (~60% width, left-aligned): Slot A, all lowercase (`rasa`, `pelayanan`), Aspal Malam. Lowercase signals creator voice — personal notation, not bureaucratic form.
- **Criterion selector** (~40% width, right-aligned): 5-slot selector using filled/empty square glyphs (12×12px, 2px corner radius, matching shape grammar). Represents a per-criterion evaluation score that feeds the overall review quality calculation.

**Row states:**

| State | Background | Label opacity | Selector | Left border |
|---|---|---|---|---|
| Unrated | Layar Pagi | 70% Aspal Malam | All slots: outline, 40% Aspal Malam | None |
| Active/Focus | Layar Pagi | 100% Aspal Malam | Hovered: filled Notifikasi | 2px Notifikasi vertical accent |
| Confirmed | Layar Pagi + 8% Notifikasi tint | 100% Aspal Malam | Selected: filled Notifikasi | None |

The 2px Notifikasi left-border on the active row also serves as the **keyboard focus indicator** for this element — Tab-navigating through checklist rows shows this border without a separate focus ring. Functional, not decorative.

1px Aspal Malam bottom border on each row (except the last) is the only structural divider between rows.

**Godot implementation:** VBoxContainer of instanced HBoxContainer scenes. State changes: set StyleBoxFlat properties on each row's PanelContainer (bg_color, border_width_left, border_color). Selector slots: TextureButton nodes with custom theme (12×12px normal/pressed texture swap). All transitions instantaneous — no AnimationPlayer.

---

### 7.3.1 Overall Star Rating Control

**Position:** Below the checklist pill rows, above Zone C, within the right column. Separated from the checklist by a full-width 1px Aspal Malam rule.

**Design:** A single row (48px height — slightly taller than criterion rows at 36px, signaling summary status) with label left + 5-star selector right. Uses a filled ★ star glyph (20×20px) rather than the square slot used in criterion rows — the star shape distinguishes the overall rating from criterion selectors at a glance.

**Label:** `Penilaian Akhir` — Slot A, regular, Aspal Malam.

**Star glyphs:** 5 × ★ shapes. Selected: filled Notifikasi. Unselected: outline, Aspal Malam 50% alpha. Hover: cumulative fill from left (1–5 highlights all stars up to and including hovered star).

**Gate behavior:** `SELESAI EVALUASI` (Zone C) remains inactive until all checklist rows are confirmed AND this control has a set value (1–5).

**Keyboard navigation:** Tab enters this control after the last checklist row. Arrow left/right adjusts star count. Enter confirms. Focus state: 2px Notifikasi outer border on the containing row (consistent with checklist active row pattern).

*Design note:* The star rating is the player's editorial judgment, not a mechanical average of criterion scores. Two visits with identical checklist states can receive different star ratings — the gap is the reviewer's call. This serves Pillar 3 — the reviewer has judgment, not just a formula.

---

### 7.4 Financial Display Design

**Persistent Balance Chip (Planning, Visiting, Publishing phases):** Small format in Zone A or Zone C. Format: `Rp 1.250.000`. Slot B, regular, state-semantic color. Glyph prefix `!!` (danger) or `!` (warning) prepended to `Rp`. Same face, weight, and color for both `Rp` prefix and numeral — no typographic separation.

**Bill Paying large-format Balance Panel:** Net balance numeral is the largest text on screen (~1/8 screen height). Same Slot B face, same color rules, same glyph prefix logic. `custom_minimum_size` on the Label node prevents layout reflow when color state changes. Transition is instantaneous — no count-up animation. You refresh the screen and the number is different.

**Debt state:** Negative balance: Saldo Merah numeral, `!!` prefix, Saldo Merah tint on divider line. No additional visual layer — existing semantic color system handles it.

**Godot notes:** `horizontal_alignment = HORIZONTAL_ALIGNMENT_RIGHT` on all financial Labels. `use_separate_yscale = false` on Slot B Labels to prevent numeral height inconsistency.

---

### 7.5 Interactive Element Design

Notifikasi (255–265°) is the sole color for all interactive elements. No exceptions.

**Standard button:**
- Shape: 2px corner radius, min 80px width, 36px standard / 48px primary action height.
- Resting: Notifikasi fill, white Slot A label, all caps, +0.05em tracking.
- Hover: Notifikasi at ~85% brightness. Label white. No size change, no glow.
- Pressed: Notifikasi at ~70% brightness. Instantaneous.
- Disabled: Aspal Malam fill at 30% opacity, label at 50% opacity. Absence of blue = inactive.

**Keyboard focus (buttons and non-checklist interactive elements):** A 2px outer rule drawn 2px outside the element's bounding box in full-opacity Aspal Malam. Distinct from the Notifikasi hover/press state. Implemented as a focused StyleBox variant with `expand_margin_all = 2` and `border_width_all = 2`. Explicitly exempt from the "no ornamental borders" rule in Section 3 — this is a functional accessibility element.

**Card selection (Planning Phase):** 2px Notifikasi border on the card container + immediate 1.05× thumbnail scale. Keyboard and mouse selection share the same visual state — Tab cycles grid cards, Enter activates. No separate focus ring needed.

**`POST` button (Publishing Phase):** Standard primary button. Activates one frame after review card preview renders. Only interactive element on screen — importance conveyed by context, not special treatment.

**`+` new run card (Main Menu):** Top slot of the run archive feed. Same card proportions as archive cards but: Layar Pagi body, centered `+` glyph in Notifikasi (Slot A body weight), label below: `Mulai Blog Baru` — Slot A, regular, Aspal Malam. Diegetic label grounds the action in the social media metaphor while communicating roguelike restart. Hover: standard 2px Notifikasi border.

---

### 7.6 Badge and Overlay System

Badges are flat, rectangular (2px corner radius), opaque digital stamps. Uniform shape across all types — differentiation through fill color, label text, and scale only. No starburst, no circle, no shield.

**Base anatomy:** Fill color, 2px corner radius, white Slot A label in bold weight (the only context in the game where bold is used), all caps, +0.03em tracking. Width: content-driven, minimum 48px. Height: 20px standard, 28px for BANGKRUT.

**Placement:** Always top-left or top-right of the parent card's photo area. Never centered, never bottom. Maximum two badges per card (one per corner). If a third state must be communicated, update an existing badge rather than adding a third.

| Badge | Fill | Label | Position | Notes |
|---|---|---|---|---|
| REVIEWED | Aspal Malam | `REVIEWED` | Top-left | Applied after completed visit |
| ★ [N] | Aspal Malam | `★ 3` | Top-right | Star glyph + numeral, white; overall rating display |
| VIRAL | Notifikasi | `VIRAL` | Top-right | Replaces ★ badge position when active |
| BANGKRUT | Saldo Merah | `BANGKRUT` | Zone B center | Game Over exception — see below |

**Publishing Phase badge animation:** Frame 1: badge at 1.2× scale. Frame 2: badge at 1.0× (one frame later). Hard frame swap — 2-keyframe AnimationPlayer or `await get_tree().process_frame`. If VIRAL fires after REVIEWED: sequential pulses, one frame apart.

**BANGKRUT — UI layer exception:** Occupies Zone B center as a full-panel-width badge. Rendered on CanvasLayer 10, above CanvasModulate (Layer 0). Full Saldo Merah at ~5% global saturation. No animation — static on Game Over screen load. The only saturated element in the game at this state.

**Godot:** All badges: Label inside PanelContainer with StyleBoxFlat (fill color, 2px radius, no border). BANGKRUT on CanvasLayer 10. Star badge built from a single Label template with text set at runtime.

---

### 7.7 Typography Direction

**Two typeface slots. Adding a third is a violation of this section.**

**Slot A — Proportional Body Face:**
All labels, criterion names, restaurant names, button labels, section headers, general UI text.

Character: clean humanist or geometric sans-serif with mild warmth in the letterforms. Not a corporate grotesque. Should feel at home on an Indonesian food blog or product label — functional and legible with enough personality to feel human at small sizes.

Weight: Regular for body text. Bold reserved exclusively for badge text. No italic. No medium/semibold.

**Slot B — Monospaced Numerals:**
All financial figures, month indicator, follower count, engagement numbers, star badge numeral.

Character: tabular monospaced (all digits equal width — prevents lateral shift on value updates). Reads as receipt or banking interface, not terminal. Not a pixel font.

**No pixel font.** A pixel font reads as retro-game aesthetic, contradicting the feed-native identity established in Section 1.

**Size hierarchy:**

| Element | Slot | Target size | Weight |
|---|---|---|---|
| Net balance numeral (Bill Paying) | B | ~48–64px | Regular |
| BANGKRUT badge | A | 18px | Bold |
| Section headers | A | 14px | Regular, all caps, +0.05em |
| Restaurant name / criterion labels | A | 12–13px | Regular |
| Button labels | A | 12px | Regular, all caps, +0.05em |
| Month indicator / follower count | B | 12px | Regular |
| Badge labels | A | 10px | Bold, all caps |
| Persistent balance chip / engagement range | B | 11px | Regular |

Minimum rendered text size: **10px** at final display resolution. If UI scaling is supported, all text scales linearly — no secondary small-text face.

**Rendering (Godot 4.6):** Vector font rendering via built-in Label. `use_mipmaps = false`. Hinting: `HINTING_NORMAL` for Slot A, `HINTING_NONE` for Slot B (prevents numeral-width inconsistency). No outline on body text. 1px Aspal Malam outline on Slot A text appearing over variable photo content (e.g., restaurant name on card).

**Independent creator marker:** Lowercase criterion labels (`rasa`, `pelayanan`) are the only departure from standard mixed-case or all-caps UI convention. This single typographic choice carries the system's personality without decorative treatment.

---

### 7.8 Notification and Milestone UI

**Notification banner:**

Position: enters from top edge of Zone B, settles at Zone B top, occupies full Zone B width as a ~40px strip. Exits back upward after 2.5 seconds. Full-width notification mimics a status-bar push notification covering the top of a phone feed.

Anatomy: Layar Pagi background, 1px Aspal Malam bottom border, icon glyph (16×16px, left), message text (Slot A, 12px, Aspal Malam, ellipsis on overflow), optional numeral (Slot B, 12px, right-aligned).

Examples:
- `[person-glyph] +1.200 follower baru`
- `[flame-glyph] Review kamu trending!`
- `[bell-glyph] Bulan baru dimulai`

Entry/exit: position offset -40px → 0px (enter), 0px → -40px (exit). Instantaneous (1-frame) — no tween. Social media notifications do not ease.

**Deferral queue:** Notifications generated during Visiting Phase are queued. Queue flushes at the start of the next Planning Phase — banners fire sequentially at 2.5-second intervals before the restaurant grid becomes interactive. This preserves the focused evaluation mood of Section 2.2.

**Godot implementation:** Panel in CanvasLayer 5 (above content, below BANGKRUT at Layer 10). Position and visibility set instantaneously. Timer drives the 2.5-second display duration. Queue is an Array of notification data dictionaries; flush logic runs at Planning Phase entry.

---

**Engagement updates:**

Follower count in Zone A updates at phase transitions only, instantaneously. No counter rollup. You refresh the page and the number has changed.

Engagement estimate in Publishing Phase preview (`~[X]–[Y] tayangan`) is a static calculated string — not live. Actual engagement reveals at the next Bill Paying income row.

---

**Milestone white-wash:**

Triggered by: `POST` confirmation, and any defined milestone (first viral post, 12-month clear).

Implementation: Full-viewport ColorRect on CanvasLayer 100 (highest layer). White, alpha 1.0. Frame 1: visible = true. Frame 2: visible = false. ~16ms at 60fps. Hard on, hard off — a seam, not a ceremony. Player's eye resets and finds the badge already placed, the follower count already updated.

---

**"Going Viral" event sequence:**

1. `POST` pressed → 1-frame white-wash fires and clears
2. Publishing Phase layout resumes with completed review card
3. REVIEWED badge stamps (2-frame pulse, top-left)
4. If viral: VIRAL badge stamps immediately after (2-frame pulse, top-right, one frame offset)
5. Notification banner enters: `[flame-glyph] Review kamu trending!`
6. Zone A follower counter updates (instantaneous)
7. `LANJUT` becomes available in Zone C

If not viral: step 4 skipped, step 5 shows neutral follower gain. No mandatory wait timers after step 7.

---

### Section 7 Consistency Check

| Decision | Serves Feed Aesthetic? | Solo-dev Producible? |
|---|---|---|
| HUD is feed content, not overlay layer | Yes — every screen is a social media screen state | Yes — no separate HUD system needed |
| Three persistent elements only (Month, Follower, Balance chip) | Yes — minimal chrome, content-forward | Yes — three static Label nodes |
| Three-zone layout (A/B/C) | Yes — mirrors story/feed structure (header/content/action) | Yes — three VBoxContainer regions |
| Restaurant cards: photo + name only | Yes — feed grid, content-first decision-making | Yes — minimal card content, no extra data nodes |
| Budget strip in Zone C, not on each card | Yes — status bar shows context; cards show content | Yes — one Label row in Zone C |
| Visiting Phase 55/45 column split (photo + checklist) | Yes — creator composing a review at location | Yes — HBoxContainer with two children |
| Checklist: uniform pill rows, lowercase labels | Yes — review form native to mobile apps | Yes — VBoxContainer of instanced HBoxContainer scenes |
| Three checklist row states via StyleBoxFlat swaps | Yes — form state clarity without animation | Yes — instantaneous property sets |
| 2px Notifikasi left-border as checklist focus indicator | Yes — feed-app active-item pattern | Yes — StyleBoxFlat border_width_left = 2, functional |
| Overall star rating: separate control below checklist | Yes — summary publish-rating is a distinct concept | Yes — one additional row scene |
| ★ glyph distinguishes overall rating from square criterion selectors | Yes — star = publish-ready rating language | Yes — texture swap, same HBoxContainer pattern |
| `SELESAI EVALUASI` gated on all checklist rows + star rating | Yes — prevents partial review submission | Yes — boolean check across row states + star control |
| Zone C `LANJUT` delay (1.5s) in Bill Paying | Yes — forces reading the analytics dashboard | Yes — single Timer node |
| Bill Paying: full Zone B balance panel, net balance ~1/8 screen height | Yes — analytics-screen-as-reckoning | Yes — Label with font_size override, VBoxContainer |
| Saturation lever exempt from all body text | Yes — feed readability at all phase states | Yes — one CanvasLayer split |
| Notifikasi blue = sole interactive color, no exceptions | Yes — platform color = interactive affordance | Yes — one color, one meaning |
| Keyboard focus: 2px offset outer rule in Aspal Malam | Yes — functional, invisible to mouse users | Yes — separate focused StyleBox variant |
| `POST` activates 1 frame after preview renders | Yes — prevents accidental double-click without breaking flow | Yes — single deferred call or `await process_frame` |
| `+` card labeled `Mulai Blog Baru` | Yes — creation-language native to the social media metaphor | Yes — string constant on the card Label |
| Archive cards at reduced saturation + warm shift | Yes — "past, not active" archived-post treatment | Yes — semi-transparent warm tint overlay |
| BANGKRUT on CanvasLayer 10, above CanvasModulate | Yes — full red isolation from global desaturation | Yes — one additional CanvasLayer node |
| Badge: flat 2px radius rectangle, white label, bold | Yes — digital overlay stamp, not physical | Yes — one StyleBoxFlat template per badge type |
| 2-frame badge pulse only (1.2× → 1.0×) | Yes — digital stamp "thunk" at moment of posting | Yes — 2-keyframe AnimationPlayer or `await process_frame` |
| Notifications deferred from Visiting Phase; flushed at Planning | Yes — "you check notifications when you pick up your phone" | Yes — Array queue + flush at phase transition |
| Follower count updates instantaneous at phase transition | Yes — "you refreshed the page" model | Yes — set Label text at transition, no tween |
| Engagement estimate: static string, not live counter | Yes — analytics report, not live feed | Yes — calculated once, displayed as string |
| White-wash: 1-frame ColorRect on Layer 100 | Yes — photographic overexposure at peak moment | Yes — single ColorRect node, two-line toggle |
| Two typeface slots only (Slot A proportional + Slot B monospaced) | Yes — social media uses one or two system fonts | Yes — two font resources, theme-applied |
| No pixel font | Yes — feed-native identity, not retro-game | Yes — eliminates pixel font tooling entirely |
| Bold weight only on badge labels | Yes — badges are emphasis objects; body is reading text | Yes — single FontVariation weight override |

---

## 8. Asset Standards

*This section translates all visual decisions from Sections 1–7 into production-level rules: naming, canvas specs, color budgets, Godot import settings, scene architecture, palette enforcement, and the MVP production shortlist. The two halves (art production and technical pipeline) are merged here and must be read together.*

---

### 8.1 File Naming Convention

All assets follow the pattern: `[category]_[descriptor]_[variant/state]_[size].[ext]`

Segments are lowercase, separated by underscores. No spaces. No camelCase. Abbreviations are fixed — do not improvise new ones.

**Category prefixes:**

| Category | Prefix |
|---|---|
| Food photo tile | `food` |
| Environment tile | `env` |
| NPC sprite | `npc` |
| Player avatar | `plr` |
| Player hand/phone | `hand` |
| UI element (raster) | `ui` |
| Font resource | `fnt` |

*Badges have no category prefix — they are code-driven Control nodes, not imported image assets. See Section 8.9.*

**Food photo tiles:** `food_[dish]_[tier]_64.png`
- `[dish]` — romanized Indonesian slug, max 16 chars (e.g., `nasigoreng`, `bakso`, `miegoreng`)
- `[tier]` — temperature tier: `t1`, `t2`, or `t3`
- Size suffix always `64` (64×64px canvas)

Examples: `food_nasigoreng_t1_64.png`, `food_bakso_t3_64.png`

**Environment tiles:** `env_[pool]_[object]_[variant]_48.png`
- `[pool]` — `uniq` / `shared` / `univ`
- `[object]` — object slug, max 12 chars
- `[variant]` — numeric `01`–`99` or short descriptor (`a`, `b`, `clean`, `dirty`)

Examples: `env_uniq_kursi_01_48.png`, `env_shared_meja_dirty_48.png`, `env_univ_lantai_a_48.png`

**NPC sprites:** `npc_[archetype]_[id]_[state]_32x48.png`
- `[archetype]` — `owner`, `chef`, or `rival`
- `[id]` — `01`–`99` per archetype (not globally unique)
- `[state]` — `idle`, `breathe01`, `breathe02`, `pleased`, `tense`

Examples: `npc_owner_01_idle_32x48.png`, `npc_chef_02_tense_32x48.png`

**Player sprites:**
- Avatar: `plr_avatar_[id]_24x24.png` (e.g., `plr_avatar_01_24x24.png`)
- Hand/phone: `hand_[state]_48x32.png` (states: `hold`, `shoot`, `review`, `scroll`)

**UI raster elements** (icons, glyphs — only when not covered by the typeface):
`ui_[component]_[variant]_[state].png`
- Component slugs: `icon`, `glyph`, `bar`, `divider`
- State: `default`, `hover`, `pressed`, `disabled`, `active`

Examples: `ui_glyph_down_default.png`, `ui_glyph_warn_default.png`, `ui_glyph_check_default.png`

**Font resources:** `fnt_[slot]_[weight].[ttf|otf]`
- Slot: `a` (proportional body) or `b` (monospaced numerals)
- Weight: `regular`, `bold`

Examples: `fnt_a_regular.ttf`, `fnt_b_regular.ttf`, `fnt_a_bold.ttf`

---

### 8.2 Canvas and Export Standards

#### Food Photo Tiles (64×64px)

| Property | Value |
|---|---|
| Canvas size | 64×64px |
| Export format | PNG-32 |
| Alpha channel | Required — 1px transparent border enforced (see below) |
| 1px transparent border | Required on all four sides. Dish content lives within 62×62px inner area. Prevents NEAREST filter color bleed when tiles are placed adjacent. |
| Bleed/margin | None beyond the transparent border |

#### Environment Tiles (48×48px)

| Property | Value |
|---|---|
| Canvas size | 48×48px |
| Export format | PNG-32 |
| Alpha channel | Required — TileMap compositor needs alpha channel for layering |
| 1px transparent border | Required on all four sides. Visible content within 46×46px. Non-negotiable at NEAREST filter. |
| Bleed/margin | None |

#### NPC Sprites (32×48px)

| Property | Value |
|---|---|
| Canvas size | 32×48px |
| Export format | PNG-32 |
| Alpha channel | Required — NPCs composite over environment layer |
| 1px transparent border | Required on left and right edges. Top: 2px transparent minimum (headwear must not touch the topmost pixel row). Bottom: 1px. |

#### Player Avatar (24×24px)

| Property | Value |
|---|---|
| Canvas size | 24×24px |
| Export format | PNG-32 |
| Alpha channel | Required — circular crop applied at runtime; square canvas corners must be alpha 0 |
| 1px transparent border | Required on all sides. Visible face content within 22×22px inner area. |

#### Player Hand/Phone (48×32px)

| Property | Value |
|---|---|
| Canvas size | 48×32px (landscape) |
| Export format | PNG-32 |
| Alpha channel | Required — composites over food photo in Visiting Phase |
| 1px transparent border | Required on all sides |

#### UI Raster Elements (icons, colorblind glyphs)

| Property | Value |
|---|---|
| Canvas size | Icons: 16×16px. Colorblind glyphs: 8×8px standard / 12×12px for large contexts |
| Export format | PNG-32 |
| Alpha channel | Required |
| 1px transparent border | Required for icons. Not required for 1×1px tiling fills. |

**General export rules (all types):**
- Always PNG. No JPEG, no WebP, no interlacing.
- Never use "save for web" lossy export options.
- Color profile: sRGB, no embedded ICC profile.
- Strip all metadata (comments, author fields) before committing.

---

### 8.3 Color Budget Per Asset Type

Color budget is a hard ceiling on distinct RGBA values in the exported PNG, excluding fully-transparent pixels (alpha 0).

| Asset type | Color budget | Notes |
|---|---|---|
| Food photo tiles | 16 colors (24 max permitted) | Food-only color language — named palette colors must NOT appear in food tiles |
| Environment tiles | 12 colors max | Universal pool tiles: 8 colors max (must read across all tier contexts) |
| NPC sprites (32×48px) | 16 colors max | 3 skin values + clothing + Warung Siang on food pixels only + headwear accent + outline |
| Player avatar (24×24px) | 8 colors | 2-3 skin values + hair + eye + clothing + outline (per Section 5) |
| Player hand/phone (48×32px) | 10 colors | Skin must match avatar skin tone set exactly |
| UI chrome elements | Named palette only | 7 named colors + white (Layar Pagi) + dark (Aspal Malam) — no additions |
| Colorblind glyph icons | 3 colors max | Glyph color + background color + transparent |

**Strict Warung Siang rule:** Warung Siang (28–38° warm amber-orange) may only appear in food photo tiles, environment tiles (as ambient warmth per Section 6.1), and NPC sprites when the pixel represents literal food content (a bowl being carried, steam from a dish). It must not appear in UI chrome, badges, or non-food NPC details. Any warm amber-orange pixel in a UI asset is an error.

**Strict Notifikasi rule:** Notifikasi (255–265° electric blue-violet) may only appear in UI interactive elements and badge fills (VIRAL badge). It must not appear in any environment tile or NPC sprite.

---

### 8.4 Per-Asset Production Checklist

Apply this checklist before committing any asset. A "no" on any item is a blocking issue.

**Universal checklist (all asset types):**
```
[ ] 1. File name matches Section 8.1 convention exactly.
[ ] 2. Canvas dimensions match Section 8.2 spec for this asset type.
[ ] 3. Export format is PNG-32 (or PNG-8 only where explicitly permitted).
[ ] 4. Alpha channel correct: transparent areas are alpha 0, not near-transparent.
        No anti-aliasing fringe pixels (50-200 alpha) on shape edges.
[ ] 5. 1px transparent border is intact on all required edges.
        Zoom to 1600% and verify every border pixel is alpha 0.
[ ] 6. No anti-aliased pixel edges. Every edge pixel is alpha 0 or alpha 255.
[ ] 7. Color count is within budget for this asset type (Section 8.3).
[ ] 8. All colors are authorized for this asset type.
        UI chrome: named palette only. NPCs: approved skin tones + permitted accents.
        Food tiles: food-only color language (no named palette contamination).
```

**Food photo tiles (additional):**
```
[ ] 9.  No named palette color (Layar Pagi, Notifikasi, Saldo Merah, etc.) appears.
[ ] 10. Dish content contained within 62×62px inner area (not touching 1px border).
[ ] 11. Temperature tier is correct: T1=warm, T2=neutral, T3=cool/mixed.
```

**Environment tiles (additional):**
```
[ ] 9.  Notifikasi is absent.
[ ] 10. Warung Siang appears only on pixels depicting literal food content.
[ ] 11. Primary object is identifiable at 100% zoom (no magnification).
[ ] 12. Max one storytelling signal per tile (per Section 6.3).
```

**NPC sprites (additional):**
```
[ ] 9.  Notifikasi is absent.
[ ] 10. Warung Siang absent except on food-representing pixels.
[ ] 11. Archetype differentiator readable at 32×48px:
         Owner: headwear silhouette present. Chef: hand state active. Rival: phone angle present.
[ ] 12. Skin tone values match one of the three approved skin tone sets.
```

**UI chrome elements (additional):**
```
[ ] 9.  Warung Siang is absent.
[ ] 10. Only named palette colors present.
[ ] 11. Shape grammar correct: 2px outer radius, 0px inner radius.
[ ] 12. Interactive elements use Notifikasi. Static elements use Aspal Malam or Layar Pagi.
```

---

### 8.5 Colorblind Safety Production Standards

#### The Canonical Glyph Set

Color is never the only signal. Every color-coded state requires a non-color glyph backup. The four canonical glyphs:

| Glyph | State | Accompanies color |
|---|---|---|
| Downward arrow (↓) | Deficit / negative trend | Saldo Merah |
| Exclamation mark (!) | Warning / critical threshold | Amber Kritis |
| Checkmark (✓) | Safe / positive state | Foto Hijau |
| Stable line (—) | Neutral / no change | Aspal Malam |

**Glyph sizes and production method:**

| Context | Glyph size | Method |
|---|---|---|
| HUD financial readout | 8×8px (as font character) | Runtime: Slot B font Unicode character. Verify Slot B font includes ↓ ! ✓ — before committing to this approach. If absent, substitute baked icon. |
| Bill Paying summary | 12×12px | Runtime font character at larger font size |
| UI bar state indicator | 8×8px baked icon | Separate PNG asset (`ui_glyph_down_default.png` etc.) — baked because bar alignment requires pixel precision |

**Glyph pixel construction (for baked icons at 8×8px):**
- Downward arrow: 3px-wide chevron pointing down, 1px stem above it. Total: 5px tall. Must not read as a minus sign.
- Exclamation mark: 1px wide, 1×3px stem + 1px gap + 1×1px dot. Total: 5px tall.
- Checkmark: 3-pixel rising diagonal, 3-pixel falling diagonal. Total: ~5×4px. Fits in 8×8 with 1px padding.

**Glyph color rule:** White or Layar Pagi on Saldo Merah/Amber Kritis/Notifikasi fills. Aspal Malam on Foto Hijau or Layar Pagi fills. Minimum 4.5:1 contrast ratio required.

#### Solo Dev Verification Process (in order)

1. **Grayscale conversion check.** Convert asset to grayscale. Every semantically distinct state (safe/warning/danger) must be distinguishable by lightness value alone, without color.
2. **Glyph presence audit.** For every asset using Saldo Merah, Amber Kritis, or Foto Hijau: verify the corresponding canonical glyph is visible at 100% game scale (not zoomed-in authoring view).
3. **Simulation tool check.** Run the exported PNG through a colorblind simulation tool (Coblis or equivalent). Check deuteranopia, protanopia, tritanopia. Required for all badge-type UI and HUD assets. Recommended but not required for individual food tiles.
4. **No-color-name test.** Describe the asset state out loud without using color words. If you cannot describe the state without naming a color, the "color is never the only signal" rule has not been implemented.

**Per-asset colorblind requirement:**

| Asset type | Required measure |
|---|---|
| Food photo tiles | None — tiles are aesthetic, not game-state-communicating |
| Environment tiles | None — environment does not communicate game state |
| NPC sprites | None — archetypes differentiated by shape, not color |
| UI financial readouts | State glyph required (runtime font character or baked icon) |
| UI buttons | Disabled state: reduced opacity (50%) in addition to color change |
| BANGKRUT badge text label | Text "BANGKRUT" is the primary signal; Saldo Merah fill is reinforcement |

---

### 8.6 MVP Production Shortlist

MVP = 3-month survival loop, 5 Tier-3 restaurants.

**Blocking (game cannot be playtested without these):**

Environment foundation (5 of 26 MVP tiles; remainder use Godot ColorRect placeholders):
- `env_univ_lantai_01_48.png`
- `env_univ_tembok_a_48.png`
- `env_univ_pintu_01_48.png`
- `env_shared_meja_clean_48.png`
- `env_shared_kursi_01_48.png`

NPC sprites (one per archetype to test NPC system):
- `npc_owner_01_idle_32x48.png`
- `npc_chef_01_idle_32x48.png`
- `npc_rival_01_idle_32x48.png`

Player sprites:
- `plr_avatar_01_24x24.png`
- `hand_hold_48x32.png`
- `hand_shoot_48x32.png`

Food photo tiles (minimum to test temperature system and saturation lever):
- One T1 tile: `food_[dish]_t1_64.png`
- One T2 tile: `food_[dish]_t2_64.png`
- One T3 tile: `food_[dish]_t3_64.png`

UI glyph icons (colorblind safety minimum):
- `ui_glyph_down_default.png` — danger state indicator
- `ui_glyph_warn_default.png` — warning state indicator

Font resources:
- `fnt_a_regular.ttf` + `fnt_a_bold.ttf`
- `fnt_b_regular.ttf`

**Non-blocking (use placeholder, validate loop first):**
- Remaining 21 environment tiles (Godot ColorRect in named palette colors)
- Owner variants `npc_owner_02` through `npc_owner_05` (duplicate `owner_01` with hue shift)
- NPC breathing loop frames (`breathe01`, `breathe02` for all archetypes)
- Remaining food photo tiles for all 5 restaurants
- `ui_glyph_check_default.png` (safe state — missing this causes false anxiety, not missed danger)

---

### 8.7 Art Direction Self-Review Checklist

Answer all 10 questions before committing any asset. A "no" requires revision.

```
[ ] 1. Feed aesthetic: Does this look like it belongs in a personal food blog or
        indie creator feed — not a corporate product or a physical notebook?

[ ] 2. Warm color containment: If this is UI chrome, badge, or environment tile,
        is Warung Siang (28-38° warm amber-orange) absent?

[ ] 3. Shape grammar: Do rounded corners match the spec — 2px outer, 0px inner?
        Is there any decorative curvature that wasn't in the brief?

[ ] 4. Visual weight: Does this element feel like the right weight for its role?
        Does it compete with elements that should be above it in the hierarchy?

[ ] 5. Color signal backup: If this communicates game state via color, is there
        a non-color signal (glyph, shape change, size change) present?

[ ] 6. NEAREST filter safety: Zoom to 400%. Are all edges fully hard —
        alpha 0 or alpha 255 only, no intermediate values?

[ ] 7. Color budget: Is the color count within budget (Section 8.3)?
        Can any two similar values be unified?

[ ] 8. Palette purity: Does this use only authorized colors for its type?
        UI chrome: named palette only. Food tiles: food-only color language.
        NPCs: approved skin tones + permitted accents.

[ ] 9. Naming and size: Is the file name exactly correct (Section 8.1)?
        Is the canvas size exactly correct (Section 8.2)?

[ ] 10. Solo dev gut check: Step away 5 minutes, then look at 100% game scale.
         Does it feel like it belongs in this game?
```

---

### 8.8 Godot Import Settings Per Asset Type

*Badges and UI chrome are composed from Godot Control nodes with StyleBoxFlat — they have no imported textures and are excluded from this section.*

**General principle:** All pixel art uses lossless compression and nearest-neighbor filtering. Lossy compression (S3TC/ETC2/BPTC) applies block-compression that destroys sub-pixel color boundaries — unacceptable for a 7-color palette where a single incorrect pixel is immediately visible.

**Do not change the project-level default texture filter.** Set `texture_filter = NEAREST` on each individual node (TextureRect, Sprite2D, TileMap/TileMapLayer). This preserves default linear filtering for vector fonts and SVG assets globally. [VERIFY IN GODOT 4.6 DOCS — Confirm node-level `texture_filter` override behavior in 4.6, given rendering pipeline changes in 4.4+.]

**Food Photo Tiles (64×64px):**

| Setting | Value | Reason |
|---|---|---|
| `compress/mode` | Lossless | Preserves indexed-color palette exactly |
| `flags/mipmaps` | Off | At NEAREST filter, mipmaps cause bleeding artifacts at tile boundaries |
| `process/fix_alpha_border` | On | Prevents color fringing at transparent border edges |
| `process/premult_alpha` | Off | Enable only if tiles show dark halos in-engine |
| `texture_filter` | NEAREST (node-level) | Set on each TextureRect node |

**Environment Tiles (48×48px):**

| Setting | Value |
|---|---|
| `compress/mode` | Lossless |
| `flags/mipmaps` | Off |
| `process/fix_alpha_border` | Off (tiles are opaque within footprint) |
| `texture_filter` | NEAREST (TileSet or TileMapLayer node level) |

*TileSet note:* If tiles are imported into a TileSet resource, the filter setting on the TileSet's texture takes precedence over node-level settings. Verify the TileSet Inspector shows `texture_filter = NEAREST` per texture entry. [VERIFY IN GODOT 4.6 DOCS — In Godot 4.4+, TileMap was refactored into TileMapLayer. Confirm whether the TileSet texture filter is set on the TileSet resource or on the TileMapLayer node in 4.6.]

**NPC Sprites (sprite sheet, 32×48px cells):**

| Setting | Value |
|---|---|
| `compress/mode` | Lossless |
| `flags/mipmaps` | Off |
| `process/fix_alpha_border` | On |
| `process/premult_alpha` | Off |
| `texture_filter` | NEAREST (Sprite2D node level) |

**Player Avatar (24×24px):** Same as NPC sprites. Circular crop applied at runtime via ShaderMaterial (see 8.9).

**Player Hand/Phone (48×32px):** Same as NPC sprites.

**UI Raster Elements (icons, colorblind glyphs):** Same as NPC sprites — Lossless, no mipmaps, `fix_alpha_border` on.

---

### 8.9 Scene and Node Architecture for Asset Usage

**Food photo tiles in cards:** `TextureRect` node. Set `expand_mode` and `stretch_mode` to display at exactly 64×64 logical pixels without stretching. `texture_filter = NEAREST`. Cards (PanelContainer) handle layout sizing; TextureRect does not drive layout. [VERIFY IN GODOT 4.6 DOCS — `TextureRect.expand_mode` was reworked in Godot 4.x. Confirm the non-stretched display combination in 4.6.]

**Environment tiles:** Use **TileMap (or TileMapLayer in Godot 4.4+)** — not manually placed Sprite2D nodes. TileMap/TileMapLayer provides built-in grid snapping, a visual tile editor, batched rendering, and a straightforward data model. One shared `TileSet.tres` resource covers all three tile pools (unique, shared, universal) as separate atlas source IDs within the single TileSet. Two TileMap layers within the node: one for floors, one for walls/objects.

**NPC sprites:** Use **sprite sheet with `region_rect`** — not separate Texture2D files per expression state. One PNG per archetype. `Sprite2D` node with `region_enabled = true`; `region_rect` is set per expression state in code. Sheet layout: horizontal strip, one column per state. If the optional 2-frame breathing loop is implemented, use a top row (frame A) and bottom row (frame B) with a 2-keyframe `AnimationPlayer` at 0.75–1.0 fps.

**Player avatar (circular crop):** `TextureRect` at 24×24px + `ShaderMaterial` with a fragment shader that discards pixels outside `length(UV - vec2(0.5)) > 0.5`. The source PNG remains a square sprite with standard import settings. Do not pre-crop to a circle at export — this discards pixels permanently and prevents use at other sizes. [VERIFY IN GODOT 4.6 DOCS — Confirm CanvasItem ShaderMaterial assignment on TextureRect in 4.6; verify `UV` built-in availability in canvas item shaders.]

**Badges:** `PanelContainer + Label` nodes. No imported texture asset. Fill, corner radius, and border are set via `StyleBoxFlat` on the PanelContainer. Label text and font are set at runtime. Badge appearance changes are resource/code edits, not asset re-imports. The BANGKRUT badge is the same node structure, placed on CanvasLayer 90 (see 8.11).

---

### 8.10 Palette Enforcement in Godot

**Palette reference asset:** `assets/art/palette/palette_reference.png` — a 7×1px PNG where each pixel is one of the seven canonical palette colors in fixed left-to-right index order. This is the single source of truth for all pipeline tools.

**GIMP Palette file:** `assets/art/palette/cicip-catat.gpl` — plain text, importable into Aseprite and most pixel art tools. Both files are committed together and must change together if the palette changes.

**Aseprite export workflow:**
1. Use **Indexed Color Mode** in Aseprite — enforces palette membership at paint time.
2. Load `cicip-catat.gpl` as the active palette before creating any new sprite document.
3. Export as PNG with **Color Mode: Indexed**. Do not convert to RGB at export.
4. No dithering on environment tiles and NPC sprites (dithering introduces off-palette in-between colors). Dithering is selectively permitted on food photo tiles where gradient simulation is intentional — document which food categories permit it.
5. Do not use Aseprite's palette reduction or quantize on final exports.

**Runtime palette validation (editor tool):** Implement a lightweight `EditorScript` at `tools/art-pipeline/palette_validator.gd` that iterates over `assets/art/`, loads each PNG as an `Image`, samples every pixel via `get_pixel()`, and reports any out-of-palette colors to the Output panel. Runs on demand, not in CI. Output only — no file modifications. [VERIFY IN GODOT 4.6 DOCS — `DirAccess` API changed in 4.4 with updated return types; verify current usage pattern before implementing.]

---

### 8.11 CanvasLayer Architecture

*The layer numbers in this section supersede the rough references in Section 7 (which used 5, 10, 100 as illustrative values). Section 8.11 is the definitive stack.*

**Exemption mechanism:** `CanvasModulate` multiplies its color against all content in the same viewport. To exempt a CanvasLayer from the saturation shader, place a second `CanvasModulate` node on that layer set to `Color(1,1,1,1)` (neutral white). Each CanvasLayer is an independent compositing context, so the neutral modulate on that layer overrides the world-layer desaturation for content on that layer. [VERIFY IN GODOT 4.6 DOCS — The interaction between CanvasModulate and multiple CanvasLayers in Godot 4.6 should be tested with a minimal scene. The D3D12 default on Windows in 4.6 and glow rework may have incidental effects on CanvasModulate compositing.]

**Complete CanvasLayer stack:**

| Layer | Name | Contents | Saturation exempt? |
|---|---|---|---|
| 0 | World Content | TileMap/TileMapLayer (environment), Sprite2D (NPCs, player), food photo TextureRects | No — this layer IS what the saturation lever controls |
| 20 | HUD | Month indicator, follower counter, balance chip, phase indicators | Yes — `Color(1,1,1,1)` CanvasModulate |
| 30 | Semantic Colors | Saldo Merah display, financial delta indicators, all state-semantic color text | Yes |
| 40 | Text | Body text labels that must remain legible at all saturation states | Yes |
| 50 | Notifications | Toast notification banners, badge reveal animations | Yes |
| 90 | BANGKRUT Overlay | BANGKRUT badge, full-screen Game Over treatment | Yes |
| 100 | White-Wash | Single ColorRect, white at full alpha, 1-frame milestone flash | Yes (not modulated) |

**Layer 100 white-wash:** ColorRect is a child of the Layer 100 CanvasLayer node, not any world-space node. CanvasLayer ordering by index number is authoritative in Godot 4.x — higher index renders on top regardless of scene tree position. [VERIFY IN GODOT 4.6 DOCS — Confirm CanvasLayer z-ordering has not changed in 4.5 or 4.6.]

**Scene tree placement:** All CanvasLayer nodes are direct children of the root persistent scene (game manager or main scene). Do not place CanvasLayer nodes inside restaurant scenes that load/unload — this would reset the overlay stack on scene transitions.

---

### 8.12 Asset Directory Structure

```
assets/
├── art/
│   ├── sprites/
│   │   ├── npc_owner_01_idle_32x48.png      # one file per NPC + state
│   │   ├── npc_chef_01_idle_32x48.png
│   │   ├── npc_rival_01_idle_32x48.png
│   │   ├── plr_avatar_01_24x24.png
│   │   └── hand_hold_48x32.png
│   ├── tiles/
│   │   ├── unique/                           # 30 restaurant-specific tiles
│   │   │   ├── warung-bu-siti/               # slug matches restaurant ID
│   │   │   └── [restaurant-slug]/
│   │   ├── shared/                           # 18 tier-shared tiles
│   │   └── universal/                        # 10 tiles used by all tiers
│   ├── tileset.tres                          # shared TileSet resource (all three pools)
│   ├── food-photos/
│   │   ├── warung-bu-siti/                   # one subdirectory per restaurant
│   │   │   └── food_nasigoreng_t3_64.png
│   │   └── _placeholder/                     # generic tiles for dev/testing
│   ├── ui/
│   │   └── glyphs/                           # colorblind safety glyph icons only
│   │       ├── ui_glyph_down_default.png
│   │       ├── ui_glyph_warn_default.png
│   │       └── ui_glyph_check_default.png
│   └── palette/
│       ├── palette_reference.png             # 7×1px canonical strip
│       └── cicip-catat.gpl                   # GIMP palette file for Aseprite
├── fonts/
│   ├── slot-a/
│   │   ├── fnt_a_regular.ttf
│   │   ├── fnt_a_bold.ttf
│   │   └── slot_a.tres                       # Godot FontFile resource
│   └── slot-b/
│       ├── fnt_b_regular.ttf
│       └── slot_b.tres
└── shaders/
    └── circle_mask.gdshader                  # Circle crop for player avatar TextureRect
```

**Food photo naming:** `[restaurant-slug]_[dish-slug]_[variant].png` inside the restaurant's subdirectory. The restaurant slug matches the subdirectory name exactly, enabling a data-driven texture loader to construct file paths from restaurant ID + dish ID without a lookup table.

---

### 8.13 Performance and Memory Constraints

At this project's scale — a 2D roguelike with no dynamic lighting and ≤58 environment tiles — performance concerns are minimal on any PC/Steam hardware from the last decade. The figures below are practical upper bounds, not constraints requiring active optimization.

**Texture atlases:** Recommend one atlas per tile pool: `256×256px` for universal + shared combined (28 tiles), `128×128px` per unique-tier subdirectory (≤10 tiles each). One atlas PNG can hold ~100 tiles at 48×48px; all 58 MVP tiles fit in two atlases. All atlas textures imported Lossless.

**Sprite sheets vs. separate files:** At this scale (3–4 archetypes, ≤5 expression states each), the performance difference is immeasurable. Sprite sheets are preferred for workflow simplicity (one file import, one atlas entry in VRAM), not for frame-time impact.

**MVP VRAM estimate:**

| Asset category | Estimated VRAM |
|---|---|
| Environment tile atlases (~4 × 256×256 worst case) | ~1 MB |
| Food photo tiles (~15 tiles × 64×64px) | ~0.25 MB |
| NPC sprite sheets (4 sheets × ~160×96px) | ~0.25 MB |
| UI glyph icons (minimal) | negligible |
| **Total pixel art VRAM** | **~1.5 MB** |

Fonts are system RAM (not VRAM): ~2 MB for two vector typefaces. Total memory well within any PC target. No atlas packing optimization or streaming needed for MVP.

**CanvasModulate:** A single color change per phase transition is a single uniform update — effectively free. Eight CanvasLayers add approximately 8 compositing passes per frame; negligible overhead on PC at this scene complexity.

**NPC breathing loop (2 frames):** Two AnimationPlayer nodes cycling a 2-keyframe animation at 0.75 fps are computationally free. Include without hesitation if the art direction calls for it.

[VERIFY IN GODOT 4.6 DOCS — Godot 4.6 defaults to D3D12 on Windows. Confirm D3D12 does not introduce behavioral differences for CanvasModulate or CanvasLayer compositing compared to Vulkan. For development on Linux/macOS, the rendering backend differs and may produce slightly different compositing results — test on target platform before final art pass.]

---

## 9. Reference Direction

[To be authored]
