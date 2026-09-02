# NERV Personality Quiz v3.6

A static, client-side, unofficial Evangelion fan-made personality quiz.

## GitHub Pages

Publish this repository from the repository root with GitHub Pages. No build step, server, database, or API is required.

All quiz scoring and interpretation run locally in the visitor's browser. The site does not submit quiz answers to a server.

## Current model

- 30 questions across five analysis phases
- 16 character profiles
- Character Compatibility: 75% accumulated evidence + 25% phase breadth
- EVA Sync Rate and Profile Structure
- Eight-trait interpretive psychological profile
- Provisional MAGI Cross-Check for close/tied results

The MAGI Cross-Check activates when the top two underlying compatibility scores are within 0.75 points or when they round to the same displayed percentage. It is a provisional tester feature and does not silently replace the behavioural winner.

## Fan project notice

This is an unofficial, non-commercial fan project inspired by *Neon Genesis Evangelion* and the wider *Evangelion* franchise. It is not affiliated with or endorsed by the Evangelion rights holders.

*Evangelion*, NERV, its characters, names, logos, terminology and related intellectual property belong to their respective rights holders. No ownership of those properties is claimed.

The quiz is for entertainment only. Its psychological profiles and scores are not psychological, medical or clinical assessments.

## Project material

Original quiz text, scoring methodology and source code were created for this fan project. Third-party intellectual property is excluded from any permission or licence that may apply to original project material.

## v3.6 UI/UX pass

The scoring/calibration model is unchanged from v3.5.1. This release improves pacing, progress feedback, result hierarchy, metric explanations, bipolar psychological spectra, keyboard focus, ARIA state/status handling, and reduced-motion support. Fonts are self-hosted; no external font request is required.


## Compact result sharing

Shared results use a compact `#r=` fragment. The payload stores only the derived result needed to reconstruct the result page; it does not contain the 30 individual answers. Browsers with Web Share support use the native share sheet, with clipboard copying as the fallback. Older `#result=` links remain readable.

## v3.6.7 sharing reliability

Compact shared results now use `?r=` rather than `#r=` for newly generated links. Query parameters are more reliably preserved by browsers, redirectors, messaging applications and GitHub Pages navigation. Existing `#r=` compact links and older `#result=` links remain supported.

## v3.6.7 share restoration/cache fix

The main JavaScript asset now has a versioned filename (`quiz-v3.6.7.js`). This prevents a browser or GitHub Pages/CDN cache from pairing a newly deployed `index.html` with an older quiz script that does not understand the compact shared-result format.

New shares continue to use compact `?r=` links. Existing `#r=` and `#result=` links remain supported.


## v3.6.7 — result layout refinement

- Character quote and character blurb now appear immediately after the primary result metrics/interpretation, before MAGI Analysis / Match Rationale.
- Secondary and tertiary character patterns have moved into the left result column directly beneath the primary dossier artwork.
- On desktop the supporting patterns stack beneath the primary image, making better use of the previously unused space below the portrait.
- On smaller screens the supporting cards adapt to two columns where space allows, then one column on narrow phones.
- No scoring, calibration, MAGI Cross-Check, compact sharing, or result-restoration logic has changed.

## v3.6.7 — thematic UX refinement

The 30-question assessment, all answer-to-character score vectors, compatibility calibration,
EVA Sync calibration, Profile Structure thresholds, eight-trait logic and compact sharing are unchanged.

Changes:
- all 30 prompts receive light NERV/MAGI scenario framing while preserving their original psychological dilemma;
- phase cards now state what each MAGI phase is assessing;
- transitions explicitly report that the previous response pattern was acquired and that MAGI is synchronising;
- answer guidance now asks for the response closest to the user's first instinct;
- the result header is framed as a MAGI Personnel Compatibility Record;
- no question was added, removed or moved, and no answer score was altered.
