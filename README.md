# achawaqat-research

Deploy source for the AchaWaqat /research/ static toolkit on achawaqat.com.
Deployed via deploy-from-github.php (manifest in ~/workspace/deploy/).

## 2026-10-07 — A24/A25 title fix
All 119 scale pages (scales/<slug>/index.html) got new <title> tags:
- A24: removed the double-encoded `&amp;amp;` (was rendering literally as "&amp;" in tabs/search).
- A25: shortened every title to <= 60 visible characters (was 86-163, truncating in search).
Template: `{ACRONYM} — {short label} | DoctorWithData`; 52 hand-shortened overrides for long names.
Everything else in each file is byte-identical to the live original.
