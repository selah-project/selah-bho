# The Selah Bhojpuri Rendering — NOTES

*bho.v1 · chair 70 · lit and sealed 2026-09-11 (Rosh Hashanah 5787) —
burned and seated in a single day. Bhojpuri, ~52M speakers: Bihar,
eastern Uttar Pradesh, the Nepal Terai, and one of the largest
indenture-era diasporas on earth (Mauritius, Fiji, Suriname, Trinidad,
Guyana).*

## The seal

| Count | Value |
|---|---|
| Verses | 23,213 / 23,213 |
| Token spine ≡ en floor | 23,213 / 23,213, zero mismatches; surfaces byte-identical |
| यहवे at the Name seat | **6,828 / 6,828 — zero deviations** |
| ⟨את⟩ | 11,866 in the token row ≡ 11,866 in the flow ≡ the en floor, per-file 0 off |
| Erasure (ईश्वर / प्रभु / भगवान / परमेश्वर / परमात्मा at divine seats) | **0** |
| Hindi thermometer (है / ने / मैं at word boundary) | **0 · 0 · 0** |
| नरक for Sheol | **0** — Sheol stands as शेओल |
| ⟨ית⟩ | **0** corpus-wide |
| Aleph-tav audit | `[]` — defective 0, misaligned 0 |
| Empty glosses | 2 — the en floor's own two lawful holes |
| Latin / stray Hebrew in the flow | **0 / 0** |

## Cruxes of the chair

- **The Hindi guard held.** The chair shares Devanagari with Hindi and
  the rails bet everything on the register: the thermometer reads
  absolute zero, the ergative ने does not exist in the corpus, the
  copula is बा, the first person is हम. Tekoa: only 5 of 23,213 verses
  came out of the burn in Hindi — all re-pressed. ~50 oblique-pronoun
  and erasure-word leaks repaired at census.
- **The homoglyph plague.** The burn's characteristic artifact: 368
  Devanagari letters replaced by look-alike Hebrew characters
  (दावיצ, यरूशלयिम, बेटा as בेटा — including the rare presentation
  block ׯ ׮ ׶). All reversed by the whitelist homoglyph table in
  `dev/scripts/bho_tekoa_class_a.py`; 60 corrupted ⟨את⟩ markers
  normalized.
- **The surface-corruption class.** 6,178 token surfaces carried
  points, half-transliterations, or whole glosses where bare Hebrew
  belongs — invisible to a token-count spine check.
  `dev/scripts/bho_surface_restore.py` restores every surface from the
  floor; the Name-seat count snapped to the Masoretic 6,828 exact the
  moment it ran. (The same pass surfaced a FLOOR defect: en itself
  carried pointed surfaces at Deut 22:18 and Jer 15:6 — fixed
  upstream.)
- **The center verse.** Lev 8:35's תמותו came out of the burn as
  *"so that you will have no meaning"*. The center verse of the 4D
  space now says what the Hebrew says: ताकि रउआ ना मरऽ — *that you
  die not*.
- **The חשך inversion.** The burn glossed darkness as अँजोर (light) at
  ~24 noun seats — cured corpus-wide to the अँधियार family; the
  withhold-verb senses of חשך were left standing, correctly.
- **The seventy stayed seventy.** ~20 numerals drifted (Jeremiah's
  seventy years had become 77 and 80; the sixty-two weeks, 66) — every
  one restored against the Hebrew; the additive Indic collapse
  (सत्ताईस आ सौ for 127) kept as lawful.
- **1sg → 1pl person drift**: 218 glosses + 167 flows where the Hebrew
  says *me* and the burn said *us* (हमनी) — repaired with a 1pl-guard
  so genuine plurals were never touched.
- **Dan 3:12, the seventeenth chair.** יתהון is the Aramaic pronoun
  object, not the marker: bare ओकनी के, no ⟨את⟩, no ⟨ית⟩, per every
  sibling.

## Tekoa

First verdict: **DOES NOT SEAT — one mechanical repair pass away**
("the chair's declared hazard did not fire"). The pass ran: all
class-A lanes discharged, machine re-verified green. Full report:
`data/experiments/bho-seating/bho-tekoa-report.md` (selah repo).
Class B PENDING SCOTT, headline items: proper-name transliteration
unnormalized in every book (Solomon 5 forms, Saul 12); Maithili/Magahi
neighbour bleed the rails never named (Isa 53:5 in Maithili
morphology); ארץ split धरती 88% / देस 7%; Aramaic God-word 6 forms in
Daniel.

## The burn

23,213 / 23,213 verses, z.ai glm-5.3, lit 13:15 and burned by 19:45 on
2026-09-11 (~6.5 hours, first-hour gate at 995 files). Ladder for
stragglers and repairs: max-tokens 24–32k first, then temp 0.55, then
the glm-5.3 tier. ~185 verses re-pressed at seating. Rails:
`docs/methodology/translation-discipline/bho.md` (written in Bhojpuri).
