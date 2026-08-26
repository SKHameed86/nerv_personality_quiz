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
