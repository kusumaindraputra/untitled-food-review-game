# Game Concept: Cicip & Catat

*Created: 2026-06-25*
*Status: Draft*

---

## Elevator Pitch

> Roguelike management game di mana kamu menjadi food reviewer yang harus
> survive 12 bulan — mengunjungi restoran, menilai dengan checklist ketat, dan
> menerbitkan ulasan yang menentukan nasib orang lain, sambil berjuang agar
> rekeningmu tidak nol sebelum tahun berakhir.

---

## Core Identity

| Aspect | Detail |
| ---- | ---- |
| **Genre** | Roguelike Management / Bureaucratic Sim |
| **Platform** | PC (Steam / Epic Games Store) |
| **Target Audience** | Mid-core solo players, fans of Papers Please dan Balatro |
| **Player Count** | Single-player |
| **Session Length** | 30-60 menit |
| **Monetization** | Premium |
| **Estimated Scope** | Medium (3–5 bulan, solo dev) |
| **Comparable Titles** | Papers Please, Balatro, Spiritfarer |

---

## Core Fantasy

Merasakan kekuatan dan beban menjadi food influencer — di mana kata-katamu
menentukan nasib sebuah warung makan yang sudah berdiri dua puluh tahun, tapi
rekeningmu sendiri selalu di ujung tanduk. Kamu bukan dewa rasa, kamu hanya
seseorang dengan mulut yang dipercaya orang banyak, dan kepercayaan itu punya
harga.

---

## Unique Hook

Seperti Papers Please TAPI kamu yang memberi stempelnya ke restoran — dan
restoran yang pernah kamu hancurkan atau selamatkan punya cerita yang akan
kamu temui lagi di run berikutnya, dengan cara yang tidak selalu kamu duga.

---

## Visual Identity Anchor

**Arah Visual: "Buku Catatan yang Hidup"**

*One-line rule*: Setiap elemen UI dan environment terasa seperti halaman buku
catatan seorang reviewer sungguhan — coretan, stempel, foto polaroid, dan
tanda centang.

**Prinsip Visual:**

1. **Pixel art dengan karakter yang expressive** — karakter NPC punya idle
   animation yang mencerminkan mood mereka. Chef yang bangga berdiri tegak.
   Owner yang tertekan mengusap tangan ke celemek.
   *Design test*: "Kalau debating antara animasi yang lebih complex vs karakter
   yang lebih banyak — prioritaskan ekspresi karakter yang sudah ada."

2. **UI sebagai artefak fisik** — checklist dievaluasi dengan tanda centang
   atau silang yang terasa ditulis tangan. Rating bintang 'dicap' seperti
   stempel. Budget tracker terlihat seperti pembukuan nota.
   *Design test*: "Kalau ada elemen UI yang terasa seperti software, bukan
   seperti buku catatan — redesign."

3. **Warna hangat dengan aksen merah dan kuning** — palet dominan warm off-white
   dan cokelat muda (seperti kertas lama), dengan merah untuk highlight negatif
   (pengeluaran, review buruk) dan kuning untuk highlight positif (viral, income).
   *Design test*: "Kalau warna baru terasa 'dingin' atau digital — reject."

**Color Philosophy**: Dunia ini terasa seperti arsip hidup seorang reviewer,
bukan aplikasi tech startup.

---

## Player Experience Analysis (MDA Framework)

### Target Aesthetics (What the player FEELS)

| Aesthetic | Priority | How We Deliver It |
| ---- | ---- | ---- |
| **Sensation** (sensory pleasure) | 3 | Pixel art yang expressive, sound feedback saat checklist dicentang, "thud" satisfying saat bintang di-stamp |
| **Fantasy** (make-believe, role-playing) | 2 | Player IS food reviewer — bukan mengontrol satu, tapi menghayati peran itu |
| **Narrative** (drama, story arc) | 4 | Cerita mini tiap restoran, arc 12 bulan dari unknown ke influential |
| **Challenge** (obstacle course, mastery) | 5 | Survival ekonomi yang mepet tapi bisa dipelajari |
| **Fellowship** (social connection) | N/A | Single-player, tidak ada multiplayer |
| **Discovery** (exploration, secrets) | 2 | Cerita tersembunyi di balik tiap restoran, sistem yang revealed seiring waktu |
| **Expression** (self-expression, creativity) | 4 | Pilihan tone review (jujur/diplomatik/brutal), prioritas spending yang mencerminkan gaya bermain |
| **Submission** (relaxation, comfort zone) | 1 | Ritual bulanan yang absorbing dan meditative — ini primary aesthetic |

