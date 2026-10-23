# Changelog

## 1.0.6 (2026-10-23)
- README: new "Testing status" section. Local automated tests pass; in-app testing is not yet completed. Records that the marketplace submit form's "tested locally and in-app" confirmation (2026-10-20, under the former name TruthTrace) was checked in error before any in-app test; in-app testing is pending.
- Docs only; no behavior changes. Local tests re-run and passed. Not tested in-app. Not resubmitted.

## 1.0.5 (2026-10-23)
- Translations: each language section in TRANSLATIONS.md now starts with a one-line notice in that language saying it is a machine translation, not reviewed by a native speaker, and that the English version is authoritative. README Languages section notes this. No behavior changes.
- Local tests re-run and passed. Not tested in-app. Not submitted to the marketplace.

## 1.0.4 (2026-10-22)
- Renamed from TruthTrace to TruthSweep (manifest name `truthsweep`, repo github.com/OmnipotentCEOxJenny/truthsweep, skill `truthsweep-check`). Releases 1.0.0 to 1.0.3 and the 2026-10-20 marketplace submission were made under the former name TruthTrace.
- Keywords: 40, with TruthSweep, JennyEcho and OmnipotentCeo. Logo artwork unchanged.
- No behavior changes.

## 1.0.3 (2026-10-21)
- Added `tests/check_frontmatter.py`: a strict YAML front-matter check (PyYAML `safe_load`) for every SKILL.md and rules .mdc file, plus a plugin.json JSON check. Run `python3 tests/check_frontmatter.py` from the repo root; it catches the unquoted-colon bug fixed in PluginPulse 1.0.2.
- No behavior changes to skills or rules.

## 1.0.2 (2026-10-20)
- TRANSLATIONS.md: each of the 23 languages now includes this plugin's specific limits list (from the README's "Honest assessment: what this plugin cannot do" section) plus the marketplace status. Machine translations, not reviewed by native speakers.
- Docs only; no behavior changes.

## 1.0.1 (2026-10-20)
- README follows the shared template: title, plain description, logo, existing content (Rob Domaine's four pillars unchanged), and a new final section "Honest assessment: what this plugin cannot do" listing real limits and the compliance statement.
- TRANSLATIONS.md now covers the same 23 languages as every Omnipotent plugin (title, description and honest-assessment summary for each), all marked as machine translations not reviewed by native speakers.
- Docs only; no behavior changes.
- Status corrected: marketplace submission made 2026-10-20 (pending review).

## 1.0.0 (2026-10-20)
- First release: truthsweep-check (full SIFT workflow with verdicts and confidence) and trace-to-original skills, report template, pillars rule, real worked example (Great Wall from space), logo, translated summaries in 22 languages (machine-made, not native-reviewed).
