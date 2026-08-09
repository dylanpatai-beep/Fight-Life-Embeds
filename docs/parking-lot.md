# PARKING LOT

Everything real but out of scope for the phase we're in. Nothing here is forgotten and
nothing here is being worked on.

**The rule:** closed lists stay closed. If it isn't in the current phase's scope, it lands
here instead of quietly expanding the plan. Items leave this file only when you promote them.

**Opened** 2026-08-09 (Phase 1) · **Last updated** 2026-08-09

---

## Decisions waiting on Dylan

| # | Item | Why it's parked | Blocks |
|---|---|---|---|
| P-01 | **Beehiiv vs Substack** — newsletter split 2 sent on each | Platform consolidation is a business decision, not a Phase 1 one | Newsletter as a module output channel |
| P-02 | **Department social media / outside-employment policy** — unread | Professional exposure on Paramedicine + Psychology content | Subject 4 and 8 modules |
| P-03 | **Psychedelics as published content** (subject 8) | Legal, employer, and platform policy all intersect | Subject 8 modules |
| P-04 | **Instagram** — account exists, nothing ever posted | Untested channel; not routing curriculum through it yet | Nothing currently |

---

## Known broken

| # | Item | Detail | Effort |
|---|---|---|---|
| P-05 | **Command Center tracker doesn't persist** | `index.html` calls `window.storage.get/set` (the claude.ai artifact API). That API doesn't exist on static hosting, so every checkbox resets on reload. Fix is `localStorage`. | Small |
| P-06 | **Brand token drift** | `index.html` uses bone `#E8E6E3`; `tfl-library` and `tfl-app` both use `#E8E6E1`. Library/app are canonical. | Trivial |

---

## Existing work with open gates

| # | Item | State | Note |
|---|---|---|---|
| P-07 | **tfl-app Phase 1 gate** — "Dylan logs a real training week; rollups correct" | Open since 2026-07-07 | Called out as Risk 3 in the spec. Recommended for the 8/11 set. |
| P-08 | **tfl-app Phase 2 remainder** — TestFlight tester setup + install on iPhone & iPad | Rest of Phase 2 done 2026-07-08 | One step from daily-driver |
| P-09 | **tfl-app Phase 3 prereqs** (Dylan-side) | iCloud Health sync check on both devices; Garmin Connect → Apple Health enable | From `docs/PHASE-0.md` |
| P-10 | **tfl-library: 8 sample entries sitting as drafts** | 2 per lane, `status: draft`, never published | Spec's MA-05/MA-06 finish `switch-kick.md` + `the-long-guard.md`. The other 6 stay parked. |
| P-11 | **12 Command Center foundation templates unfilled** | Every one is `[FILL IN]` skeletons — about-me, principles, brand guide, anti-AI writing style, 5 pillar files | The brand guide and anti-AI writing style are the two that matter for CREATE. Not Phase 1 work. |

---

## Deferred design problems

| # | Item | Detail | Phase |
|---|---|---|---|
| P-12 | **GoodNotes PDF round-trip** | You fill worksheets by hand on iPad and upload pages back. Static hosting has no backend to receive an upload. Options exist (commit images to the repo, iOS Shortcut, or the app handles it) — none chosen. | Phase 2 |
| P-13 | **Curriculum ↔ tracker integration** | Module completion and training data in one view. The tracker is a native iOS app; the curriculum is planned as static web. They cannot write to each other directly. Needs a real design decision. | Phase 3 |
| P-14 | **Application-period proof** | The only gate condition with no natural evidence (Risk 5). Ties to tracker session data. | Phase 3 |
| P-15 | **Review surface** | 5-min end-of-set-day check + full review on Day 1 of the 6 off | Phase 3 |

---

## Won't chase unless asked

| # | Item | Why |
|---|---|---|
| P-16 | **Stranded July sprint artifacts** in old claude.ai chats | Inventory doc, tracker update list, tagline capture, curriculum spec scaffold. Confirmed 2026-08-08 as either never built or living only in past conversations. This spec supersedes them. Recovery is only worth it if something specific is missing. |
| P-17 | **Intake pipeline** (`yt2md`, `doc2md`) | Referenced in `tfl-library/AGENTS.md` as the raw-material path, but exists in no repo. Presumed local or presumed gone. |
| P-18 | **`VS-Code` repo** | Contains one README with one line. Empty. Delete or ignore. |