### Key Dynamics (Emergent player behaviors)

- Player akan secara natural "menghitung nilai" sebuah restoran sebelum
  mengunjungi: apakah income potensial worth biaya kunjungan?
- Player akan mengembangkan "gaya review" konsisten (selalu jujur, atau selalu
  diplomatik) dan mulai merasakan konsekuensinya
- Player akan mengingat restoran yang pernah dikunjungi dan punya opini sendiri
  tentang mereka sebelum data checklist muncul
- Player akan merasakan tekanan moral ketika kriteria konflik (makanan enak
  tapi service kasar dari chef yang kamu kenal)

### Core Mechanics (Systems we build)

1. **Monthly Planning System** — setiap awal bulan, player melihat daftar
   restoran yang tersedia dengan estimasi biaya kunjungan dan potensi engagement.
   Budget terbatas memaksa prioritisasi.
2. **Checklist Evaluation** — saat mengunjungi restoran, player menilai 4-5
   kriteria satu per satu (Rasa, Plating, Service, Harga, Ambiance). Kriteria
   bisa konflik. Keputusan bintang final bersifat permanen.
3. **Review Publishing** — setelah evaluasi, player memilih tone (Jujur /
   Diplomatik / Brutal) dan mempublikasikan. Hasilnya memengaruhi followers,
   income, dan reaksi NPC.
4. **Economic Survival** — setiap akhir bulan: bayar sewa, biaya hidup,
   cicilan equipment. Saldo minus = game over. Setiap pengeluaran punya trade-off.
5. **NPC Reaction System** — restoran dan karakter (chef, owner, rival reviewer,
   fans) merespons ulasanmu. Reaksi ini bisa membuka atau menutup peluang bulan
   berikutnya.

---

## Player Motivation Profile

### Primary Psychological Needs Served

| Need | How This Game Satisfies It | Strength |
| ---- | ---- | ---- |
| **Autonomy** (freedom, meaningful choice) | Pilih restoran mana yang dikunjungi, tentukan penilaian tiap kriteria, pilih tone review, prioritaskan spending | Core |
| **Competence** (mastery, skill growth) | Makin pintar membaca "nilai" sebuah kunjungan vs biayanya; mengelola bulan-bulan kritis dengan lebih efisien | Core |
| **Relatedness** (connection, belonging) | Reaksi NPC yang genuine — chef yang terima kasih, owner yang kecewa, fans yang setia, rival yang mengintai | Supporting |

### Player Type Appeal (Bartle Taxonomy)

- [x] **Achievers** — Survive 12 bulan, capai fame tier tertinggi, tidak pernah bangkrut
- [x] **Explorers** — Temukan cerita tersembunyi di balik tiap restoran, pelajari sistem ekonomi yang dalam
- [x] **Socializers** — Bangun hubungan dengan NPC restoran, rasakan dampak sosial dari reviewmu
- [ ] **Killers/Competitors** — Tidak relevan, tidak ada PvP

### Flow State Design

- **Onboarding curve**: Bulan pertama memiliki budget lebih longgar dan hanya
  3 restoran tersedia — player belajar sistem tanpa tekanan bankrupt
- **Difficulty scaling**: Semakin tinggi fame, semakin tinggi ekspektasi audiens
  dan semakin mahal gaya hidup yang "harus" dipertahankan
- **Feedback clarity**: Setiap keputusan punya angka yang jelas — followers naik
  sekian, saldo berubah sekian, bintang restoran tercatat permanent
- **Recovery from failure**: Roguelike reset yang cepat — run baru bisa dimulai
  dalam 30 detik. Kegagalan memberi pemahaman tentang pola ekonomi

