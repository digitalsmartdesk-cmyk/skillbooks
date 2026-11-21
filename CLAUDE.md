# Quizykoo Life Skills Series — Site Handoff

## Site identity
- **Name**: Quizykoo Life Skills Series
- **Series**: 20 Kindle eBooks · 4 sets × 5 books · Ages 5–10
- **Live artifact**: https://claude.ai/artifact/Lf11R3fiL2rMZgWc2bvM5Q (Version 6)
- **Contact email**: lifeskills@quizykoo.com

## File structure
```
index.html          ← single-page source, matches live artifact
```
Covers are **not** stored locally — they live in the artifact's asset store as `/_blob/<id>` URLs.
These URLs only resolve when served from the artifact. Do not replace them.

## Book data
All 20 books are in the `BOOKS` const array near the top of the `<script>` block.
Each entry: `{ id, set, title, blob }` — `blob` is the asset-store ID, used as `/_blob/<blob>`.

### Asset-store cover IDs (for reference)
| # | Title | Blob ID |
|---|-------|---------|
| 1 | Good Manners & Politeness | `5d601881e0dab4d13d1ff3378901d75a` |
| 2 | Sharing & Caring | `1c5ac68f4481156bd2d10137766690d1` |
| 3 | Listening & Communication | `5fe1115f3f379a2578421828d9164ec8` |
| 4 | Friendship & Teamwork | `b0ba15077f0ccd730fe7dcb154e53df2` |
| 5 | Respect & Kindness | `d02b1533bd870fc5f4d002a0cef2d546` |
| 6 | Understanding My Feelings | `e5199b509562e76cf6605ea981ddb9d2` |
| 7 | Managing Anger & Frustration | `86068f3ddda4677385a95835d31686c9` |
| 8 | Empathy & Caring for Others | `c8201c0d276d3b21d5cf62e4b4358492` |
| 9 | Confidence & Self-Esteem | `8c9e277fcea807fd915fc84c02626235` |
| 10 | Mindfulness & Staying Calm | `11da7a6a6a269eeb66048646985fecd6` |
| 11 | Healthy Habits | `86bd7aef3c8334205bea7bbc76724df2` |
| 12 | Cleanliness & Organization | `0213534b509c19ddf4448a52ddfadde7` |
| 13 | Helping at Home | `ec543f3cd8ec800d0edeff31403b591f` |
| 14 | Time & Routine Skills | `6ffb59f0ff9ade5205d9b7d309389ca1` |
| 15 | Safety & Awareness | `a85a478dd46abed5eee008951ad1d739` |
| 16 | Caring for Nature | `3b948db9e4e332e3cbbfcdbe6c517a37` |
| 17 | Animals & Kindness | `2a228de7bd1289a119667b9752aa7dee` |
| 18 | Saving Water & Energy | `9db0bf6bf561f554af37048ef1bbefd3` |
| 19 | Recycling & Clean Living | `580888265b9b0a2bd74ac803fe9b38cf` |
| 20 | Being a Responsible Citizen | `2e59f3f51d6775b4a410b4dfc4aa5bbe` |

## Sets
| Set | Colour | Books |
|-----|--------|-------|
| Set 1 — Social Skills | Teal `#1D8A99` | 1–5 |
| Set 2 — Emotional Intelligence | Coral `#E05C4B` | 6–10 |
| Set 3 — Life & Home Skills | Purple `#7B5EA7` | 11–15 |
| Set 4 — Planet & Citizenship | Green `#4A9B6F` | 16–20 |

## Design tokens
Font: Nunito (Google Fonts) · Background: `#FAFAF8` cream · Dark-mode aware via CSS tokens on `:root`.

## To update and publish via Claude Code
```
# Open in Claude Code, then in Claude:
# 1. Edit index.html (update Amazon links, text, etc.)
# 2. Tell Claude: "Publish this to https://claude.ai/artifact/Lf11R3fiL2rMZgWc2bvM5Q"
```

## Amazon links
Each book card links to its KDP product page. Links are in the BOOKS array in `index.html`.
Original covers (JPG) are in Dropbox → `00_FINISHED BOOKS / 0_LIVE ON AMAZON - older EPUBs`.
