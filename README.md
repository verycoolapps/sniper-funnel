# 🎯 Funnel Sniper

**Konten marketing yang tepat sasaran — bukan sekadar bagus, tapi pas di funnel stage-nya.**
**Precision-calibrated marketing content — not just good copy, but the right copy for where your audience actually is.**

[![Version](https://img.shields.io/badge/version-1.0.0-blue?style=flat-square)](./SKILL.md)
[![Works with](https://img.shields.io/badge/works%20with-Claude%20Code-blueviolet?style=flat-square)](https://claude.ai/code)
[![Stage Coverage](https://img.shields.io/badge/stages-TOFU%20%7C%20MOFU%20%7C%20BOFU-green?style=flat-square)](#)
[![License: MIT](https://img.shields.io/badge/license-MIT-yellow?style=flat-square)](./LICENSE)

---

## Masalahnya / The Problem

Sebagian besar konten marketing gagal bukan karena jelek — tapi karena **salah stage**.

Most marketing content fails not because it's bad — but because it's **aimed at the wrong funnel stage**.

| ❌ Yang biasa terjadi / What usually happens | ✅ Yang seharusnya terjadi / What should happen |
|---|---|
| Caption bagus tapi CTA "Beli sekarang" ke cold audience | TOFU: bangun keingintahuan, bukan closing |
| Email panjang ngajarin hal basic ke lead yang udah riset | MOFU: tangani keberatan, bukan edukasi ulang |
| Landing page yang masih "awareness mode" ke hot lead | BOFU: hapus gesekan, langsung ke konversi |

---

## Cara Kerja / How It Works

```
Input Kamu / Your Input
─────────────────────────────────────
Produk: Suplemen tidur herbal
Target: Profesional muda yang begadang karena kerjaan
Stage: TOFU (cold audience, belum kenal brand)
Format: Caption Instagram

Output Funnel Sniper
─────────────────────────────────────
Stage: TOFU — audience belum aware dengan solusi
Format: Caption Instagram
Platform: Instagram — maks 2200 karakter; 3-5 hashtag targeted
Psychological trigger: Shared identity — "pekerja yang begadang" 
  diname secara ultra-spesifik sebelum ada mention produk

───────────────────
Jam 11 malam, kerjaan belum kelar, dan kamu udah buka 
YouTube ketiga kalinya "buat semangat".

Itu bukan kurang disiplin.
Itu kortisol yang naik pas harusnya turun.

(Simpan ini kalau kamu sering di posisi ini 👇)
───────────────────

CTA: "Simpan" — stage-appropriate, tidak meminta pembelian
Tone: Peer-to-peer, tidak ada nada brand corporate
Non-obvious move: Membingkai masalah sebagai respons 
  biologis (kortisol), bukan karakter — reframe yang 
  tidak akan dibuat oleh template generik manapun
```

---

## Apa yang Dicakup / What It Covers

| Format | TOFU | MOFU | BOFU |
|---|:---:|:---:|:---:|
| Caption & Social Copy | ✓ | ✓ | ✓ |
| Email & Nurture Sequence | ✓ | ✓ | ✓ |
| Blog Post & Long-form | ✓ | ✓ | — |
| Landing Page | — | — | ✓ |
| Video Script (Reels/TikTok/YT) | ✓ | ✓ | ✓ |
| Carousel & Thread | ✓ | ✓ | — |
| Ads (Awareness / Retargeting / Close) | ✓ | ✓ | ✓ |
| Proposal & B2B Follow-up | — | ✓ | ✓ |
| Cart Abandonment Email | — | — | ✓ |

---

## Cara Install / How to Install

```bash
# Salin folder ke direktori skills Claude Code kamu
# Copy the folder to your Claude Code skills directory

git clone https://github.com/verycoolapps/sniper-funnel.git
cp -r sniper-funnel/ ~/.claude/skills/funnel-sniper/
```

Restart Claude Code. Skill aktif otomatis saat kamu minta konten dengan konteks produk + audiens.

Restart Claude Code. The skill activates automatically when you ask for content with a product + audience context.

---

## Cara Pakai / How to Use

Cukup deskripsikan produk, audiens, dan stage (opsional — bisa auto-detect):

Just describe your product, audience, and stage (optional — it auto-detects):

```
"Bikin caption TOFU untuk brand kopi specialty, target pekerja kantoran Jakarta"

"Write a cart abandonment email for my Rp 2.5jt online design course"

"Konten nurturing untuk warm leads yang udah download lead magnet gue"

"Landing page closing untuk program coaching digital marketing saya"
```

---

## Kenapa Bukan AI Slop / Why This Isn't AI Slop

Funnel Sniper punya **quality gates konkret** yang dijalankan sebelum output dikirim:

Funnel Sniper enforces **concrete, observable quality gates** before any output is delivered:

- Setiap psychological trigger diberi nama dengan mekanismenya — bukan label kosong seperti "buat keingintahuan"
- CTA divalidasi ke stage-nya: TOFU tidak pernah closing, BOFU tidak pernah soft
- Dilarang keras: "Halo guys", "Apakah kamu pernah…", emoji walls, scarcity palsu, testimoni rekaan
- Setiap konten punya ≥1 "non-obvious move" yang diderivasi dari dunia produk itu sendiri — bukan dari template
- Tidak ada statistik rekaan; kalau butuh angka, pakai placeholder `[X]` yang harus diisi data nyata

---

## Struktur / Structure

```
funnel-sniper/
├── SKILL.md                          # Core skill — loaded on trigger
├── references/
│   ├── tofu-playbook.md             # TOFU triggers, formats, bans, patterns
│   ├── mofu-playbook.md             # MOFU triggers, formats, bans, patterns
│   └── bofu-playbook.md             # BOFU triggers, formats, bans, patterns
└── evals/
    └── evals.json                    # 12 trigger tests + 4 behavior cases
```

Setiap playbook dibaca **on-demand** — hanya stage yang relevan yang di-load.

Each playbook is read **on-demand** — only the relevant stage is loaded per run.

---

## Dibangun Dengan / Built With

[Skill Forge Ultra](https://github.com/verycoolapps/skill-forge-ultra) — framework untuk membuat Claude Skills yang production-ready, teruji, dan tidak berisi adjective kosong.

---

## Kontribusi / Contributing

Pull request untuk tambahan format, playbook bahasa lain, atau perbaikan quality gates sangat disambut.

PRs for additional formats, localized playbooks, or improved quality gates are very welcome.

---

## License

MIT — gunakan, modifikasi, dan distribusikan bebas dengan atribusi.
MIT — use, modify, and distribute freely with attribution.

---

<p align="center">
  <strong>⭐ Star this repo kalau kamu capek konten bagus tapi salah sasaran.</strong><br>
  <strong>⭐ Star this if you're tired of writing great content that hits the wrong audience.</strong>
</p>