---

## Core Loop

### Moment-to-Moment (30 detik)

Player mengevaluasi satu kriteria restoran pada satu waktu. Setiap kriteria
punya dua kemungkinan konflik dengan kriteria lain — dan keputusan bintang
final bersifat irreversible. Satisfaction datang dari "click" saat keputusan
dibuat dan stempel bintang jatuh.

### Short-Term (5-15 menit)

Satu bulan adalah satu siklus lengkap: Plan → Visit (beberapa restoran) →
Publish → Pay Bills → lihat hasil. "One more month" datang dari: *selalu ada
restoran bulan depan yang tampak menjanjikan, tapi budget selalu mepet.*

### Session-Level (30-60 menit)

Satu session = 1-3 bulan gameplay. Natural stopping point: akhir tiap bulan
(setelah bayar tagihan, saldo terlihat jelas). Hook untuk kembali: restoran
baru muncul di preview bulan depan, atau ada NPC yang merespons review terakhir.

### Long-Term Progression

**Dalam satu run (12 bulan):**
- Bulan 1-3: Unknown Reviewer — struggling, tiap pengeluaran terasa berat
- Bulan 4-7: Rising Reviewer — momentum mulai ada, tapi ekspektasi naik
- Bulan 8-11: Known Reviewer — tekanan puncak, cicilan lama jatuh tempo
- Bulan 12: Climax — survive atau bankrupt. Ending berbeda tergantung keputusan

**Antar run (roguelike):**
- Setiap run punya seed berbeda: restoran yang tersedia, urutan event, harga
- Player membawa pengetahuan (bukan power) antar run — tahu cara baca pola ekonomi

### Retention Hooks

- **Curiosity**: Restoran misterius yang belum terbuka, NPC yang belum selesai ceritanya
- **Investment**: Run yang hampir selesai di bulan ke-10 — terlalu sayang untuk dilepas
- **Social**: N/A (single-player)
- **Mastery**: Bisa survive dengan margin yang semakin sempit dan efisien

---

## Game Pillars

### Pillar 1: Tiap Rupiah Bercerita
Setiap keputusan finansial membawa konsekuensi naratif, bukan sekadar
perubahan angka. Membeli lensa baru bukan hanya "+quality" — artinya bulan
ini tidak ada budget untuk restoran high-end.

*Design test*: "Jika debating antara fitur yang menambah angka vs fitur yang
menambah cerita di balik angka — pilih yang menghasilkan cerita."

### Pillar 2: Rutinitas yang Menyerap
Loop bulanan harus terasa seperti ritual yang absorbing dan meditative, bukan
treadmill yang menegangkan. Player harus bisa masuk ke flow state dalam 2-3
menit setelah membuka game.

*Design test*: "Jika ada mekanik baru yang mempercepat pace tapi menghilangkan
momen refleksi checklist — tolak."

### Pillar 3: Reviewer Bukan Dewa
Player punya kekuatan tapi selalu ada konsekuensi. Review jujur bisa
menghancurkan. Review diplomatik bisa mempermalukan. Tidak ada pilihan yang
sepenuhnya aman.

*Design test*: "Jika ada opsi yang selalu optimal tanpa risiko apapun —
tambahkan risikonya."

### Pillar 4: Restoran Punya Jiwa
Setiap lokasi bukan sekadar stat block. Ada lore kecil, ada karakter, ada
sejarah yang tidak langsung terlihat. Player harus merasa ada cerita yang
layak untuk ditemukan.

*Design test*: "Jika debating antara menambah restoran generic baru vs
memperdalam cerita restoran yang sudah ada — pilih yang kedua."

### Anti-Pillars (What This Game Is NOT)

- **BUKAN cooking game**: Player tidak memasak, tidak ada minigame memasak.
  Player menilai, bukan berkreasi di dapur. Ini melindungi Pilar 2.
- **BUKAN social sim dengan romance mechanic**: Hubungan dengan NPC punya
  bobot tapi tidak ada romance path — terlalu kompleks untuk scope dan akan
  mengalihkan dari economic survival.
