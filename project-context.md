# KOR-0187 marketing site context

## Scope

- Independent public marketing and study site for released app `KOR-0187` only.
- App source is read-only: `/Users/youngjunma/Documents/various test prep apps project/services/kor/01/kor-0187`.
- Android package and iOS bundle identifier: `app.mcyj.examprep.kor0187`.
- Production target: `https://mcyj.github.io/korean-hairdresser-exam-prep-web/`.

## Verified Store state — 2026-09-19

- Google Play resolves publicly for the exact package.
- Apple public lookup returned no matching app in checked storefronts; the signed iOS build and App Store Connect work are not publication evidence.
- Google Play is the only active Store link. App Store is a localized disabled control with no URL.
- Both marketplace controls use the same 194 × 75 px outer frame.

## Content and official facts

- Korean and English routes with 10 substantive guides per locale.
- Official name: 미용사(일반) / Hairdresser (`jmCd=7937`).
- Written: four-option multiple choice, 60 items in 60 minutes; pass mark 60/100.
- Practical: hairdressing work, approximately 2 hours 25 minutes; pass mark 60/100.
- Current specification is 2022–2026. Candidates taking the exam in 2027 must recheck the 2027–2031 transition.
- Required materials and model conditions must be checked for the current exam year on Q-Net.
- Canonical sources:
  - `https://www.q-net.or.kr/crf005.do?id=crf00503&jmCd=7937`
  - `https://www.q-net.or.kr/crf005.do?id=crf00503s02&jmCd=7937&jmInfoDivCcd=B0`
  - `https://www.q-net.or.kr/cst006.do?artlSeq=5208127&brdId=Q006&code=1202&gId=&gSite=Q&id=cst00602`
  - `https://www.q-net.or.kr/rcv011.do?gSite=Q&id=rcv01103s02&jmCd=7937`

## Design and implementation

- Visual thesis: soft-rose salon editorial with precise sectioning lines and a diagnose–section–shape–finish workflow.
- Global Korean-safe wrapping uses `word-break: keep-all` and `overflow-wrap: break-word`.
- Dependency-free static generator; GitHub Actions builds, checks and deploys `dist/` to Pages.

## Verification log

- 2026-09-19: project initialized from the proven static-site system and retargeted to KOR-0187 content, assets and verified Store state.
- 2026-09-19: local build generated 34 indexable routes and 36 HTML files; the checker passed metadata, links, exact Play identity, disabled App Store state, `keep-all` and equal marketplace frames.
- 2026-09-19: local HTTP QA returned 200 for all 34 sitemap routes and five key assets; an unknown route returned 404.
- 2026-09-19: live Store recheck returned Google Play 200 and Apple `resultCount: 0` in KR, US and GB.
- 2026-09-19: GitHub Pages workflow run `35362985191` completed successfully.
- 2026-09-19: production QA returned 200 for all 34 sitemap routes and five key assets; an unknown route returned 404.
- 2026-09-19: production CSS contains global `word-break: keep-all` and the shared 194 × 75 px marketplace frame; the Korean home links only the exact public Google Play package.
