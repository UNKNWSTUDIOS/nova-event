# Speaker notes — Nova × unknw, 29.09, 19:00 (90 min slot; talk ~50, Q&A rest)

Timing target per act. Deep-link: index.html#N.

## Act 1 · Basics (19:00–19:15) · slides 01–07
01 cover — 30s. Who I am: 20 years studio, unknw.com was on Webflow until 2025.
02 agenda — 30s. "Slides first, then real repos on screen. Interrupt me."
03 why leave — 3 min. Give the builder its due (speed, no engineer, one bill). Then the five things it takes back. Ceiling / loop / system / exit / cost. The exit one is the killer: "you've been renting your own website".
04 what changed — 2 min. The three flips. The point: custom code lost because it was SLOW, not because it was worse. That variable changed in 2025.
05 what Claude Code is — 3 min. "Colleague in the terminal", not a chat. It reads the repo, edits, runs, opens the browser, commits. Then the honest column: not a designer, not magic, not free. What you need: Mac, Node, git, editor, Max subscription, two days of patience.
06 session stage — 2 min. Let it type. Narrate: "I said one sentence. It read the token file, changed one class, opened the browser, checked, reported, asked before committing." That's the whole product.
07 the loop — 3 min. Left column is their life today. Right column is the new one. Underline "Vercel deploys in 40 seconds" and "client wants a change → one sentence".

## Act 2 · Quirks (19:15–19:35) · slides 08–10
08 three exits — 5 min. Webflow exports static HTML (best of three), Framer exports nothing, Wix exports nothing. Nobody exports interactions. CMS → CSV everywhere.
09 what you take — 5 min. Content, assets (originals!), URLs, design decisions read off the live site, screenshots of every page. LEAVE the HTML — say it twice. "The builder is a source of truth for content, not for code."
10 the traps — 8 min, this is the meat for them. Webflow: CDN resizes, rich text as HTML in CSV, fonts not in export, symbols map to components. Framer: fake scroll, per-frame breakpoints, outlined text, localisation. Wix: absolute positioning (nothing maps), Wix apps need replacements, ugly URLs → 301 everything, DNS last. Ask the room which platform they're on.

## Act 3 · Pipeline (19:35–20:00) · slides 11–19
11 pipeline — 3 min. Five stages, two weeks, one person. Audit → System → Components → Pages → Ship. System stage is red because it's the one people skip.
12 audit stage — 2 min. Let it type. "Day one is counting. 14 font sizes → 6. 9 greys → 3. Two dead pages."
13 tokens first — 4 min. Show the actual :root. Read them off the builder site; round to a system; name by role; put them on /ds; write the rule in CLAUDE.md. "A raw hex in a component is a bug."
14 /ds shot — 1 min. "This page is read by Claude AND by every freelancer we hire."
15 CLAUDE.md — 4 min. Read two rules aloud. "This file is where your taste goes. The model has none of yours until you write it down." Grew over a year, ~150 lines.
16 components — 3 min. Eight things, then compose. ORDER: tokens → ui → fx → layout → primitives → pages. "If it starts a page before Nav exists, stop it."
17 prompts — 4 min. Three prompts, same page. Too short → generic. Adjective soup → generic with a gradient. A brief → screenshots, JSON, named components, tolerance, and "check in the browser before reporting".
18 page stage — 2 min. Let it type. Point at "compare → gap 40 vs 48 → fix → compare ✓".
19 result — 1 min. unknw.com home + case. ~40 pages, every one is JSON + eight components.

## Act 4 · Environment (20:00–20:20) · slides 20–24
20 stack — 3 min. Boring on purpose. Next or Vite; TS; plain CSS w/ tokens; JSON/MDX content, Sanity only if the client needs a panel; CSS + GSAP + View Transitions; GitHub + Vercel + Resend. DNS last.
21 setup stage — 3 min. Let it type. Six commands, /init, then the first prompt is the design-system skeleton.
22 day to day — 4 min. Six habits. One task per session; look before you approve; commit small; corrections → rules; preview URLs for clients; content stays in JSON.
23 tips — 4 min. Screenshots are the spec; give it the browser; make it measure; plan mode; skills. Don't let it invent; fonts are files; mobile is a second brief; cost; it will be wrong like a junior.
24 when to stay — 2 min. Honest version. Three stay, three move.

## Close (20:20) · slides 25–26
25 five things — 1 min. Read them.
26 questions — Q&A to 20:30+.

## Live demo fallback
If the room wants to see the real thing: open ~/code/unknw-web in a terminal, `claude`, ask it to "list the design-system rules from CLAUDE.md and show me /ds" — cheap, safe, no edits.