- **BUKAN action/combat game**: Chef yang marah tidak dihadapi dengan combat.
  Konflik diselesaikan melalui keputusan review dan konsekuensi ekonomi.
- **BUKAN perfectly balanced**: Akan selalu ada bulan yang terasa tidak adil.
  Itu disengaja — seperti Papers Please, tension datang dari constraint yang
  tidak bisa selalu diatasi dengan sempurna.

---

## Inspiration and References

| Reference | What We Take From It | What We Do Differently | Why It Matters |
| ---- | ---- | ---- | ---- |
| **Papers Please** | Checklist ritual sebagai gameplay utama; moral weight dalam keputusan sederhana; dunia yang merespons pilihanmu | Player punya kekuatan lebih (reviewer bisa MEMILIH tidak menulis) dan setting lebih hangat | Membuktikan bahwa mundane bureaucracy bisa jadi drama emosional yang dalam |
| **Balatro** | "Just one more run" psychology; satisfaction dari keputusan yang irreversible; emergent complexity dari sistem sederhana | Tidak ada kartu — keputusan berbentuk judgment call manusia, bukan matematik kartu | Membuktikan roguelike loop bisa bekerja tanpa combat sebagai inti |
| **Hades** | Narrative yang terungkap melalui repeated runs; NPC yang punya memory terhadap run sebelumnya | Tidak ada meta-progression power — yang bertahan antar run hanya pengetahuan player | Membuktikan roguelike bisa punya kedalaman emosional dan karakter yang diingat |

**Non-game inspirations**:
- Blog kuliner Indonesia dan culture food reviewer di media sosial (Magdalene,
  Pergikuliner) — tone dan tantangan relatable
- Film *Ratatouille* — gagasan bahwa kritikus punya kekuatan menghancurkan yang
  sama besarnya dengan kekuatan memuji
- Esai *The Inspector General* (Gogol) — birokrat kecil yang tiba-tiba punya
  kekuatan besar dan tidak tahu harus berbuat apa

---

## Target Player Profile

| Attribute | Detail |
| ---- | ---- |
| **Age range** | 18-30 |
| **Gaming experience** | Mid-core |
| **Time availability** | 30-60 menit per session, bisa beberapa kali seminggu |
| **Platform preference** | PC |
| **Current games they play** | Papers Please, Balatro, Slay the Spire |
| **What they're looking for** | Game yang absorbing tapi tidak butuh reaction time tinggi — bisa sambil dengar podcast, bisa dimainkan setelah capek kerja |
| **What would turn them away** | Real-time combat yang butuh reflex, grind yang terasa meaningless, UI yang membingungkan |

---

## Technical Considerations

| Consideration | Assessment |
| ---- | ---- |
| **Recommended Engine** | Godot 4.6 — lightweight, cocok untuk 2D management, export ke PC sangat clean |
| **Key Technical Challenges** | Balance ekonomi (roguelike balance butuh banyak playtest); procedural restaurant pool per run |
| **Art Style** | Pixel art 2D — estetik "buku catatan hidup", warm color palette |
| **Art Pipeline Complexity** | Medium — custom pixel art per restoran, karakter NPC dengan ekspresi, UI sebagai artefak fisik |
| **Audio Needs** | Moderate — ambient restaurant sounds, UI feedback (stamp, checkmark, coins), mungkin 2-3 tracks musik ambient |
| **Networking** | None |
| **Content Volume** | 15 restoran, 12 bulan gameplay, 30-60 menit per run, ~5-8 jam total discovery |
| **Procedural Systems** | Restaurant availability pool per run (seed-based), urutan event random, variasi harga dan kondisi restoran |

---

## Risks and Open Questions

### Design Risks

- **Economic balance**: Terlalu ketat → frustrasi dan unfun. Terlalu longgar →
  tidak ada tension dan "one more month" hilang. Ini adalah risiko terbesar.
- **Replayability**: Jika tiap run punya restoran yang sama, player habis konten
  dalam 1-2 run. Butuh variasi procedural yang terasa genuine, bukan hanya
  angka yang diacak.
- **Flow vs Stress tension**: Menginginkan "rutinitas absorbing" tapi juga
  "tekanan ekonomi yang nyata" — keduanya bisa saling bertentangan jika tidak
  di-tune dengan benar.

### Technical Risks

- **Balance tuning**: Roguelike economy balance membutuhkan banyak playtest
  iteration — bisa memakan sebagian besar timeline.
- **Content generation cost**: Pixel art untuk 15 restoran + NPC + food items
  bisa menjadi bottleneck untuk solo dev.

### Market Risks

- **Niche audience**: Target player yang suka Papers Please + roguelike adalah
  niche — tapi Papers Please membuktikan niche ini ada dan committed.
- **Tema lokal**: Food reviewer culture Indonesia sangat relatable secara lokal,
  tapi perlu localization atau universalization untuk jangkauan internasional.

### Scope Risks

- **Content volume**: 15 restoran dengan cerita masing-masing adalah target
  ambisius untuk solo dev dalam beberapa bulan.
- **NPC reaction system**: Sistem reaksi NPC yang terasa genuine bisa menjadi
  rabbit hole yang menyedot waktu development.

### Open Questions

- **Apakah checklist loop fun dalam isolasi?** → Dijawab oleh MVP (3 bulan, 5
  restoran, 4 kriteria). Kalau tidak absorbing dalam MVP, pivot ke Konsep 2
  (card combo system).
- **Seberapa besar variasi procedural yang dibutuhkan?** → Dijawab setelah
  3-5 playtest run — apakah player bosan atau masih menemukan hal baru?
- **Apakah pixel art "buku catatan" bisa dikerjakan solo dalam timeline?** →
  Dijawab di fase awal production dengan membuat 2-3 environment restoran
  sebagai test.

---

## MVP Definition

**Core hypothesis**: Evaluasi checklist restoran satu per satu + tekanan budget
bulanan terasa absorbing dan meaningful selama 30+ menit — bukan klik-klik
membosankan.

**Required for MVP**:
1. Monthly planning screen — pilih dari 5 restoran dengan estimasi biaya
2. Checklist evaluation — 4 kriteria (Rasa, Plating, Service, Harga), keputusan bintang
3. Basic economic system — income dari views, fixed expenses akhir bulan,
   bankrupt jika saldo minus
4. 3 bulan gameplay dengan restoran yang sama tiap run (no procedural yet)
5. Minimal pixel art placeholder — cukup untuk merasakan tone

**Explicitly NOT in MVP** (defer to later):
- NPC story arcs dan reaksi karakter
- Equipment system (kamera, notebook upgrade)
- Procedural restaurant variety antar run
- Rival reviewer mechanic
- Random events (food festival, health inspection)
- Polish art dan audio

### Scope Tiers (if budget/time shrinks)

| Tier | Content | Features | Timeline |
| ---- | ---- | ---- | ---- |
| **MVP** | 5 restoran, 3 bulan | Core loop: checklist + budget + publish | 3-4 minggu |
| **Vertical Slice** | 10-12 restoran, 12 bulan | Core + NPC reaksi + equipment sederhana + basic procedural | ~2 bulan |
| **Alpha** | 15 restoran, 12 bulan | Semua fitur, art placeholder, balance kasar | ~3.5 bulan |
| **Full Vision** | 15+ restoran, 12 bulan | Semua fitur polished, rival, events, Steam release | ~5 bulan |

---

## Next Steps

- [ ] Run `/setup-engine` — konfigurasi Godot 4.6 dan populate version-aware reference docs
- [ ] Run `/art-bible` — establish visual identity "buku catatan hidup" sebelum menulis GDD apapun
- [ ] Run `/prototype checklist-economy-loop` — validasi apakah checklist + budget bulanan terasa
      fun sebelum menulis GDD sistem penuh (Path B — Prototype-First)
- [ ] Jika prototype PROCEEDS: run `/map-systems` untuk decompose ke sistem individual
- [ ] Jika prototype PIVOTS: kembali ke `/brainstorm` dengan learnings dari prototype
- [ ] Setelah full design: `/vertical-slice` untuk validasi full game loop
- [ ] `/gate-check pre-production` sebelum commit ke production sprint
